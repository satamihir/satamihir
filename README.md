<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/header-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/header-light.svg">
  <img alt="Mihir Sata, software developer" src="./assets/header-dark.svg" width="100%">
</picture>

<p align="center">
  <a href="https://satamihir.github.io"><picture><source media="(prefers-color-scheme: dark)" srcset="./assets/btn-portfolio-dark.svg"><source media="(prefers-color-scheme: light)" srcset="./assets/btn-portfolio-light.svg"><img alt="portfolio: satamihir.github.io" src="./assets/btn-portfolio-dark.svg" height="44"></picture></a>
  <a href="https://www.linkedin.com/in/satamihir/"><picture><source media="(prefers-color-scheme: dark)" srcset="./assets/btn-linkedin-dark.svg"><source media="(prefers-color-scheme: light)" srcset="./assets/btn-linkedin-light.svg"><img alt="linkedin: /in/satamihir" src="./assets/btn-linkedin-dark.svg" height="44"></picture></a>
  <picture><source media="(prefers-color-scheme: dark)" srcset="./assets/btn-status-dark.svg"><source media="(prefers-color-scheme: light)" srcset="./assets/btn-status-light.svg"><img alt="status: open to work" src="./assets/btn-status-dark.svg" height="44"></picture>
</p>

```console
$ whoami
mihir sata · full-stack developer · kitchener, ontario · five years in

$ cat principles.txt
▸ full-stack, in both directions
  i don't hand off at the API boundary. i follow the bug.
▸ payments-grade carefulness
  an edge case isn't a ticket. it's someone's 4pm friday.
▸ llms in production, not demos
  if it doesn't ship, it doesn't count.
```

---

### `01 / trajectory`
<sub>where the five years went</sub>

<pre>
$ git log --graph --oneline career

* 2026 ─ now    <b>(HEAD -&gt; open-to-work)</b>  your team, maybe?
│
* 2024 ─ 2026   <b>LBMX</b> · software developer · london, on
│               ├─ 9 payment workflows, angular front to .net back
│               ├─ gemini over 1,000+ documents in a single pass
│               └─ sql server sleuthing on live production issues
│
* 2022 ─ 2023   <b>CONESTOGA COLLEGE</b> · pg cert, web development · gpa 3.5
│
* 2021          <b>STACKBY.COM</b> · frontend engineer
│               ├─ 8+ modules in react, redux, typescript
│               ├─ page loads 25–30% faster
│               └─ shipped a private npm ui library, used platform-wide
│
* 2020 ─ 2021   <b>NAROLA INFOTECH</b> · software engineer
│               ├─ traffic simulator (vue + node)
│               ├─ booking system + slot-conflict detection (django)
│               └─ payment gateway modules (react + tailwind)
│
* 2014 ─ 2018   (root)  <b>PARUL UNIVERSITY</b> · b.e. computer science · gpa 3.4
</pre>

<details>
<summary><code>$ git show --stat</code> &nbsp;·&nbsp; the full changelog</summary>
<br>

**LBMX** · Intermediate Software Developer · `Feb 2024 — Jun 2026` · London, ON
- Shipped full-stack features across **9 payment workflows** on an enterprise B2B payment platform:
  `Make Payments` `Payment Batches` `Received Invoices` `Invoice Reconciliation` `Statement of Account` `Pay by Statement` `Mark as Paid` `Allocate Credit` `Print Payment Options`
- Built the **Angular + TypeScript** frontend for those flows: complex UI state, form validation, and dense data tables for invoice, supplier and transaction views.
- Extended **C#/.NET** service-layer logic across **5+ modules**: request handlers, validation rules and REST integrations powering core payment operations.
- Integrated **Gemini LLM APIs** into TradeSync for AI-assisted bulk document processing, **1,000+ documents per run**.
- Wrote and tuned **SQL Server** queries to trace data discrepancies and fix live production issues mid-feature.

**Stackby.com** · Software Engineer, Frontend · `May 2021 — Dec 2021` · Gujarat, India
- Built and extended **8+ platform modules** in React, Redux and TypeScript:
  `Dashboard` `Grid View` `Kanban Board` `Calendar View` `Authentication` `Search & Filters` `Notifications` `User Management`
