<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/banner-light.svg">
  <img src="assets/banner-dark.svg" alt="Neri Edri — Full-Stack Developer: automation, web systems and AI-powered solutions" width="100%">
</picture>

<br>

<a href="https://portfolio-website-psi-gray-62.vercel.app/">
  <img src="https://img.shields.io/badge/Portfolio-111827?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio">
</a>
<a href="https://www.linkedin.com/in/neri-edri-111388341">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
</a>
<a href="mailto:neriapple7@gmail.com">
  <img src="https://img.shields.io/badge/Email-C5221F?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
</a>

</div>

---

## About

I build software that comes out of real operational needs, not exercises — an order and quote
platform running for a working business, a personal-finance engine that classifies and de-duplicates
transactions, and desktop tools that collapse a multi-hour SQL Server setup into a guided wizard.

Most of my work is full-stack **Python** and **TypeScript**: an async FastAPI or Next.js backend, a
React or Qt client on top, PostgreSQL underneath, and automation wherever a person would otherwise
repeat themselves. I spend my attention on the parts users never see — layered architecture,
background workers, encryption of sensitive fields, RTL-correct interfaces — because those are what
decide whether a tool survives contact with real use.

---

## Tech Stack

<div align="center">

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI">
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
<img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React">
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js">
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
<img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" alt="Playwright">

</div>

|                        |                                                                                                        |
| :--------------------- | :----------------------------------------------------------------------------------------------------- |
| **Languages**          | Python · TypeScript · JavaScript · SQL · PowerShell · HTML / CSS                                         |
| **Backend**            | FastAPI · SQLAlchemy 2.0 (async) · Alembic · Celery · Pandas · Next.js Route Handlers · Prisma           |
| **Frontend**           | React · Next.js · Tailwind CSS · Vite · TanStack Query · Zustand · React Hook Form · Zod · Recharts      |
| **Desktop**            | PySide6 / Qt · Tkinter · PyInstaller                                                                     |
| **Data**               | PostgreSQL · SQL Server · SQLite · Redis                                                                 |
| **Automation & AI**    | Playwright · AI-assisted classification · Telegram Bot API · WMI · Windows Registry                      |
| **Infra & DevOps**     | Docker · Docker Compose · Nginx · Vercel · Upstash Redis · Blob storage                                  |
| **Security**           | JWT + refresh tokens · bcrypt · AES-256-GCM field encryption · Rate limiting · Input sanitization         |

---

## Featured Projects

<table>
<tr>

<td width="50%" valign="top">

<h3>SQL Server Config Generator</h3>

<img src="https://img.shields.io/badge/open%20source-238636?style=flat-square" alt="Open source">
<img src="https://img.shields.io/badge/live-1f6feb?style=flat-square" alt="Live">

<p><b>A browser tool that writes SQL Server answer files for you.</b></p>

<p><b>Problem</b> — an unattended SQL Server install needs a hand-written <code>ConfigurationFile.ini</code>, and a single wrong key means rebuilding the machine.</p>

<p><b>Built</b> — a 12-step wizard that renders the <code>.ini</code>, the <code>setup.exe</code> command and a PowerShell script live as you type, with instance-name validation, an SA-password strength meter, ZIP export, share links that encode the config in the URL, an offline-capable PWA shell, full keyboard + ARIA support, and a 28-assertion in-browser test suite. Runs entirely client-side — nothing reaches a server, and the SA password is never persisted or placed in a share link.</p>

<p><code>JavaScript</code> <code>HTML</code> <code>CSS</code> <code>PWA</code> <code>Service Worker</code></p>

<p>
<a href="https://github.com/neriedri/Generate-SQL-Server-Configuration_ini"><b>Code</b></a> ·
<a href="https://generate-sql-server-configuration-i.vercel.app/"><b>Live demo</b></a>
</p>

</td>

<td width="50%" valign="top">

<h3>FinCoreAI</h3>

<img src="https://img.shields.io/badge/private-6e7681?style=flat-square" alt="Private">
<img src="https://img.shields.io/badge/in%20development-d29922?style=flat-square" alt="In development">

<p><b>A personal finance and pension intelligence system with three surfaces.</b></p>

<p><b>Problem</b> — personal financial and pension data arrives as inconsistent statements that nobody wants to reconcile by hand.</p>

<p><b>Built</b> — a layered architecture (FastAPI REST layer → service layer → SQLAlchemy data layer) serving two clients from one core: a PySide6 desktop app and a React/TypeScript web client. An intelligence engine handles rule-based plus AI-assisted transaction classification, duplicate detection and inter-account transfer normalization, alongside CSV/Excel import via Pandas and a KPI dashboard. Authentication uses bcrypt-hashed credentials, and sensitive fields are encrypted with AES-256-GCM. The interface is RTL-first.</p>

<p><code>Python</code> <code>FastAPI</code> <code>SQLAlchemy</code> <code>PySide6</code> <code>React</code> <code>TypeScript</code></p>

<p><sub>Closed source — described at a high level.</sub></p>

</td>

</tr>
<tr>

<td width="50%" valign="top">

<h3>ZFB Order Center</h3>

<img src="https://img.shields.io/badge/private-6e7681?style=flat-square" alt="Private">
<img src="https://img.shields.io/badge/live-1f6feb?style=flat-square" alt="Live">

<p><b>Orders and quotes for a real catering business, end to end.</b></p>

<p><b>Problem</b> — a working business tracking orders and issuing price quotes by hand, with no single source of truth.</p>

