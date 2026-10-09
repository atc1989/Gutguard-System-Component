# Gutguard Unified Platform Architecture v2 (Reconciled)

**Date:** 3 October 2026
**Owner:** CSA, Founder, Chairman and CEO, Gutguard Corp.
**Status:** Replaces the devs' Architecture Proposal (v1)

All diagrams are in Mermaid. They render in GitHub, GitLab, VS Code (Mermaid extension) and Obsidian.

---

## Contents

1. Purpose and reconciliation rule
2. Core principle and member journey
3. System registry
4. Gates and business rules
5. Identity, roles and member record
6. Access matrix
7. Data ownership
8. Integration events
9. Key flows
10. Tech stack, security and reporting
11. Build phases
12. Open decisions

**Diagram index**

| No. | Diagram | Section |
|---|---|---|
| D1 | System architecture | 2 |
| D2 | Member journey (state machine) | 2 |
| D3 | Gate check: opening GEMA | 4 |
| D4 | Status state machines | 5 |
| D5 | Core database (ER) | 5 |
| D6 | Lifestyle main tables (ER) | 7 |
| D7 | Event trigger map | 8 |
| D8 | Event processing pipeline | 8 |
| D9 | Single Sign-On | 9 |
| D10 | Guest to member | 9 |
| D11 | 5-Night Watch trial | 9 |
| D12 | Member to Gentrep | 9 |
| D13 | GOCC credit | 9 |
| D14 | Lifestyle Coach, Phase 1 | 9 |
| D15 | Build phases | 11 |

---

## 1. Purpose and reconciliation rule

This v2 replaces the devs' Architecture Proposal (v1). It keeps the devs' technology and adds our locked business logic.

**The rule:** Our logic and design govern the member journey, the gates, the app roles and the names. The devs' document governs the tech stack, login method, domains, tables, event pattern and security. Where v1 and v2 differ on logic, v2 wins.

**Adopted from v1 (devs):**

- One Gutguard ID with Single Sign-On at `auth.gutguard.ph`
- Gutguard Core API at `api.gutguard.ph`
- One subdomain per app
- The `users`, `profiles`, `roles` and `user_roles` tables
- The `integration_events` table and sync worker
- The `audit_logs` table and the 10 security rules
- The tech stack: Next.js, React, TypeScript, Tailwind, Supabase, PostgreSQL
- The admin portal at `admin.gutguard.ph`

**Changed in v2 (our logic):**

- Lifestyle is the product-use app, not only a prospect app
- Our gates are written as Core rules, not left to roles alone
- Our funnel stages, E-Points ledger, BASE, GOCC credits and the Lifestyle Coach are added
- The event log moves to Phase 1

---

## 2. Core principle and member journey

One person, one Gutguard ID, one member record, many apps. Every app reads the person's place in the journey from Core.

### D1. System architecture

Apps never call each other directly. Every app logs in through Gutguard ID, then calls Core and writes events.

```mermaid
flowchart TB
    P["Prospect / Member"]

    subgraph APPS["Gutguard apps (one login for all)"]
        direction LR
        subgraph BUY["For buying"]
            direction TB
            WEB["Website<br/>gutguard.ph"]
            SHOP["Shop<br/>shop.gutguard.ph"]
        end
        subgraph USE["For using"]
            LIFE["Lifestyle<br/>lifestyle.gutguard.ph<br/>Rewards mode + Member mode"]
        end
        subgraph BIZ["Business apps"]
            direction TB
            GEMA["GEMA<br/>gema.gutguard.ph"]
            ACAD["Gentrep Academy<br/>gentrep.gutguard.ph"]
            GGV["GG Verse<br/>ggverse.gutguard.ph"]
        end
        subgraph HEALTH["Health"]
            GLIS["BioScan / GLIS<br/>glis.gutguard.ph"]
        end
    end

    ID["Gutguard ID<br/>auth.gutguard.ph<br/>One Account login, SSO"]
    CORE["Gutguard Core<br/>api.gutguard.ph<br/>member record, roles, gates"]
    EV[("integration_events")]
    AUD[("audit_logs")]
    WK["Sync Worker"]
    COACH["Lifestyle Coach<br/>Col. Lacto"]
    ADMIN["Admin<br/>admin.gutguard.ph"]
    MAYA["Maya payments"]
    TG["Telegram / Messenger"]

    P --> APPS
    APPS -->|"1. login"| ID
    ID -->|"session + gates"| CORE
    APPS -->|"2. API calls + events"| CORE
    SHOP -.->|pay| MAYA
    CORE --> EV
    CORE --> AUD
    EV --> WK
    WK -->|"update member_status"| CORE
    WK --> COACH
    COACH -->|"messages, push"| APPS
    COACH -->|"sponsor alerts"| TG
    ADMIN --> CORE
```