- Cut page-load time by **25–30%** with reusable components, render optimisation, memoisation and lazy loading.
- Published a **private npm library** of reusable UI components (forms, modals, data tables, filters, validation) adopted across the whole platform.

**Narola Infotech Solutions** · Software Engineer · `Jun 2020 — May 2021` · Gujarat, India
- **Traffic Simulator:** full-stack modules in Vue.js and Node.js, with REST APIs for simulation scenarios, vehicle movement, routes and signal timing.
- **Booking Management System:** Python + Django + MySQL backend. Designed the schema and REST APIs for scheduling, including **time-slot conflict detection** across overlapping bookings.
- **Payment gateway:** contributed React, TypeScript and TailwindCSS modules and CRUD APIs alongside senior developers.

**Education**
- **Post Graduate Certificate, Web Development** · Conestoga College, Waterloo, ON · `2022 — 2023` · GPA 3.5 / 4.0
- **B.E. Computer Science Engineering** · Gujarat Technological University (Parul University) · `2014 — 2018` · GPA 3.4 / 4.0

</details>

---

### `02 / selected work`
<sub>three things worth showing. each one is a problem, a move, and a result.</sub>

<table>
<tr><td>

#### `i.` &nbsp;Enterprise B2B payment platform
<sub><b>LBMX</b> · Angular · C#/.NET · SQL Server</sub>

> **problem** &nbsp;Suppliers and buyers reconciling invoices across nine payment paths, each with its own rules.<br>
> **move** &nbsp;&nbsp;&nbsp;&nbsp;End-to-end features across all nine workflows and the invoice, supplier and banking modules, from frontend state and validation through to .NET service logic.<br>
> **result** &nbsp;&nbsp;Core payment operations **shipped and running in production**.

</td></tr>
<tr><td>

#### `ii.` &nbsp;AI-assisted bulk document processing
<sub><b>LBMX</b> · Gemini API · TradeSync</sub>

> **problem** &nbsp;Users opening documents one at a time to pull out the same handful of fields.<br>
> **move** &nbsp;&nbsp;&nbsp;&nbsp;Integrated Gemini so a user can upload a batch and run a custom prompt across the whole set.<br>
> **result** &nbsp;&nbsp;**1,000+ documents** analysed in one pass instead of one by one.

</td></tr>
<tr><td>

#### `iii.` &nbsp;Zorro Copilot &nbsp;<img alt="in development" src="https://img.shields.io/badge/in_development-7ba5d0?style=flat-square">
<sub><b>personal project</b> · Python · FastAPI · PydanticAI · React · pgvector · OpenAI</sub>

> **problem** &nbsp;Analysts digging through 10-Ks and 10-Qs by hand to answer questions they need a citable source for.<br>
> **move** &nbsp;&nbsp;&nbsp;&nbsp;An internal AI chatbot with a FastAPI backend and a Vite + React + TypeScript frontend. Ask in plain English, get **sourced, citable answers** back.<br>
> **result** &nbsp;&nbsp;Running against a real document corpus right now.

</td></tr>
</table>

<details>
<summary><b>also built</b> · five more from the archive</summary>
<br>

**Stackby component library** &nbsp;<sub>`React` `Redux` `TypeScript` `npm`</sub><br>
Eight product modules were each re-implementing the same forms, modals, tables and filters. I extracted the shared patterns into a versioned private npm library with consistent validation and state contracts, then moved Calendar View onto Grid View's data flow so the two stopped drifting apart. The result was one UI vocabulary across the product and **25–30% faster page loads**.

**Traffic simulator** &nbsp;<sub>`Vue.js` `Node.js` `Vuetify`</sub><br>
A full-stack simulation of vehicle movement, routing and signal timing. I designed the REST APIs for scenarios and live simulation state, and built the parameter-input, traffic-flow monitoring and chart-analytics interfaces on top. I chose Vuetify over Bootstrap and tuned against Lighthouse profiles, so the UI stays responsive while the simulation runs.

**Job Board Platform** &nbsp;<sub>`Java` `SQL` `AWS Amplify`</sub><br>
A hiring marketplace that puts job listings next to company reviews and salary data, so candidates can judge an offer before they apply. The relational schema connects companies, roles, reviews and compensation, with Java services behind it and AWS Amplify for hosting.

