# Miroslav Tadej

### Full Stack Software Engineer · React · Node.js · PostgreSQL · AWS · Dublin, Ireland

I build secure full-stack web applications on the PERN stack (PostgreSQL · Express · React · Node.js)
and ship them to production — with security designed in from the first commit, not bolted on after.
**Two systems now run live on AWS**: my consultancy platform at
[veritydigital.ie](https://veritydigital.ie), and Verity Tender Radar at `radar.veritydigital.ie`
(authenticated, no public sign-up). Both deploy through GitHub Actions CI/CD pipelines I built end to
end, authenticating to AWS with keyless OIDC. I also work in **C# and .NET** — I've ported one of these
platforms to .NET 10 on ASP.NET Core and EF Core, and proved the port by running its original React
client against the new API unmodified. I came to software engineering from a prior career in sales
management and training, and I pair hands-on building with a postgraduate cybersecurity background.

**🟢 Open to Full Stack / Software Engineer roles in Ireland.**

---

## 🛠️ Tech Stack

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat&logo=dotnet&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat&logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat&logo=expo&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat&logo=prisma&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI%2FCD-2088FF?style=flat&logo=githubactions&logoColor=white)

**Focus areas:** secure-by-design architecture · OWASP-aware practices · JWT authentication ·
role-based access control · refresh-token rotation · parameterised SQL · concurrency correctness
enforced at the database · GDPR compliance (ROPA, DPIA, Art. 28) · keyless OIDC deploys · production
monitoring and alerting · WCAG 2.2 AA accessibility.

---

## 🚀 Featured Projects