### D2. Member journey (state machine)

Everyone starts as a product user. BASE gates every earner.

```mermaid
stateDiagram-v2
    state "Suspect<br/>name on a list" as Suspect
    state "Prospect<br/>registered by event link" as Prospect
    state "Lead<br/>checked in by QR" as Lead
    state "Lifestyle Member<br/>paid in" as Member
    state "User only" as UserOnly
    state "Affiliate<br/>self-serve, free" as Affiliate
    state "BASE Activation" as BASE
    state "Gentrep Seller<br/>direct commission" as Seller
    state "Gentrep Builder<br/>sponsor invite only" as Builder
    state "Business apps open<br/>GEMA, Gentrep Academy, GG Verse" as Apps

    [*] --> Suspect
    Suspect --> Prospect: registers via GEMA event link
    Prospect --> Lead: QR check-in at the event
    Lead --> Member: pays in at the Shop
    Member --> UserOnly: stays a product user
    Member --> Affiliate: turns on affiliate
    Member --> BASE: starts BASE
    BASE --> Seller: BASE activated
    BASE --> Builder: BASE activated and enrolled by invite
    Seller --> Builder: steps up by invite
    Builder --> Apps
```

A Seller earns direct commission without GEMA and can step up to Builder at any time.

---

## 3. System registry

The ecosystem has 10 systems on the devs' domains. The website is for buying. Lifestyle is for using. GEMA, Gentrep Academy and GG Verse are business apps.

| System | Domain | Job | Who uses it |
|---|---|---|---|
| Gutguard ID | auth.gutguard.ph | One Account login and Single Sign-On for all apps | Everyone |
| Gutguard Core | api.gutguard.ph | Member record, roles, gates, event log, audit log | All apps (no screens) |
| Website | gutguard.ph | Public site: About, science, 5-Night Watch hook, BioScan story | Public |
| Shop | shop.gutguard.ph | All buying: 5-Night Watch ₱499, Lifestyle Protocol, subscriptions, gift for family. Same look as the website | Public, members |
| Lifestyle | lifestyle.gutguard.ph | One app, two modes. **Rewards mode:** guest card, invites, E-Points. **Member mode:** My Lifestyle (doses, Reveille / Midday / Taps), My Team, My Journey, BASE Activation, Gentrep Officer Dashboard | Prospects, all members |
| GEMA | gema.gutguard.ph | Events, event links, QR check-in, Event Requests, AER, Members Training Record, My Network Status | BASE-activated Builders, staff |
| Gentrep Academy | gentrep.gutguard.ph | GOCC courses, Zoom lectures, title checklists, certificates | BASE-activated Builders, instructors |
| GG Verse | ggverse.gutguard.ph | Genealogy, sales, commissions, ranks, bubble chart, Members Shop door | Paid-in Gentreps |
| BioScan / GLIS | glis.gutguard.ph | Lab results, GLIS score, MiAge (Beta), health consent | Members, doctors, medical staff |
| Admin | admin.gutguard.ph | Users, roles, orders, AER audit, reports, system health | Company staff |