**FoodX** &nbsp;<sub>`React` `Redux` `MySQL` `AWS`</sub><br>
A recipe platform where users build and customise their own recipes, starting from star-rated recipes and chefs. Ratings, chef profiles and user-curated recipes are modelled in MySQL, and a React + Redux client handles the customisation flow. Deployed on AWS.

**PayFX** &nbsp;<sub>`React` `Redux` `Python` `Flask`</sub><br>
A market-research platform for crypto and equities. Each asset gets a detailed view of its data and analysis to help users decide what to buy. A Python/Flask service handles market data, and a React + Redux dashboard presents it.

</details>

---

### `03 / toolkit`
<sub>what i'd want to be hired for. no percentage bars.</sub>

<p>
<img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-0e141d?style=flat-square&logo=typescript&logoColor=c2d6ea">
<img alt="Angular" src="https://img.shields.io/badge/Angular-0e141d?style=flat-square&logo=angular&logoColor=c2d6ea">
<img alt="React" src="https://img.shields.io/badge/React-0e141d?style=flat-square&logo=react&logoColor=c2d6ea">
<img alt="Vue.js" src="https://img.shields.io/badge/Vue.js-0e141d?style=flat-square&logo=vuedotjs&logoColor=c2d6ea">
<img alt="Python" src="https://img.shields.io/badge/Python-0e141d?style=flat-square&logo=python&logoColor=c2d6ea">
<img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-0e141d?style=flat-square&logo=fastapi&logoColor=c2d6ea">
<img alt="C#" src="https://img.shields.io/badge/C%23-0e141d?style=flat-square">
<img alt=".NET" src="https://img.shields.io/badge/.NET-0e141d?style=flat-square&logo=dotnet&logoColor=c2d6ea">
<img alt="Node.js" src="https://img.shields.io/badge/Node.js-0e141d?style=flat-square&logo=nodedotjs&logoColor=c2d6ea">
<img alt="SQL Server" src="https://img.shields.io/badge/SQL%20Server-0e141d?style=flat-square">
<img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-0e141d?style=flat-square&logo=postgresql&logoColor=c2d6ea">
<img alt="Docker" src="https://img.shields.io/badge/Docker-0e141d?style=flat-square&logo=docker&logoColor=c2d6ea">
</p>

<details>
<summary><code>$ ls --all ~/toolkit</code> &nbsp;·&nbsp; the full spectrum, grouped by where it sits in the stack</summary>
<br>