| Project | Status | Stack | What it proves |
| --- | --- | --- | --- |
| **[Verity Digital](https://veritydigital.ie/case-studies/consultancy-platform)** | 🟢 **Live** | PERN · AWS · Docker | Secure delivery from commit to production infrastructure |
| **[Tender Radar](https://veritydigital.ie/case-studies/tender-radar)** | 🟢 **Live** | PERN · TypeScript · AWS · AI | Measured engineering: load, security and accessibility passes |
| **[JS Academy](https://veritydigital.ie/case-studies/js-academy)** | Built | PERN · TypeScript · Acorn | Interpreter design and safely running untrusted code |
| **[Shopora Commerce](https://veritydigital.ie/case-studies/ecommerce-engine)** | Built | Monorepo · Prisma · Expo | One API, two clients, no contract drift |
| **[Grand Stay Hotel](https://veritydigital.ie/case-studies/hotel-booking-platform)** | Built | PERN · raw SQL | Correctness under concurrency, enforced by the database |
| **GrandStay.NET** | Built | C# · .NET 10 · EF Core | The same guarantees, rebuilt on a second stack and proved |

### 🔐 [Verity Digital — Consultancy Platform](https://veritydigital.ie) · **Live**
A production PERN platform combining a public marketing site, an authenticated client portal, and an
admin back-office — deployed to AWS via a keyless, gated CI/CD pipeline (Elastic Beanstalk, RDS, S3,
CloudFront, ECR, CloudWatch, IAM, ACM). *Demonstrates secure-by-design delivery from commit to live
infrastructure: httpOnly-cookie JWT with refresh-token rotation, TOTP two-factor auth, RBAC, Stripe,
Docker, and GitHub OIDC.* 59 API integration suites and 472 unit tests gate every deploy, across 50
forward-only SQL migrations. The whole repository is **strict TypeScript** across three separately
type-checked surfaces at zero errors, with every request body derived from the Zod schema that
validates it rather than Express's `any`.

*Recent work:* a **GDPR and Irish/EU compliance pass** — ROPA, DPIA, an Article 28 processor agreement
as a signable document, a data-export button and a legal-hold runbook, plus retention crons that
anonymise audit-log IPs and hard-delete stale leads. A **/trust page** answering the security
questionnaire public buyers actually send (data location, encryption, access control, tested restores,
monitoring) with every claim either evidenced or explicitly marked outstanding — the partial restore
drill and absent penetration test are stated as gaps rather than glossed. Production **alerting and
CloudWatch monitoring**, so a failure is not discovered by a client; a **Content-Security-Policy** on
production HTML; **CloudFront origin verification**; and an accessibility fix where ten public pages
had no `h1` at all.
**[Read the case study →](https://veritydigital.ie/case-studies/consultancy-platform)**

### 🧠 JS Academy — JavaScript learning platform · *Built · not yet deployed*
A learning platform built around a custom **generator-based execution visualiser** (call stack,
scopes/closures, heap, and a data-structures view with a live complexity meter) on the Acorn parser,
plus a tiered curriculum and an AI-powered interview coach. *Demonstrates language tooling, interpreter
design, and sandboxed code execution — including a critical sandbox escape I found by attacking my own
grader, then fixed and regression-tested.*
**[Read the case study →](https://veritydigital.ie/case-studies/js-academy)**

### 🛒 E-commerce Platform — web + mobile + shared core
An Amazon-style commerce engine in an npm-workspaces monorepo: one Express + Prisma API behind a React
web store and an Expo/React Native app, with a shared Zod-validation and integer-cents money package so
the clients can't drift from the API. *Demonstrates a transactional, oversell-safe checkout, idempotent
Stripe webhooks, and refresh-token families with reuse detection.* Roughly **580 tests** across four
workspaces, the API suite running against a real PostgreSQL database because transactions and races
don't show up against a mock.

*Recent work:* a **strict TypeScript migration** of the shared, API and web workspaces, gated by
`tsc --noEmit` in CI. The migration is the argument for itself — it surfaced an API **leaking password
hashes in admin responses** and a pickup-checkout path the API rejected against its own seeded data,
neither of which the JavaScript build had complained about. Also a dependency pass clearing every high
advisory, including two `react-router` CVEs.
**[Read the case study →](https://veritydigital.ie/case-studies/ecommerce-engine)**

### 🏨 Hotel Management & Booking Platform · *Built · not yet deployed*
A commission-free direct-booking and hotel-operations platform built on raw parameterised SQL.
*Demonstrates database-level concurrency safety — a PostgreSQL `EXCLUDE` constraint makes overlapping
bookings physically impossible — plus multi-property RBAC and idempotent Stripe refunds.*
**[Read the case study →](https://veritydigital.ie/case-studies/hotel-booking-platform)**

### 🟣 GrandStay.NET — the hotel platform, rebuilt in C#/.NET · *Built · not yet deployed*
A full port of the platform above to **C# and .NET 10** (ASP.NET Core, EF Core, PostgreSQL 18),
delivered in seven phases across a five-project layered architecture — Domain → Application →
Infrastructure → PostgreSQL provider → API. *Demonstrates that the engineering transfers across stacks,
and that layering can be enforced rather than merely intended.*

**The layering is not honour-system.** Architecture tests assert the reference graph and fail CI on
violation: the Domain project has no dependencies at all, and Npgsql is forbidden outside the provider
project — because SQL Server is a planned second target and `EXCLUDE USING gist` has no equivalent
there, so the booking guarantee sits behind an `IBookingConflictGuard` port (ADR-0001).

**The port was proved, not asserted.** The original React client was retained and run **unmodified**
against the new API — that is the proof the contract is faithful, and it's banked at the tag
`parity-proof-v1`. A repeatable route-level diff then found **thirteen missing endpoints**, plus a
fourteenth the diff itself had missed because it lived outside the directory being scanned. *A diff is
only as complete as the surface it scans* — the method is the lesson, not the route.

*Verified rather than asserted:* the double-booking guarantee holds at **N = 2, 10 and 50** concurrent
bookings and **under load at N = 200**, losers receiving a clean typed **409, never a 500**, with the
absence of overlap proved by independent SQL. **Over 1,100 tests** — domain, application, architecture
and integration — with integration tests against **real PostgreSQL 18 containers** (Testcontainers) in
CI. And every guard was **checked by removing it and confirming the tests fail** — the advisory lock,
CSRF middleware, per-request session validation, logout's session revocation. *A guard that has never
been observed failing is an assumption, not a guarantee.*

The assurance work is written down and deliberately self-critical — a verification report checked
against the live database, a security-hardening review, a **penetration test** (28 attacks, 71
confirmed-safe checks each recorded with the predicate that makes it safe), **mutation testing**, a
committed **OpenAPI spec with a CI drift gate**, a performance report, and a **WCAG 2.2 AA** audit
enforced by CI across 29 checks over 13 routes. Each records what was *not* checked as well as what was.
Thirteen ADRs cover the decisions.

*Two findings worth the detour:* load testing exhausted PostgreSQL's connection limit outright
(`FATAL: sorry, too many clients already`) because Npgsql's default pool of 100 met a `max_connections`
of 100 — now bounded at 40, answering **`503` with `Retry-After`** rather than a `500`, since
exhaustion is a capacity signal that clears by itself. And converting the retained client to **strict
TypeScript** surfaced defects that had been failing *silently*: a checkout that could never complete,
three admin pages rendering nothing but the error boundary, a property switcher that had never worked,
and five staff controls posting fields no command declared — discarded by the model binder without an
error.

### 📡 Verity Tender Radar — Irish public-procurement radar · **Live**
Ingests EU and Irish procurement notices from the live TED API, scores each against a capability
profile, and surfaces the ones worth bidding for — every one explaining in plain sentences why it
surfaced. Tracks the qualification documents a bid needs, and drafts tender requirements with AI that a
person confirms against the source quote. *The decision I'd point at: **eTenders is never scraped.** Its
terms prohibit it, so those notices are entered by hand instead — materially more work, and the only
version worth running. Reading the terms of service is part of the engineering.*

**Live at `radar.veritydigital.ie`** — authenticated, no public sign-up, so it is not a clickable demo;
happy to walk through it. It runs as **two Elastic Beanstalk environments** — an API and a separate
scheduled ingestion worker — on commit-tagged ECR images against a private, encrypted RDS instance,
with secrets in SSM as SecureString, S3 archival of every raw payload before parsing, a dead-letter
queue with replay, and a GitHub OIDC deploy role scoped so it cannot reach the sibling app's resources.
The scheduled worker is *why* it moved to AWS: `croner` only fires while the process is alive, so a
laptop shut at 18:00 never runs its 06:00 job.

*Verified rather than asserted:* **1,898 tests** (104 files, 84.71% statement coverage) plus a
**138-test Playwright suite** driving a real browser, a load pass at **100× a realistic corpus** with
zero errors at 128 concurrent users, an adversarial security assessment, and a **WCAG 2.2 AA** pass —
every finding remediated. The AI extraction eval harness caught a **1000× money-parsing defect**
(€6.5m read as €6.5bn) that was intermittent enough to survive a spot check.

*Recent work:* an **admin automation-scheduling panel** with its own save-blocker and wheel-adjustable
window times; **CloudWatch log streaming**, which turned out never to have been enabled — every
`logger.error` the API and worker had ever written was going to a container filesystem and being
discarded on the next deploy; an **uptime check on a health path that actually resolves**, after
finding that CloudFront's SPA rewrite was turning a missing `/health/ready` into a `200` and would have
reported "up" forever; and a corrected RDS storage alarm that treated missing data as *missing* rather
than *breaching*, so a stopped instance would have gone quiet instead of alarming.

![Verity Tender Radar](https://raw.githubusercontent.com/MiroTadej/mirotadej/main/screenshots/tender-radar.png)

**[Read the case study →](https://veritydigital.ie/case-studies/tender-radar)**

> **Why you can't see the code here.** These are proprietary products, not open-source samples, so the
> application repositories are private. Each case study above walks through the architecture, the
> trade-offs and the code that matters — and I'm happy to grant repository access or walk through any
> of it live on request.
>
> **Status, stated honestly:** two systems are deployed — Verity Digital at
> [veritydigital.ie](https://veritydigital.ie), which is public, and Verity Tender Radar at
> `radar.veritydigital.ie`, which is authenticated with no public sign-up, so there is nothing a
> visitor can click into. The other four — JS Academy, the commerce engine, and the hotel platform in
> both its PERN and .NET forms — are feature-complete and tested, but not yet publicly hosted.

---

## 🎓 Education

- **Postgraduate Diploma in Science in Cybersecurity** — NFQ Level 9, National College of Ireland, Dublin (2026)
- **Higher Diploma in Science in Computing (Web Development)** — NFQ Level 8, National College of Ireland, Dublin (2024)
- **Bachelor of Commerce (Hons) in Business Management** — University of South Africa (2015)
- **Bachelor of Commerce in Management** — University of South Africa (2012)

## 📜 Certifications

- **Computer Science and Python Programming** — Massachusetts Institute of Technology (MITx)
- **PRINCE2** — APMG
- **Managing Successful Programmes (MSP)** — APMG
- **Project Management** — University of South Africa
- **Project Management** — University of the Witwatersrand
- **Occupationally Directed Education, Training & Development Practices** — ETDP SETA

---

## 📫 Contact

- **Portfolio:** [veritydigital.ie](https://veritydigital.ie)
- **LinkedIn:** [linkedin.com/in/miroslavtadej](https://www.linkedin.com/in/miroslavtadej)
- **Email:** mirotadej@gmail.com
