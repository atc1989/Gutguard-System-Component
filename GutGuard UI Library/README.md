---
title: GutGuard UI Library
tags: [gutguard, ui-library, index]
updated: 2026-10-08
status: draft
code: D:\Users\najee\Downloads\Gutguard_Components_1\gutguard-ui
---

# GutGuard UI Library

Reusable components from the approved **Website, Shop and Lifestyle** screens (captured 5 Oct 2026), rebuilt in **Next.js 16 + Tailwind CSS v4**. Kept separate from [[GutGuard Design System/Components/Index|the GutGuard Design System]] (Doctors / booth / admin).

- **Code + showcase:** `D:\Users\najee\Downloads\Gutguard_Components_1\gutguard-ui`. Run `npm install`, then `npm run dev`, then open http://localhost:3000. Each component shows on a phone (390) and a desktop (1440), with its usage example and code to copy.
- **How the 79 captured parts map to these components:** [[00 - Component Inventory]]
- **New here / not seeing the changes?** [[01 - Sync and Team Guide]]
- **Tokens:** `gutguard-ui/app/globals.css` (`@theme`). Colours are only available as tokens; Tailwind's default palette is switched off.

## Primitives

[[Button]] · [[IconButton]] · [[Badge]] · [[Eyebrow]] · [[Price]] · [[Avatar]] · [[PointsPill]] · [[ProgressBar]] · [[Stepper]] · [[TextField]] · [[Checkbox]] · [[CodeInput]]

## Components

[[SegmentedControl]] · [[Tabs]] · [[OptionCard]] · [[ChoiceChip]] · [[Combobox]] · [[StatGroup]] · [[TrustLine]] · [[Note]] · [[LineItem]] · [[OrderTotals]] · [[ListRow]] · [[IconRow]] · [[Card]] · [[Quote]] · [[SectionHeading]] · [[Timeline]]

## Shell

[[TopBar]] · [[Footer]] · [[BottomBar]]

## Overlays & states

[[Sheet]] · [[MobileMenu]] · [[EmptyState]] · [[SuccessState]]

## Patterns (GutGuard-specific)

[[MemberCard]] · [[DoseRow]] · [[OfferCard]] · [[PersonRow]] · [[AdherenceCalendar]] · [[NutritionFacts]] · [[StepProgress]] · [[ProductHeader]]

## Sections (page-specific blocks)

Notes in `Sections/`. Built from the library, used on one page each.

- Website: [[Sections/Hero|Hero]] · [[Sections/BloodScanReadout|BloodScanReadout]] · [[Sections/MiAgeBlock|MiAgeBlock]] · [[Sections/TrajectoryChart|TrajectoryChart]] · [[Sections/StoryOfHope|StoryOfHope]] · [[Sections/ProtocolSteps|ProtocolSteps]]
- Lifestyle: [[Sections/MemberGreeting|MemberGreeting]] · [[Sections/ProtocolJourney|ProtocolJourney]] · [[Sections/BusinessTools|BusinessTools]] · [[Sections/AuthPanel|AuthPanel]]

## Screens (in the showcase)

Whole screens composed from the library, showing how the pieces combine. They are examples, not components.

- Website: Home · Shop: choose a pack · Checkout and Done
- Lifestyle: My Health · My Story · My Team · sheets (plan, settings, E-Points)
- Lifestyle landing: free card · sign-up flow (sign up, code, first step, log in)

All 79 captured parts are now covered by a component, a section or a screen.

All components, sections and screens also appear as screenshots in the Design System showcase (`GutGuard Design System/Showcase/index.html`, part "UI Library"). Refresh with `node scripts/export-obsidian-showcase.mjs` in `gutguard-ui` (see its README).