**Lifestyle Coach (Col. Lacto)** is not a separate app. It is a Core service that sends text messages and push notifications inside all four member apps. No voice.

---

## 4. Gates and business rules

Core checks these rules on the server. An app never decides them alone, and the frontend is never trusted.

1. **One person, one ID.** The Lifestyle card number (16 digits) and QR belong to the Gutguard ID. When a guest becomes a member, the card keeps the same number.
2. **Product user first.** Everyone starts as a Lifestyle Member. Then each person picks one path: user only, Affiliate, Gentrep Seller or Gentrep Builder.
3. **Believer before builder.** Earning tools open only after the person's OWN pay-in, not a pay-in in his team.
4. **Gentrep by invitation.** Affiliate is self-serve. Gentrep enrolment needs an invite link issued by the sponsor for that one person.
5. **BASE gates every earner.** My Team, GEMA and the 2Lt Course open only after BASE Activation is complete. This applies to Sellers and Builders.
6. **Every invite is a GEMA event link.** A suspect enters the funnel only through an event invitation.
7. **Pay on attendance.** Registration is shown but not paid. The inviter's Rewards Credit lands only at the guest's GEMA QR check-in. Rewards Credit is product credit only, never cash.
8. **Two ledgers, never mixed.** E-Points (product credit) live in Lifestyle. Commissions live in GG Verse.
9. **Rank is earned, never bought.** GOCC titles (2Lt, 1Lt, Capt, Major) live in Gentrep Academy. Commission ranks live in GG Verse. The product ladder is separate from both.
10. **Not in GEMA, did not happen.** A GOCC credit is written only by a signed After Event Report (AER).
11. **No earning talk before pay-in.** Ginhawa pages and prospect screens show health content only.
12. **Active means one transaction in the last 60 days.**
13. **Buying for family.** E-Points go to the payer. The person bought for joins under the payer as referrer.

### D3. Gate check: opening GEMA

The same pattern applies to Academy and GG Verse.

```mermaid
flowchart TD
    A["Member opens GEMA"] --> B{"pay_in_status = paid?"}
    B -- No --> X1["Show: Start my Lifestyle Protocol"]
    B -- Yes --> C{"base_status = activated?"}
    C -- No --> X2["Show locked My Team:<br/>N to go, Continue BASE"]
    C -- Yes --> D{"fork_type = builder<br/>and gentrep_invite = enrolled?"}
    D -- No --> X3["Show: Ask my sponsor for access"]
    D -- Yes --> E["Open GEMA"]
```

---

## 5. Identity, roles and member record

Keep the devs' `users`, `profiles`, `roles` and `user_roles` tables as written. Add one `member_status` table in Core.

- **Roles** say what a person may open.
- **Status** says where the person is in the journey.
- The gates read status, not roles alone.

### member_status (new, in Core)

| Field | Values |
|---|---|
| user_id | Gutguard ID |
| card_no | 16-digit Lifestyle card number |
| funnel_stage | suspect, prospect, lead, member |
| fork_type | user, affiliate, seller, builder |
| pay_in_status | none, paid |
| base_status | not_started, in_progress, activated |
| gentrep_invite | none, requested, issued, enrolled |
| sponsor_id | Gutguard ID of the direct sponsor |
| center_id, area | Product center and Director's area |
| member_type | A builder, B seller, C user (set by the system from history, not by the sponsor) |
| active | true if one transaction in the last 60 days |
| gocc_title | none, 2Lt, 1Lt, Capt, Major (read from Academy) |
| commission_rank | read from GG Verse |

### Funnel stages (our definitions)

- **Suspect:** on a member's list, not yet registered
- **Prospect:** registered through an event link
- **Lead:** attended a GEMA event (QR check-in)
- **Member:** paid in

### Roles (replaces the v1 list)

`prospect`, `lifestyle_member`, `affiliate`, `gentrep_seller`, `gentrep_builder`, `doctor`, `instructor`, `course_director`, `event_supervisor`, `center_commander`, `center_staff`, `csr`, `accounting`, `admin`, `super_admin`