<table>
<tr>
<td valign="top" width="150"><b>frontend</b><br><sub>the layer users judge you by</sub></td>
<td>
<img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-0e141d?style=flat-square&logo=typescript&logoColor=c2d6ea">
<img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-0e141d?style=flat-square&logo=javascript&logoColor=c2d6ea">
<img alt="Angular" src="https://img.shields.io/badge/Angular-0e141d?style=flat-square&logo=angular&logoColor=c2d6ea">
<img alt="React" src="https://img.shields.io/badge/React-0e141d?style=flat-square&logo=react&logoColor=c2d6ea">
<img alt="Vue.js" src="https://img.shields.io/badge/Vue.js-0e141d?style=flat-square&logo=vuedotjs&logoColor=c2d6ea">
<img alt="Next.js" src="https://img.shields.io/badge/Next.js-0e141d?style=flat-square&logo=nextdotjs&logoColor=c2d6ea">
<img alt="Redux" src="https://img.shields.io/badge/Redux-0e141d?style=flat-square&logo=redux&logoColor=c2d6ea">
<img alt="Vuex" src="https://img.shields.io/badge/Vuex-0e141d?style=flat-square&logo=vuedotjs&logoColor=c2d6ea">
<img alt="HTML5" src="https://img.shields.io/badge/HTML5-0e141d?style=flat-square&logo=html5&logoColor=c2d6ea">
<img alt="SCSS" src="https://img.shields.io/badge/SCSS-0e141d?style=flat-square&logo=sass&logoColor=c2d6ea">
<img alt="CSS3" src="https://img.shields.io/badge/CSS3-0e141d?style=flat-square&logo=css&logoColor=c2d6ea">
<img alt="Tailwind" src="https://img.shields.io/badge/Tailwind-0e141d?style=flat-square&logo=tailwindcss&logoColor=c2d6ea">
<img alt="Bootstrap" src="https://img.shields.io/badge/Bootstrap-0e141d?style=flat-square&logo=bootstrap&logoColor=c2d6ea">
<img alt="jQuery" src="https://img.shields.io/badge/jQuery-0e141d?style=flat-square&logo=jquery&logoColor=c2d6ea">
</td>
</tr>
<tr>
<td valign="top" width="150"><b>backend</b><br><sub>where the rules live</sub></td>
<td>
<img alt="Python" src="https://img.shields.io/badge/Python-0e141d?style=flat-square&logo=python&logoColor=c2d6ea">
<img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-0e141d?style=flat-square&logo=fastapi&logoColor=c2d6ea">
<img alt="Django" src="https://img.shields.io/badge/Django-0e141d?style=flat-square&logo=django&logoColor=c2d6ea">
<img alt="Flask" src="https://img.shields.io/badge/Flask-0e141d?style=flat-square&logo=flask&logoColor=c2d6ea">
<img alt="C#" src="https://img.shields.io/badge/C%23-0e141d?style=flat-square">
<img alt=".NET" src="https://img.shields.io/badge/.NET-0e141d?style=flat-square&logo=dotnet&logoColor=c2d6ea">
<img alt="Node.js" src="https://img.shields.io/badge/Node.js-0e141d?style=flat-square&logo=nodedotjs&logoColor=c2d6ea">
<img alt="Express" src="https://img.shields.io/badge/Express-0e141d?style=flat-square&logo=express&logoColor=c2d6ea">
<img alt="Java" src="https://img.shields.io/badge/Java-0e141d?style=flat-square">
<img alt="C++" src="https://img.shields.io/badge/C%2B%2B-0e141d?style=flat-square&logo=cplusplus&logoColor=c2d6ea">
<img alt="C" src="https://img.shields.io/badge/C-0e141d?style=flat-square&logo=c&logoColor=c2d6ea">
<img alt="REST" src="https://img.shields.io/badge/REST-0e141d?style=flat-square">
<img alt="GraphQL" src="https://img.shields.io/badge/GraphQL-0e141d?style=flat-square&logo=graphql&logoColor=c2d6ea">
<img alt="RabbitMQ" src="https://img.shields.io/badge/RabbitMQ-0e141d?style=flat-square&logo=rabbitmq&logoColor=c2d6ea">
</td>
</tr>
<tr>
<td valign="top" width="150"><b>data</b><br><sub>where the truth lives</sub></td>
<td>
<img alt="SQL Server" src="https://img.shields.io/badge/SQL%20Server-0e141d?style=flat-square">
<img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-0e141d?style=flat-square&logo=postgresql&logoColor=c2d6ea">
<img alt="pgvector" src="https://img.shields.io/badge/pgvector-0e141d?style=flat-square">
<img alt="MySQL" src="https://img.shields.io/badge/MySQL-0e141d?style=flat-square&logo=mysql&logoColor=c2d6ea">
<img alt="MongoDB" src="https://img.shields.io/badge/MongoDB-0e141d?style=flat-square&logo=mongodb&logoColor=c2d6ea">
<img alt="Redis" src="https://img.shields.io/badge/Redis-0e141d?style=flat-square&logo=redis&logoColor=c2d6ea">
<img alt="Firebase" src="https://img.shields.io/badge/Firebase-0e141d?style=flat-square&logo=firebase&logoColor=c2d6ea">
</td>
</tr>
<tr>
<td valign="top" width="150"><b>ai & agents</b><br><sub>shipped, not demoed</sub></td>
<td>
<img alt="OpenAI" src="https://img.shields.io/badge/OpenAI-0e141d?style=flat-square">
<img alt="Gemini" src="https://img.shields.io/badge/Gemini-0e141d?style=flat-square&logo=googlegemini&logoColor=c2d6ea">
<img alt="OpenRouter" src="https://img.shields.io/badge/OpenRouter-0e141d?style=flat-square&logo=openrouter&logoColor=c2d6ea">
<img alt="PydanticAI" src="https://img.shields.io/badge/PydanticAI-0e141d?style=flat-square">
<img alt="MCP" src="https://img.shields.io/badge/MCP-0e141d?style=flat-square">
<img alt="RAG" src="https://img.shields.io/badge/RAG-0e141d?style=flat-square">
<img alt="Tool calling" src="https://img.shields.io/badge/Tool%20calling-0e141d?style=flat-square">
<img alt="Structured outputs" src="https://img.shields.io/badge/Structured%20outputs-0e141d?style=flat-square">
<img alt="Agent memory" src="https://img.shields.io/badge/Agent%20memory-0e141d?style=flat-square">
<img alt="Prompt engineering" src="https://img.shields.io/badge/Prompt%20engineering-0e141d?style=flat-square">
<img alt="Evals" src="https://img.shields.io/badge/Evals-0e141d?style=flat-square">
</td>
</tr>
<tr>
<td valign="top" width="150"><b>cloud & infra</b><br><sub>where it runs</sub></td>
<td>
<img alt="Docker" src="https://img.shields.io/badge/Docker-0e141d?style=flat-square&logo=docker&logoColor=c2d6ea">
<img alt="AWS Amplify" src="https://img.shields.io/badge/AWS%20Amplify-0e141d?style=flat-square">
<img alt="GCP" src="https://img.shields.io/badge/GCP-0e141d?style=flat-square&logo=googlecloud&logoColor=c2d6ea">
<img alt="DigitalOcean" src="https://img.shields.io/badge/DigitalOcean-0e141d?style=flat-square&logo=digitalocean&logoColor=c2d6ea">
<img alt="Vercel" src="https://img.shields.io/badge/Vercel-0e141d?style=flat-square&logo=vercel&logoColor=c2d6ea">
<img alt="Railway" src="https://img.shields.io/badge/Railway-0e141d?style=flat-square&logo=railway&logoColor=c2d6ea">
<img alt="Linux" src="https://img.shields.io/badge/Linux-0e141d?style=flat-square&logo=linux&logoColor=c2d6ea">
<img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub%20Actions-0e141d?style=flat-square&logo=githubactions&logoColor=c2d6ea">
</td>
</tr>
<tr>
<td valign="top" width="150"><b>workflow</b><br><sub>how it gets there</sub></td>
<td>
<img alt="Git" src="https://img.shields.io/badge/Git-0e141d?style=flat-square&logo=git&logoColor=c2d6ea">
<img alt="GitHub" src="https://img.shields.io/badge/GitHub-0e141d?style=flat-square&logo=github&logoColor=c2d6ea">
<img alt="SourceTree" src="https://img.shields.io/badge/SourceTree-0e141d?style=flat-square&logo=sourcetree&logoColor=c2d6ea">
<img alt="Jira" src="https://img.shields.io/badge/Jira-0e141d?style=flat-square&logo=jira&logoColor=c2d6ea">
<img alt="Rally" src="https://img.shields.io/badge/Rally-0e141d?style=flat-square">
<img alt="TFS" src="https://img.shields.io/badge/TFS-0e141d?style=flat-square">
<img alt="Figma" src="https://img.shields.io/badge/Figma-0e141d?style=flat-square&logo=figma&logoColor=c2d6ea">
<img alt="Agile" src="https://img.shields.io/badge/Agile-0e141d?style=flat-square">
<img alt="Codex" src="https://img.shields.io/badge/Codex-0e141d?style=flat-square">
</td>
</tr>
</table>

</details>

---

### `04 / reach me`
<sub>take the glasses off. let's talk.</sub>

| **connect** | [linkedin.com/in/satamihir](https://www.linkedin.com/in/satamihir/) | the full résumé, always current |
|---|---|---|
| **see it properly** | [satamihir.github.io](https://satamihir.github.io) | the whole thing, seen through sunglasses |
| **based in** | Kitchener, Ontario | open to intermediate & senior full-stack roles, on-site or remote |

<br>

<p align="center">
  <sub><code>&gt; keep looking</code></sub><br>
  <sub>made with love and far too many late nights.</sub>
</p>
