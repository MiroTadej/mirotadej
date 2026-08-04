# Miroslav Tadej

### Full Stack Software Engineer · React · Node.js · PostgreSQL · AWS · Dublin, Ireland

I build secure full-stack web applications on the PERN stack (PostgreSQL · Express · React · Node.js)
and ship them to production — with security designed in from the first commit, not bolted on after.
My consultancy platform is **live at [veritydigital.ie](https://veritydigital.ie)**, deployed to AWS
through a GitHub Actions CI/CD pipeline I built end to end. I came to software engineering from a prior
career in sales management and training, and I pair hands-on building with a postgraduate cybersecurity
background.

**🟢 Open to Full Stack / Software Engineer roles in Ireland.**

---

## 🛠️ Tech Stack

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
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
role-based access control · refresh-token rotation · parameterised SQL · GDPR-aware builds.

---

## 🚀 Featured Projects

| Project | Status | Stack | What it proves |
| --- | --- | --- | --- |
| **[Verity Digital](https://veritydigital.ie/case-studies/consultancy-platform)** | 🟢 **Live** | PERN · AWS · Docker | Secure delivery from commit to production infrastructure |
| **[JS Academy](https://veritydigital.ie/case-studies/js-academy)** | Built | PERN · TypeScript · Acorn | Interpreter design and safely running untrusted code |
| **[Shopora Commerce](https://veritydigital.ie/case-studies/ecommerce-engine)** | Built | Monorepo · Prisma · Expo | One API, two clients, no contract drift |
| **[Grand Stay Hotel](https://veritydigital.ie/case-studies/hotel-booking-platform)** | Built | PERN · raw SQL | Correctness under concurrency, enforced by the database |
| **[Tender Radar](https://veritydigital.ie/case-studies/tender-radar)** | Built | PERN · TypeScript · AI | Reading the rules before writing the scraper |

### 🔐 [Verity Digital — Consultancy Platform](https://veritydigital.ie) · **Live**
A production PERN platform combining a public marketing site, an authenticated client portal, and an
admin back-office — deployed to AWS via a keyless, gated CI/CD pipeline (Elastic Beanstalk, RDS, S3,
CloudFront, ECR, CloudWatch, IAM, ACM). *Demonstrates secure-by-design delivery from commit to live
infrastructure: httpOnly-cookie JWT with refresh-token rotation, TOTP two-factor auth, RBAC, Stripe,
Docker, and GitHub OIDC.*
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
Stripe webhooks, and refresh-token families with reuse detection.*
**[Read the case study →](https://veritydigital.ie/case-studies/ecommerce-engine)**

### 🏨 Hotel Management & Booking Platform · *Built · not yet deployed*
A commission-free direct-booking and hotel-operations platform built on raw parameterised SQL.
*Demonstrates database-level concurrency safety — a PostgreSQL `EXCLUDE` constraint makes overlapping
bookings physically impossible — plus multi-property RBAC and idempotent Stripe refunds.*
**[Read the case study →](https://veritydigital.ie/case-studies/hotel-booking-platform)**

### 📡 Verity Tender Radar — Irish public-procurement radar · *Built · internal tool*
Ingests EU procurement notices from the TED API, scores each against a capability profile, and surfaces
the ones worth bidding for — every one explaining in plain sentences why it surfaced. Tracks the
qualification documents a bid needs, and drafts tender requirements with AI that a person confirms
against the source quote. *The decision I'd point at: **eTenders is never scraped.** Its terms prohibit
it, so those notices are entered by hand instead — materially more work, and the only version worth
running. Reading the terms of service is part of the engineering.*

![Verity Tender Radar](https://raw.githubusercontent.com/MiroTadej/mirotadej/main/screenshots/tender-radar.png)

**[Read the case study →](https://veritydigital.ie/case-studies/tender-radar)**

> **Why you can't see the code here.** These are proprietary products, not open-source samples, so the
> application repositories are private. Each case study above walks through the architecture, the
> trade-offs and the code that matters — and I'm happy to grant repository access or walk through any
> of it live on request.
>
> **Status, stated honestly:** only Verity Digital is deployed at
> [veritydigital.ie](https://veritydigital.ie). The other four are feature-complete and tested, but
> not yet publicly hosted.

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