### D4. Status state machines

**pay_in_status and base_status**

```mermaid
stateDiagram-v2
    direction LR
    state "pay_in_status" as PAY {
        none --> paid: shop.order_paid
    }
    state "base_status" as BS {
        not_started --> in_progress: first BASE step
        in_progress --> activated: all BASE steps done
    }
```

**gentrep_invite**

```mermaid
stateDiagram-v2
    direction LR
    [*] --> none
    none --> requested: member asks sponsor
    none --> issued: sponsor issues directly
    requested --> issued: sponsor issues link
    issued --> enrolled: member enrols
    enrolled --> [*]
```

**Invite stage (one row per shared invite, in Lifestyle)**

```mermaid
stateDiagram-v2
    direction LR
    [*] --> sent
    sent --> registered: guest registers
    registered --> showed: QR check-in, inviter credit vests
    showed --> bought: guest pays in
    bought --> [*]
```

### D5. Core database (ER)

```mermaid
erDiagram
    users ||--|| profiles : has
    users ||--o{ user_roles : holds
    roles ||--o{ user_roles : grants
    users ||--|| member_status : has
    users ||--o{ member_status : sponsors
    users ||--o{ integration_events : about
    users ||--o{ audit_logs : about

    users {
        uuid id PK
        text email
        text mobile
        text status
        timestamptz created_at
        timestamptz updated_at
    }
    profiles {
        uuid user_id FK
        text first_name
        text middle_name
        text last_name
        text city
        text province
        text country
    }
    roles {
        uuid id PK
        text name
    }
    user_roles {
        uuid id PK
        uuid user_id FK
        uuid role_id FK
        text status
        timestamptz assigned_at
        uuid assigned_by
        timestamptz expires_at
    }
    member_status {
        uuid user_id PK
        text card_no
        text funnel_stage
        text fork_type
        text pay_in_status
        text base_status
        text gentrep_invite
        uuid sponsor_id FK
        text center_id
        text area
        text member_type
        boolean active
        text gocc_title
        text commission_rank
    }
    integration_events {
        uuid id PK
        text event_type
        text source_system
        uuid user_id FK
        text entity_type
        text entity_id
        jsonb payload
        text status
        int retry_count
        timestamptz created_at
        timestamptz processed_at
    }
    audit_logs {
        uuid id PK
        uuid user_id FK
        uuid actor_user_id
        text source_system
        text action
        text entity_type
        text entity_id
        jsonb old_value
        jsonb new_value
        timestamptz created_at
    }
```

---

## 6. Access matrix

This replaces the v1 matrix. Gates in Section 4 still apply on top of roles.

| Role | Website / Shop | Lifestyle | GEMA | Academy | GG Verse | BioScan / GLIS | Admin |
|---|---|---|---|---|---|---|---|
| Prospect | Public | Rewards mode | Event link only | No | No | No | No |
| Lifestyle Member | Yes | Member mode | No | No | No | Own results | No |
| Affiliate | Yes | Member mode + share | No | No | No | Own results | No |
| Gentrep Seller | Yes | Member mode | No | To confirm | Commission view (to confirm) | Own results | No |
| Gentrep Builder | Yes | Member mode + My Team | Yes | Yes | Yes | Own results | No |
| Doctor | Yes | No | No | No | No | Consenting patients only | No |
| Instructor / Course Director | Yes | As member | Yes | Instructor tools | As member | Own results | No |
| Event Supervisor | Yes | As member | Approve, sign AER | As member | As member | Own results | No |
| Staff | Limited | Support view | By assignment | By assignment | Limited | Medical staff only | By assignment |
| Admin | Yes | Yes | Yes | Yes | Yes | Audit-logged only | Yes |

---

## 7. Data ownership

The devs' rule stays: each app owns its business data, and Core owns identity, access and integration. The biggest change is Lifestyle: it owns product use, not only prospects.

