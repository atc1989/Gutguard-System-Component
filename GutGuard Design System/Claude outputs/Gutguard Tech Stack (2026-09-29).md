# TECH_STACK

Reviewed 29 September 2026 from relevant vault notes and local project code. Requested exclusions respected. Versions are from package manifests; live deployment settings are unverified.

## 1. Front end

- **Framework:** Next.js App Router + React. Lifestyle: Next 16.3.1 / React 19.2.8. Website/Doctors: Next ^16.2.6 / React ^19.2.6.
- **Language:** TypeScript 5; some existing JSX.
- **Styling:** GutGuard design-system CSS; CSS modules allowed. Since 8 Oct 2026, new apps may use Tailwind v4 through the GutGuard token bridge (Tech Stack note `06 - Tailwind Bridge`); existing apps keep design-system CSS. No shadcn. Older Landing/GEMA projects use Tailwind/shadcn with their own setup.
- **Routing/state:** Next.js routes; React hooks and Context.
- **Build/libraries:** Next.js + npm; Lucide icons; Lifestyle uses React Hook Form + Zod.

## 2. Back end

- **Server:** Next.js TypeScript Server Actions/HTTP handlers; Supabase Edge Functions (Deno).
- **Database/API:** Supabase PostgreSQL + RLS; REST/PostgREST and SQL RPCs. No ORM.
- **Login:** Email/password or OneGrinders username/password for members; email OTP for website partners. Mobile + SMS login is not implemented.
- **BioScan:** Separate Python/FastAPI service.

## 3. Services

- **Hosting/domains:** Vercel + Supabase. Website code supports `gutguard.ph`, `shop.gutguard.ph`, and `partners.gutguard.ph`. BioScan has Render configuration. DNS provider unverified.
- **SMS/email/storage:** iTexMo SMS adapter; Resend and Supabase Auth email; Supabase Storage.
- **Payments:** Maya hosted Checkout in website/Doctors. Enabled GCash/card/wallet channels need merchant confirmation. COD and instalment workflows not found.
- **Recurring billing:** Automatic monthly/every-3-months charging not found.
- **Analytics:** No dedicated analytics integration found in inspected website/Lifestyle code.

## 4. Existing systems to connect

- **GEMA:** Events, referrals, QR attendance, genealogy and commissions.
- **Members:** Supabase Auth + `public.profiles`, GEMA identity/member records, and shared One Account login code. Production rollout unverified.
- **E-Points:** Lifestyle balances/`point_events` and Doctors `partner_points`; unified cross-system reconciliation not established.
- **Orders:** Website uses `shop_orders`/`shop_order_items`; Lifestyle uses separate `orders`. Unified order sync not established.
- **Academy:** Training, BASE/ranks and certificates.
- **BioScan/GLIS:** Existing upload → extraction → confirmation/scoring API; Lifestyle connection not found.

## 5. Code rules

- **Folders:** `app/`, `components/`, `lib/`, `supabase/migrations/`, `public/`; some repos place app code under `src/`.
- **Naming:** Follow existing code: PascalCase components, camelCase functions, snake_case SQL.
- **Lint/format:** ESLint 9 + Next config; no Prettier config found in website/Doctors or Lifestyle.
- **Settings/keys:** Ignored `.env.local` locally; Vercel/Supabase secrets when deployed. Commit `.env.example` placeholders only. Secret keys stay server-side.

## 6. Repos and environments

- **Primary:** [Website/Doctors](https://github.com/atc1989/GutGuard-Doctors-HTML), [Lifestyle](https://github.com/atc1989/GutGuard-Life-Style).
- **Related:** [Landing](https://github.com/atc1989/GutGuard_Landing), [GEMA](https://github.com/atc1989/GEMA), [Academy](https://github.com/atc1989/gentrep-academy), [BioScan](https://github.com/atc1989/gutguard-bem).
- **Branches/releases:** Documented pattern: PR previews → checks/migrations/configuration → merge to configured production branch, usually `main` → Vercel deployment. Actual protections/bindings unverified.
- **Staging:** Code references [sandbox.gutguard.ph](https://sandbox.gutguard.ph) for the shop; availability unverified. Lifestyle frontend staging URL not established.

## 7. Testing

- **Lifestyle/website:** Small Node-based tests, ESLint and Next build.
- **Academy:** Node/tsx tests, pgTAP database tests and concurrency checks.
- **BioScan:** pytest.
- No configured Playwright/Jest suite found in the two primary apps. Tests were not run for this document.

## 8. Handoff format

**Recommended:** React/TypeScript components, one Next.js route entry per page, reusable components, separate design-system CSS and assets. Clearly label mock data and unfinished integrations. Optional HTML reference for visual review.

## 9. Limits

- Lifestyle queues orders but its reviewed order action does not create Maya checkout.
- SMS login, recurring billing, COD/instalments and unified points/orders need additional work or confirmation.
- Cross-app login depends on shared Auth and domain configuration; mock/local-storage behavior is not production authorization.
- BioScan needs authenticated patient ownership and durable processing before connecting real member reports.
- Full prototype parity was not assessed because the requested prototype folders were excluded.
