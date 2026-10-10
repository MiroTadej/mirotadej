# Miroslav Tadej

**Full Stack Software Engineer, Dublin.** I build secure-by-design web systems in TypeScript, React, Node.js and PostgreSQL, and run them on AWS. I also work in C# and .NET.

- **Software engineering:** full stack TypeScript, React, Node.js, PostgreSQL, AWS and C#/.NET, with security designed in from the first commit.
- **Technical project and delivery:** PRINCE2 and MSP (Foundation) certified, with seven years of account and delivery management behind hands-on software delivery.

**🟢 Open to software engineering and technical delivery roles in Ireland** — permanent, contract or fixed-term; Dublin preferred.

**Two systems live on AWS:** [veritydigital.ie](https://veritydigital.ie) (public) and Verity Tender Radar (authenticated, no public sign-up, so there is no demo to click; it ingests the live EU TED API only). Both deploy through GitHub Actions with keyless OIDC.

Verity Digital is my sole-trader business. No client engagements have been delivered to date.

---

## Featured projects

| Project | Status | In one line |
| --- | --- | --- |
| [**Verity Tender Radar**](https://veritydigital.ie/case-studies/tender-radar) | Live | Live EU public-procurement radar on AWS: ingests TED notices, scores them with recorded reasons and tells a small team whether it qualifies to bid. |
| [**Verity Digital**](https://veritydigital.ie/case-studies/consultancy-platform) | Live | Live business platform on AWS: public site, client portal and admin back office covering enquiries, quotes, engagements, time, VAT-aware invoicing and Stripe. |
| [**GrandStay.NET**](https://veritydigital.ie/case-studies/grandstay-dotnet) | Built, not publicly hosted | A C# port of a hotel booking platform, proven against the original React client run unmodified, with exactly one of up to 1,000 competing bookings accepted and the rest refused cleanly. |
| [**Shopora**](https://veritydigital.ie/case-studies/ecommerce-engine) | Built, not publicly hosted | Amazon-style commerce engine: one Express and Prisma API shared by a React web app and an Expo Android app through a single package of Zod contracts. |
| [**Grand Stay (PERN)**](https://veritydigital.ie/case-studies/hotel-booking-platform) | Built, not publicly hosted | Commission-free direct-booking system for independent hotels, with double bookings prevented by the database itself. |
| **TS Academy** | Built · runs locally by design | TypeScript learning platform with an in-browser Type Explorer that runs the real TypeScript compiler to show inferred types and narrowing. |
| [**JS Academy**](https://veritydigital.ie/case-studies/js-academy) | Built · runs locally by design | JavaScript learning platform built around a custom step-through visualiser showing the call stack, closures, heap and a complexity meter. |

<table>
<tr><td width="50%" valign="top"><a href="https://veritydigital.ie/case-studies/tender-radar"><img src="https://raw.githubusercontent.com/MiroTadej/mirotadej/main/screenshots/tender-radar.webp" alt="Verity Tender Radar: scored procurement notices, each with the reason it surfaced" width="100%"></a><br><sub><b>Verity Tender Radar · live</b></sub></td><td width="50%" valign="top"><a href="https://veritydigital.ie/case-studies/consultancy-platform"><img src="https://raw.githubusercontent.com/MiroTadej/mirotadej/main/screenshots/verity-digital.webp" alt="Verity Digital: the live business platform home page" width="100%"></a><br><sub><b>Verity Digital · live</b></sub></td></tr>
<tr><td width="50%" valign="top"><a href="https://veritydigital.ie/case-studies/grandstay-dotnet"><img src="https://raw.githubusercontent.com/MiroTadej/mirotadej/main/screenshots/grandstay-dotnet.webp" alt="GrandStay.NET: the admin overview, served by the .NET API to the original React client" width="100%"></a><br><sub><b>GrandStay.NET · C# port</b></sub></td><td width="50%" valign="top"><a href="https://veritydigital.ie/case-studies/hotel-booking-platform"><img src="https://raw.githubusercontent.com/MiroTadej/mirotadej/main/screenshots/grand-stay-pern.webp" alt="Grand Stay (PERN): the admin occupancy board with room grid and room detail" width="100%"></a><br><sub><b>Grand Stay (PERN) · occupancy board</b></sub></td></tr>
<tr><td width="50%" valign="top"><img src="https://raw.githubusercontent.com/MiroTadej/mirotadej/main/screenshots/ts-academy.webp" alt="TS Academy: the Type Explorer showing narrowing, read from the real TypeScript compiler" width="100%"><br><sub><b>TS Academy · Type Explorer</b></sub></td><td width="50%"></td></tr>
</table>

---

## Stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat&logo=dotnet&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat&logo=prisma&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat&logo=playwright&logoColor=white)

**Security:** JWT in httpOnly cookies with refresh rotation, double-gated RBAC, TOTP two-factor, parameterised SQL, validated input, authorised self-run penetration testing, GDPR-aware data handling.
**Testing:** Vitest, Jest, xUnit, Testcontainers, Playwright, axe-core, mutation testing.
**AI:** Anthropic API behind provider abstractions, with human review of every extracted field.

---

## Why the code is private

The application repositories are proprietary products, so they are private. They are available on request, and each has a case-study page at [veritydigital.ie](https://veritydigital.ie). The public, readable sample is [**booking-concurrency**](https://github.com/MiroTadej/booking-concurrency): never sell the same room twice, using a PostgreSQL EXCLUDE constraint and the concurrency tests that prove it.

---

## Education and certifications

- Postgraduate Diploma in Cybersecurity, National College of Ireland (NFQ Level 9), 2026
- Higher Diploma in Science in Computing (Web Development), National College of Ireland (NFQ Level 8), 2024
- Master of Public Administration, University of Pretoria: coursework completed, research component outstanding
- BCom (Hons) Business Management, University of South Africa
- PRINCE2 Foundation and Managing Successful Programmes (MSP) Foundation (APMG)

---

## Contact

- Web: [veritydigital.ie](https://veritydigital.ie)
- LinkedIn: [linkedin.com/in/miroslavtadej](https://www.linkedin.com/in/miroslavtadej)
- Email: [mirotadej@gmail.com](mailto:mirotadej@gmail.com)

Full working rights in Ireland, no sponsorship required.