| System | Owns |
|---|---|
| Core | Users, profiles, roles, member_status, sponsor link, center and area, integration_events, audit_logs |
| Lifestyle | Rewards card, invites (link token and stage: sent, registered, showed, bought), E-Points ledger (point_events, the single E-Points record), dosing settings, dose logs (Reveille / Midday / Taps), ATP day, adherence (x/7, x/28), reminders, 5-Night Watch nights, BASE progress, Story of Hope consent |
| Shop | Products, prices, cart, orders, payments (Maya), subscriptions, delivery status, inventory |
| GEMA | Events, event links, registrations, QR check-ins, Event Requests with named role holders, AERs, training credit lines |
| Gentrep Academy | Courses, lectures, Zoom attendance, enrolments, title checklists (Needed / Done / Left), titles earned, certificates |
| GG Verse | Genealogy, sales and BV, commissions, ranks, incentives, Members Shop access |
| BioScan / GLIS | Lab results, GLIS scores, MiAge results, health consent. Medical data never leaves this system except as a score the member has agreed to share |
| Lifestyle Coach | Message rules, messages sent, sponsor alerts. It reads events; it owns no member data |

### D6. Lifestyle main tables (ER)

Field names are proposed. Devs may adjust names, not the meaning.

```mermaid
erDiagram
    lifestyle_cards ||--o{ invites : shares
    lifestyle_cards ||--o{ point_events : earns
    lifestyle_cards ||--o{ dosing_settings : sets
    lifestyle_cards ||--o{ dose_logs : logs
    lifestyle_cards ||--o{ watch_nights : plays

    lifestyle_cards {
        uuid user_id PK
        text card_no
        text mode
        int atp_day
    }
    invites {
        uuid id PK
        uuid inviter_id FK
        text token
        text gema_event_id
        uuid invitee_id
        text stage
    }
    point_events {
        uuid id PK
        uuid user_id FK
        text type
        int points
        uuid source_event_id
        timestamptz created_at
    }
    dosing_settings {
        uuid user_id FK
        text slot
        int recommended_capsules
        int capsules
        boolean adjusted
    }
    dose_logs {
        uuid id PK
        uuid user_id FK
        date log_date
        text slot
        int capsules
        timestamptz logged_at
    }
    watch_nights {
        uuid user_id FK
        int night_no
        date night_date
        boolean video_played
    }
```

- `slot` values: `reveille`, `midday`, `taps`
- `mode` values: `rewards`, `member`
- `stage` values: `sent`, `registered`, `showed`, `bought`

---

## 8. Integration events

Use the devs' `integration_events` table exactly as written in v1 (PostgreSQL, JSONB payload, status, retry_count). This table is also our funnel meter and the Coach's trigger source, so it is built in Phase 1.

Keep the v1 event names. Add these:

```text
invite.sent
invite.registered
prospect.registered
event.checked_in            -> triggers referral.vested
referral.vested

member.paid_in
points.earned
points.redeemed

lifestyle.dose_logged
lifestyle.taps_logged
lifestyle.night_completed   (5-Night Watch, Nights 1-5)
lifestyle.atp_day_reached

base.step_completed
base.activated

gentrep.invite_requested
gentrep.invite_issued
gentrep.enrolled

gema.event_requested
gema.event_approved
gema.aer_signed             -> triggers academy.credit_awarded
academy.credit_awarded
academy.title_earned

shop.delivered              -> starts 5-Night Watch Night 1
shop.subscription_renewed

glis.result_uploaded
glis.scored

coach.message_sent
coach.sponsor_alerted
member.became_active
member.became_inactive
```

### D7. Event trigger map

What each key event causes.

