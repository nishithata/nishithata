![Banner](https://capsule-render.vercel.app/api?type=waving&color=0:2563eb,100:7c3aed&height=160&section=header&text=Full-Stack%20Developer%20%7C%20Ruby%20on%20Rails&fontSize=28&fontColor=ffffff&fontAlignY=55)

# Hi, I'm Nishitha Thatha Anil

**Full-Stack Developer · Ruby on Rails · JavaScript · PostgreSQL**

I build **RESTful APIs with Ruby on Rails, ActiveRecord, and PostgreSQL**, secured with JWT authentication and role-based authorization, and backed by automated tests that run in GitHub Actions CI. I also build full-stack **JavaScript / TypeScript** applications with React, Node.js, and AWS.

Before that, I was a **Software Developer at Tata Consultancy Services**, delivering Java/J2EE and JavaScript enterprise applications through the full SDLC.

I'm actively looking for **Ruby on Rails, backend, and full-stack engineering roles**.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/nishitha-anil)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:nishitha.1190@gmail.com)
[![Resume](https://img.shields.io/badge/Resume-1a1a1a?style=flat&logo=googledocs&logoColor=white)](https://nishithata.github.io/resume/)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat&logo=vercel&logoColor=white)](https://nishitha-studio.vercel.app)
[![Rails API Demo](https://img.shields.io/badge/Rails_API_Demo-D30001?style=flat&logo=rubyonrails&logoColor=white)](https://community-reservations-api-web.vercel.app)
[![QA Automation](https://img.shields.io/badge/QA_Automation-2EAD33?style=flat&logo=playwright&logoColor=white)](https://github.com/nishithata/community-reservations-qa)

---

## What I Do

- **Backend APIs:** Rails and Express REST APIs with clean MVC structure, validations, and consistent JSON error responses
- **Databases:** PostgreSQL schema design, migrations, indexes, constraints, and query optimization
- **Security:** JWT authentication, role-based authorization, input validation, and rate limiting
- **QA & Test Automation:** Playwright API, UI, cross-browser, and accessibility tests; test plans, test case design, exploratory testing, and defect reports
- **Quality & Delivery:** Minitest and Vitest test suites, GitHub Actions CI/CD, and cloud deployment
- **Frontend & Analytics:** React dashboards and data visualization

---

## Featured Projects

### Community Resource Reservation API · Community of Guardians

<a href="https://community-reservations-api-web.vercel.app"><img src="https://raw.githubusercontent.com/nishithata/community-reservations-api/main/web/og-image.png" alt="Community Reservations: a booking calendar showing a confirmed slot and a rejected overlapping request (409 Conflict)" width="640"></a>

🔗 **[Live demo](https://community-reservations-api-web.vercel.app)** · **[Code](https://github.com/nishithata/community-reservations-api)** · **[API docs](https://github.com/nishithata/community-reservations-api/blob/main/docs/API.md)** · **[Architecture](https://github.com/nishithata/community-reservations-api/blob/main/docs/ARCHITECTURE.md)**

A Ruby on Rails REST API for booking shared community resources (rooms, equipment, garden plots, vehicles), built so two people can never book the same slot, even when they click **Reserve** at the same moment. Try it with `demo@example.com` / `demo-password-123`.

**Stack:** Ruby · Ruby on Rails · PostgreSQL · ActiveRecord · JWT · Pagy · Minitest · GitHub Actions · Docker · Render · Neon · Vercel

- Designed and built a RESTful Rails API following **MVC** conventions
- Modeled the domain with **ActiveRecord associations, validations, migrations, and SQL indexes**, plus a health-check endpoint
- Built reservation validation that **rejects invalid time ranges and conflicting bookings**, returning structured JSON errors with the correct REST status codes
- Secured endpoints with **JWT authentication and role-based authorization** (401 / 403 responses)
- Added **Pagy pagination** to list endpoints
- Prevented **double bookings under concurrent requests** with a PostgreSQL exclusion constraint, returning **409 Conflict**
- Wrote **87 Minitest model and API request tests** for CRUD, reservation creation and cancellation, filtering, and validation errors, run by **GitHub Actions** on every change
- Deployed the API to **Render** with serverless PostgreSQL on **Neon** and a JavaScript demo client on **Vercel**, with a production-mode end-to-end job in CI

### QA & Test Automation for the Reservation System · Community of Guardians

🔗 **[Code](https://github.com/nishithata/community-reservations-qa)** · **[Test plan](https://github.com/nishithata/community-reservations-qa/blob/main/docs/TEST_PLAN.md)** · **[Bug reports](https://github.com/nishithata/community-reservations-qa/blob/main/docs/BUG_REPORTS.md)** · **[Test report](https://github.com/nishithata/community-reservations-qa/blob/main/docs/TEST_REPORT.md)**

An end-to-end quality engineering project that tests the live reservation system above, from the test plan down to automated checks running nightly in CI.

**Stack:** Playwright · TypeScript · axe-core · k6 · GitHub Actions

- Built **94 automated tests** covering the API, the UI on **Chromium, Firefox, WebKit, and mobile**, and **accessibility (WCAG 2.1 AA)**
- Wrote a **test plan** and a **test case catalog traced to 12 requirements**, using equivalence partitioning, boundary values, decision tables, and state transitions
- Found and documented **10 defects**; a **mobile layout bug that broke booking on phones** and **color-contrast failures** were fixed and re-verified by the suite
- Covered **security** (forged tokens, authorization, XSS) and **concurrency** (simultaneous bookings), plus **k6 load tests** with latency thresholds

### SDG Impact Dashboard · Community of Guardians

A full-stack platform where users track and share real-world contributions to the **UN Sustainable Development Goals**, with challenges, social features, gamification, and a 24-view analytics suite.

**Stack:** React 19 · TypeScript · Node.js · Express · Prisma · PostgreSQL · Vitest · GitHub Actions · AWS

- Engineered **70+ REST API endpoints** for authentication, social interactions, challenges, and analytics
- Implemented **JWT authentication with rotating refresh tokens**, bcrypt password hashing, Google OAuth, and role-based access for users, experts, and admins
- Designed the PostgreSQL schema with **GIN full-text search, partial, and covering indexes**, CHECK constraints, triggers, and materialized views
- Optimized critical queries from **6 seconds to under 100 ms** by rewriting correlated subqueries as CTEs with targeted indexing
- Built **24 analytics dashboards**, including cohort retention, churn prediction, geographic heat maps, and network graphs
- Wrote **40 Vitest test files** and a GitHub Actions pipeline that builds and deploys to **AWS EC2 and RDS**

### Nishitha Studio

🔗 **Live:** https://nishitha-studio.vercel.app

A React + TypeScript application featuring a component library, client-side image tools, and production analytics.

**Stack:** React 18 · TypeScript · Vite · Tailwind CSS · Radix UI · Framer Motion

- Built **30+ accessible Radix UI components** forming a reusable UI system
- Implemented **client-side image processing with HTML5 Canvas**, including HEIC to JPEG conversion and QR code generation
- Added smooth animations with **Framer Motion** and a command palette with **cmdk**
- Monitored production with **Google Analytics 4, Microsoft Clarity, and Vercel Analytics**

---

## Tech Stack

**Languages**

![Ruby](https://img.shields.io/badge/Ruby-CC342D?style=flat&logo=ruby&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

**Backend**

![Ruby on Rails](https://img.shields.io/badge/Ruby_on_Rails-D30001?style=flat&logo=rubyonrails&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat&logo=express&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat&logo=prisma&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat&logo=microsoftsqlserver&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat&logo=chartdotjs&logoColor=white)
![Radix UI](https://img.shields.io/badge/Radix_UI-161618?style=flat&logo=radixui&logoColor=white)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=flat&logo=framer&logoColor=white)

**Testing**

![Minitest](https://img.shields.io/badge/Minitest-CC342D?style=flat&logo=ruby&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat&logo=vitest&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat&logo=playwright&logoColor=white)
![k6](https://img.shields.io/badge/k6-7D64FF?style=flat&logo=k6&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white)

**DevOps & Cloud**

![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=github-actions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat&logo=render&logoColor=white)
![Neon](https://img.shields.io/badge/Neon-00E599?style=flat&logo=postgresql&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonaws&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)

**Data & AI**

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![OpenAI SDK](https://img.shields.io/badge/OpenAI_SDK-412991?style=flat&logo=openai&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-316192?style=flat&logo=postgresql&logoColor=white)
![GitHub Copilot](https://img.shields.io/badge/GitHub_Copilot-000000?style=flat&logo=github&logoColor=white)

---

## Experience

**Software Developer · Tata Consultancy Services** (Bangalore, India · 2012 - 2016)

- Built the **NGP (Next Generation Portal)** for Tata Communications, unifying five legacy customer portals into a single IBM WebSphere interface for ticketing, billing, and service management
- Developed the UI in JavaScript, HTML, and CSS, connected to backend web services and MySQL through a J2EE service layer
- Led the full SDLC in an Agile/Scrum team, mentored junior developers, conducted code reviews, and provided production support

---

## Currently

- 🛠️ Building **Ruby on Rails** APIs with PostgreSQL, JWT auth, and automated tests
- 📊 Completing the **Data Analysis program at Calbright College** (California)
- 🌱 Exploring scalable API design, background jobs, and containerized deployment

---

![Profile Views](https://komarev.com/ghpvc/?username=nishithata&color=blue&style=flat)