<p><b>Built</b> — an async FastAPI backend over PostgreSQL (SQLAlchemy 2.0 async + asyncpg, Alembic migrations) with JWT and refresh-token auth, request rate limiting, and Celery + Redis for background jobs and scheduling. Quotes render as Hebrew RTL PDFs and go out as transactional email. The frontend is React + TypeScript + Vite with TanStack Query, Zustand, React Hook Form + Zod and Recharts. The whole stack ships containerized behind Nginx.</p>

<p><code>Python</code> <code>FastAPI</code> <code>PostgreSQL</code> <code>Celery</code> <code>Redis</code> <code>React</code> <code>Docker</code></p>

<p><a href="https://zfborder.org"><b>Live site</b></a> · <sub>Closed source.</sub></p>

</td>

<td width="50%" valign="top">

<h3>Ardani Setup System</h3>

<img src="https://img.shields.io/badge/private-6e7681?style=flat-square" alt="Private">
<img src="https://img.shields.io/badge/completed-8957e5?style=flat-square" alt="Completed">

<p><b>A Windows desktop app that installs and configures SQL Server for you.</b></p>

<p><b>Problem</b> — standing up a SQL Server instance is a long manual checklist across the installer, the registry, services and the firewall, and every step is a chance to get it wrong.</p>

<p><b>Built</b> — a 6-page PySide6 wizard covering SQL Server 2017 through 2025: environment scanning for existing instances, SSMS and ports; Mixed Mode and TCP/IP configuration through WMI and the Windows Registry; firewall-rule and service management via PowerShell; folder and permission provisioning; and export of standalone PowerShell / Batch / Python install scripts. Long-running work runs on QThreads so the wizard stays responsive, and the app ships as a single PyInstaller executable.</p>

<p><code>Python</code> <code>PySide6</code> <code>PowerShell</code> <code>WMI</code> <code>PyInstaller</code> <code>SQL Server</code></p>

<p><sub>Closed source — described at a high level.</sub></p>

</td>

</tr>
<tr>

<td width="50%" valign="top">

<h3>Portfolio Platform</h3>

<img src="https://img.shields.io/badge/open%20source-238636?style=flat-square" alt="Open source">
<img src="https://img.shields.io/badge/live-1f6feb?style=flat-square" alt="Live">

<p><b>My portfolio, built as a product rather than a static page.</b></p>

<p><b>Built</b> — a Next.js App Router site on React and Tailwind, backed by PostgreSQL through Prisma, with a custom admin area for managing projects: JWT sessions, hashed credentials, rate-limited endpoints and image uploads. Fully bilingual English / Hebrew with real RTL support, light and dark themes, and an accessibility widget with a published accessibility statement.</p>

<p><code>Next.js</code> <code>React</code> <code>TypeScript</code> <code>Tailwind CSS</code> <code>Prisma</code> <code>PostgreSQL</code></p>

<p>
<a href="https://github.com/neriedri/Portfolio-Website"><b>Code</b></a> ·
<a href="https://portfolio-website-psi-gray-62.vercel.app/"><b>Live site</b></a>
</p>

</td>

<td width="50%" valign="top">

<h3>More</h3>

<p>Additional work — including browser-automation tooling and internal desktop utilities — is written up on my portfolio, with screenshots and full technical breakdowns.</p>

<p><a href="https://portfolio-website-psi-gray-62.vercel.app/"><b>Browse all projects →</b></a></p>

<br>

<p><sub>A large share of what I build ships as private or client-owned software, so public repository activity under-represents the volume of the work. Happy to walk through architecture and decisions in a conversation.</sub></p>

</td>

</tr>
</table>

---

## What I Build

|      |      |
| :--- | :--- |
| **Automation & internal tooling** | Turning repeatable manual work — installs, configuration, sign-up flows, reporting — into guided tools and scheduled jobs. |
| **Business systems** | Orders, quotes, document generation and dashboards for businesses that are actually running on them. |
| **AI-assisted data products** | Classification, de-duplication and normalization pipelines over messy real-world financial data. |
| **Windows desktop applications** | Qt wizards that drive the operating system itself: services, registry, firewall rules and permissions. |

---

## How I Work

- **Privacy by construction.** The SQL config tool never sends data to a server and never persists the SA password; FinCoreAI encrypts sensitive fields at rest. The safest data is the data you never hold.
- **Layers before features.** Keeping the API, service and data layers separate is the reason one FinCoreAI core can serve both a Qt desktop app and a React web client without forking logic.
- **Never block the user.** Long work belongs on a QThread or a Celery worker — an interface that freezes is a bug, not a performance detail.
- **Localization is architecture.** Hebrew RTL is designed into the layout, the components and the generated PDFs from the start, not retrofitted as a translation file.
- **Test the parts that can hurt you.** The public test suite targets share-link sanitization, password masking and validation logic first — the paths where a mistake is expensive.

---

## Contact

<div align="center">

<a href="https://portfolio-website-psi-gray-62.vercel.app/">
  <img src="https://img.shields.io/badge/Portfolio-111827?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio">
</a>
<a href="https://www.linkedin.com/in/neri-edri-111388341">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
</a>
<a href="mailto:neriapple7@gmail.com">
  <img src="https://img.shields.io/badge/Email-C5221F?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
</a>

<br><br>

<sub>Open to interesting problems — automation, backend systems and AI-powered products.</sub>

</div>