```mermaid
flowchart LR
    E1["event.checked_in<br/>GEMA"] --> R1["referral.vested<br/>inviter Rewards Credit"]
    E1 --> R2["funnel_stage = lead<br/>guest points vest"]
    E2["shop.order_paid<br/>Shop"] --> R3["member.paid_in<br/>card flips to member"]
    E3["shop.delivered<br/>Shop"] --> R4["5-Night Watch<br/>Night 1 starts"]
    E4["gema.aer_signed<br/>GEMA"] --> R5["academy.credit_awarded<br/>each role holder"]
    R5 --> R6["academy.title_earned<br/>when checklist is complete"]
    E5["base.activated<br/>Lifestyle"] --> R7["My Team unlocks"]
    E6["gentrep.enrolled<br/>Core"] --> R8["GEMA, Academy,<br/>GG Verse open"]
    E7["lifestyle.taps_logged<br/>shop.order_paid"] --> R9["Lifestyle Coach rules run"]
    E8["any transaction"] --> R10["active = true<br/>for 60 days"]
```

### D8. Event processing pipeline

```mermaid
flowchart LR
    APP["Any Gutguard app"] -->|write| EV[("integration_events<br/>status = pending")]
    EV --> WK["Sync Worker<br/>Edge Function / scheduled job"]
    WK --> OK{"Processed?"}
    OK -- Yes --> DONE["status = processed<br/>processed_at set"]
    OK -- No --> RETRY{"retry_count < limit?"}
    RETRY -- Yes --> EV
    RETRY -- No --> FAIL["status = failed<br/>shown in Admin, Failed Syncs"]
    DONE --> CORE["Core updates member_status"]
    DONE --> OTHER["Other apps notified by webhook"]
    DONE --> COACH["Lifestyle Coach"]
```

---

## 9. Key flows

These flows replace the v1 prospect and membership flows (v1 sections 4, 9, 10 and 11).

### D9. Single Sign-On (from v1, unchanged)

```mermaid
sequenceDiagram
    actor U as User
    participant G as GEMA
    participant A as auth.gutguard.ph
    participant C as Gutguard Core
    participant T as Gentrep Academy

    U->>G: Open gema.gutguard.ph
    G->>A: Redirect for login
    A->>U: Login screen
    U->>A: Submit credentials
    A->>C: Verify user, roles and member_status
    C-->>A: Profile, roles, gates passed
    A-->>G: Authenticated session
    G-->>U: GEMA opens
    U->>T: Later, open gentrep.gutguard.ph
    T->>A: Check session
    A-->>T: Session valid
    T-->>U: Academy opens, no second login
```

### D10. Guest to member

1. A member shares a GEMA event link.
2. The guest registers with name and mobile. A Lifestyle card opens in Rewards mode with pending points.
3. The guest attends and the card QR is scanned at check-in. The guest's points vest. The inviter's Rewards Credit vests.
4. The guest taps "Start my Lifestyle Protocol" and pays in the Shop (card number carried in the link).
5. The card flips from GUEST to LIFESTYLE MEMBER with the same number. Lifestyle opens in Member mode with no second login.

```mermaid
sequenceDiagram
    actor M as Member (inviter)
    actor G as Guest
    participant E as GEMA
    participant L as Lifestyle
    participant C as Core
    participant S as Shop

    M->>E: Share event link
    E-->>G: Event page (health content only)
    G->>L: Register with name and mobile
    L->>C: Create Gutguard ID, funnel_stage = prospect
    C-->>L: card_no, pending points
    Note over L: Card shows GUEST
    G->>E: Attends, card QR scanned
    E->>C: event.checked_in
    C->>C: funnel_stage = lead, guest points vest
    C->>C: referral.vested, inviter Rewards Credit
    G->>L: Tap Start my Lifestyle Protocol
    L->>S: Open checkout with card_no
    S->>S: Pay with Maya
    S->>C: shop.order_paid
    C->>C: member.paid_in, funnel_stage = member
    C-->>L: Card flips to LIFESTYLE MEMBER, same number
    L-->>G: Member mode opens, no second login
```

### D11. 5-Night Watch trial

