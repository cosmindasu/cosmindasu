## Dasu

**Cosmin S. Dasu** and **Lidia E. Dasu** — two developers, twenty years of web applications.
PHP and Laravel for most of that; Next.js and TypeScript for the last several years.

Everything below is running right now. Click anything.

### Demo applications

Twelve applications, each in a different domain, each self-hosted on our own infrastructure.
They are not templates — the business logic differs because the businesses do.

| Application | What it demonstrates |
|---|---|
| [throughput.dbg.ro](https://throughput.dbg.ro) | Multi-tenant B2B CRM — tenant isolation in two layers (Eloquent scope + PostgreSQL Row-Level Security), append-only stock ledger, cancellable bulk writes, public REST API with an OpenAPI contract |
| [hotel.dbg.ro](https://hotel.dbg.ro) | Resort booking — availability, rate plans, loyalty tiers, GDPR data export and scheduled anonymisation |
| [lawyer.dbg.ro](https://lawyer.dbg.ro) | Law firm, bilingual — in-browser legal calculators, client portal, WCAG 2.2 AA with screen-reader testing |
| [dealership.dbg.ro](https://dealership.dbg.ro) | Multi-dealer car marketplace — financing, trade-in, live chat over WebSockets, Turborepo monorepo |
| [restaurant.dbg.ro](https://restaurant.dbg.ro) | Restaurant — menu, reservations, takeaway, with a React Native companion app |
| [travel.dbg.ro](https://travel.dbg.ro) | Travel agency — package search, dynamic packaging, PDF vouchers with QR codes, three payment gateways |
| [fitness.dbg.ro](https://fitness.dbg.ro) | Fitness platform — plans, live classes, coaching, NestJS back end, eleven account types |
| [mechanic.dbg.ro](https://mechanic.dbg.ro) | Car service — online booking, pricing, B2B fleet portal with separate driver and administrator roles |
| [construction.dbg.ro](https://construction.dbg.ro) | Contractor — cost estimator, portfolio, client portal with work progress statements, Web Push |
| [veterinary.dbg.ro](https://veterinary.dbg.ro) | Veterinary clinic — 24/7 triage, booking, pet records, shop |
| [doctors.dbg.ro](https://doctors.dbg.ro) | Dental clinic — treatments, published fees, online booking |
| [cleaning.dbg.ro](https://cleaning.dbg.ro) | Cleaning company — instant price quote, subscriptions, loyalty |

### Stack

**Back end** — Laravel 12 (Filament, Livewire, Inertia, Horizon, Reverb, Sanctum, Fortify),
NestJS, PHP 8.3. We still maintain CodeIgniter applications.

**Front end** — Next.js 16, React 19, TypeScript, Tailwind CSS, React Native (Expo).

**Data and infrastructure** — PostgreSQL, MySQL, Redis, Prisma, Meilisearch, Docker,
GitHub Actions, S3-compatible storage. We deploy and keep things running.

**Integrations** — Stripe, PayPal and Mollie behind one interface, with normalised webhook
events and idempotency keys. Xero, Exact Online, Partena, Mailchimp, Shippo, Resend.

### How we work

Tests rather than promises: Pest and PHPUnit, Vitest and Playwright, axe-core for
accessibility, PHPStan at the strict levels. CI runs on every push and we don't merge red.

Decisions get written down — architecture records, runbooks, the reason a number is what it
is. The next person to open the code shouldn't have to guess.

### Code

Most repositories here are private. **[throughput](https://github.com/cosmindasu/throughput)**
is public as a working sample: multi-tenancy, the OpenAPI contract and its contract tests,
the CI pipeline, and the architecture decision records.

A note for anyone reading it: the code comments and commit messages are in Romanian. The
README, the API specification and the architecture decisions are in English.

---

[dbg.ro](https://dbg.ro) · available for new work