1. The buyer pays ₱499 in the Shop. Shipping is free.
2. The courier's "Delivered" status starts Night 1 automatically.
3. Each night at Taps, Lifestyle plays that night's short video (Nights 1 to 5).

```mermaid
flowchart LR
    A["Buy 5-Night Watch<br/>₱499, free shipping"] --> B["Courier status:<br/>Delivered"]
    B -->|shop.delivered| C["Night 1 starts<br/>automatically"]
    C --> D["Each night at Taps:<br/>play that night's video"]
    D --> E{"Night 5 done?"}
    E -- No --> D
    E -- Yes --> F["Sponsor call,<br/>then package offer"]
```

### D12. Member to Gentrep

1. The member completes BASE Activation in Lifestyle.
2. The sponsor issues a Gentrep invite for that member.
3. The member enrols. GEMA, Gentrep Academy and GG Verse open.

```mermaid
sequenceDiagram
    actor M as Member
    actor SP as Sponsor
    participant L as Lifestyle
    participant C as Core

    M->>L: Complete BASE steps
    L->>C: base.activated
    C-->>L: My Team unlocks
    M->>L: Tap Be a Gentrep, ask my sponsor
    L->>C: gentrep.invite_requested
    C-->>SP: Alert: member asks for access
    SP->>C: Issue invite link for this member
    C->>C: gentrep.invite_issued
    M->>C: Enrol through the link
    C->>C: gentrep.enrolled, fork_type = builder
    C-->>M: GEMA, Academy and GG Verse open
```

### D13. GOCC credit

1. An Event Manager (PL or CC) submits a GEMA Event Request naming every role holder.
2. Management approves. The event runs. Attendees check in by QR.
3. The Event Supervisor signs the AER within 24 hours.
4. Each named role holder gets a credit line on his Training Record. Academy updates the title checklist.

```mermaid
sequenceDiagram
    actor EM as Event Manager (PL or CC)
    actor SUP as Event Supervisor
    participant E as GEMA
    participant C as Core
    participant A as Gentrep Academy

    EM->>E: Event Request with all role holders named
    E->>SUP: Request for approval
    SUP->>E: Approve
    E->>C: gema.event_approved
    Note over E: Event runs, attendees check in by QR
    SUP->>E: Sign AER within 24 hours
    E->>C: gema.aer_signed
    C->>A: academy.credit_awarded for each role holder
    A->>A: Update title checklist, Needed / Done / Left
    A->>C: academy.title_earned when complete
    C->>C: member_status.gocc_title updated
    Note over SUP: 30 guests and above: company management supervises.<br/>Below 30: a Company Commander may supervise.
```

### D14. Lifestyle Coach, Phase 1

1. The Coach reads two sources only: Lifestyle dose and Taps logs, and Shop orders.
2. It sends Col. Lacto's message to the member and alerts the sponsor when the member slips.
3. Its one KPI is Active Protocol Users.

```mermaid
flowchart TD
    S1["Lifestyle<br/>dose logs, Taps, ATP day"] --> R["Coach rules"]
    S2["Shop<br/>orders, supply left"] --> R
    R --> Q{"Member on track?"}
    Q -- Yes --> M1["Col. Lacto message:<br/>encourage, mark the day"]
    Q -- "No: missed doses" --> M2["Col. Lacto message<br/>to the member"]
    M2 --> AL["Alert the sponsor<br/>Telegram / Messenger"]
    Q -- "Supply running low" --> M3["Reorder reminder"]
    M1 --> K["KPI: Active Protocol Users"]
    AL --> K
    M3 --> K
```

---

## 10. Tech stack, security and reporting

The devs' stack is adopted as written. Three items are added: payments, messaging and design tokens.

| Layer | Choice |
|---|---|
| Frontend | Next.js, React, TypeScript, Tailwind CSS |
| Login | Supabase Auth behind auth.gutguard.ph, OAuth 2.0 / OpenID Connect style SSO |
| Database | PostgreSQL on Supabase, Row Level Security on |
| API | Next.js route handlers and Supabase Edge Functions at api.gutguard.ph |
| Events | integration_events table, webhooks, Edge Functions, scheduled workers. No Kafka or RabbitMQ in version 1 |
| Payments (added) | Maya only at launch. Monthly payment link until Maya card-on-file is ready. No COD, no instalments |
| Messaging (added) | Telegram bot and FB Messenger for sponsor alerts and member reminders; app push notifications for the Coach |
| Design (added) | Shared ggverse-theme tokens. Shop and Lifestyle share the website's look. GEMA, Academy and GG Verse may keep their own look. The membership card keeps its royal blue and silver identity |

**Security:** Adopt the devs' 10 security rules and the `audit_logs` table. Two additions:

- The gates in Section 4 are checked in Core on the server, every time.
- Health data (GLIS, MiAge, Story of Hope) needs the member's consent under RA 10173 before it is stored or shared.

**Reporting:** Management dashboards live in `admin.gutguard.ph`. Obsidian is kept for developer documentation only. No member names or health data go into the vault, because vault files sit on personal laptops.

---

## 11. Build phases

Five phases. The event log moves into Phase 1, because the funnel numbers, the Coach and the Officer Dashboard all depend on it.

1. **Phase 1: Identity, member record and event log.** Gutguard ID, the v1 tables, member_status, integration_events and audit_logs. *Done when:* one login works, every person has one record, and every action is counted.
2. **Phase 2: Buy and use.** Shop with Maya, and Lifestyle in both modes (Rewards and Member), including the 5-Night Watch nights. *Done when:* a guest can register, attend, pay and land in Member mode with the same card.
3. **Phase 3: Connect the business apps.** Map existing GEMA, Gentrep Academy and GG Verse users to the Gutguard ID. Wire check-in to referral vesting, and the AER to training credits. *Done when:* a QR scan vests a referral and a signed AER writes a credit.
4. **Phase 4: Coach and health.** Lifestyle Coach Phase 1 (dose logs and orders only). BioScan / GLIS connected with consent.
5. **Phase 5: Admin and reports.** admin.gutguard.ph with users, roles, AER audit, failed syncs and management dashboards.

### D15. Build phases

```mermaid
flowchart LR
    P1["Phase 1<br/>Identity, member record,<br/>event log"] -->|"one login, one record,<br/>every action counted"| P2["Phase 2<br/>Shop + Lifestyle<br/>both modes"]
    P2 -->|"guest pays and lands<br/>in Member mode"| P3["Phase 3<br/>Connect GEMA,<br/>Academy, GG Verse"]
    P3 -->|"QR vests referral,<br/>AER writes credit"| P4["Phase 4<br/>Coach + BioScan / GLIS"]
    P4 --> P5["Phase 5<br/>Admin + reports"]
```

---

## 12. Open decisions

These need a ruling before the devs build the affected parts.

- [ ] **Members Shop:** a separate store, or a gated section of shop.gutguard.ph opened from GG Verse? The proposal is the gated section: one shop backend, gated by pay_in_status.
- [ ] **MiAge display:** where does the member see MiAge? The BioScan card shows inflammation only, so MiAge needs its own place, for example Lifestyle My Journey.
- [ ] **Operation 50 Stories:** does the challenge need GLIS scoring in the app at launch, or can the first season be scored by hand from partner-lab results? If in the app, BioScan / GLIS moves up to Phase 2.
- [ ] **E-Points values:** final earn values and the redemption cap come from the official marketing plan.
- [ ] **Officer Readiness Rating:** the 1 to 100 formula for the Gentrep Officer Dashboard.
- [ ] **Doctor access:** what a Clinical Partner doctor can see in BioScan / GLIS, and whether doctors need their own portal.
- [ ] **Gentrep Seller access:** does a Seller see Gentrep Academy, and where does a Seller view his direct commission (GG Verse or Lifestyle)?
