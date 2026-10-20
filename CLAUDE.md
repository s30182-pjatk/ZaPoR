# CLAUDE.md — ZPR course project: Com.com

Context file for Claude (and other AI assistants) continuing work on this project. Read it fully before doing anything. Mirrored in GEMINI.md — keep both files in sync when either changes.

## What this is

- **Course:** ZPR (university course, project-management focused). Work is done in a group.
- **Deliverables:** a series of numbered assignment documents ("ZPR Assignment #N"), each describing the same fictional IT project from a different project-management angle. The assignment brief for each one is provided by the lecturer as a PDF.
- **The group's project:** **Com.com** — a gamified online community platform.
- **Owner of this workspace:** Gleb Denisov (software developer, group member).

## Assignment status

| # | Assignment | Status | Files |
|---|------------|--------|-------|
| 1 | Project Overview Statement | Done | Brief: `zpr-1-project-ovierview-statement.pdf` · Submission: `ZPR_01_Com_com_Project_Overview_Statement 1.pdf` |
| 2 | Stakeholder Identification | **Next / to do** (printed 05.10.2026) | Brief: `zpr-2-stakeholder-identification.pdf` |
| 3+ | Not yet issued | — | — |

Naming convention for submissions: `ZPR_<NN>_Com_com_<Assignment_Name>.<ext>` (e.g. `ZPR_02_Com_com_Stakeholder_Identification.docx`).

## Com.com — canonical project facts (from Assignment #1)

Keep every new document consistent with these. Do not invent contradicting details.

**Business case.** Online communities/forums struggle with long-term retention because participation rarely feels rewarding. Com.com turns community activity into a game: posts, comments and conversations earn progress via XP, loyalty points, chests, unlockable perks and leaderboards. Target demographic: **males aged 18–35**. The in-game currency is **fully convertible both ways** (buy with real money, cash out to real money). Secure, **high-privacy** communication is the foundation. Revenue: **cosmetic microtransactions** (avatar skins, chests) and **currency-exchange fees**.

**Goals**
1. Gamification engine (core of the product): loyalty points, XP, chests, unlockable perks → visible progression.
2. Interactive avatar profile system + global leaderboard.
3. Fully convertible in-game currency, two-way exchange.
4. Communication platform: threads, posts, comments, like/dislike, encrypted private chat.
5. High-privacy data architecture.
6. Secure payment gateway: skins, currency purchases, real-money payouts.

**Criteria for success**
- Gamification system deployed as centrepiece of the MVP (users reliably earn points/XP/chests, progression visible on leaderboard).
- Functional MVP with bug-free threads and private chat feeding the reward system.
- Secure payment pipeline: microtransactions + two-way exchange (purchases and verified withdrawals).
- Passed security audit before launch.

**Assumptions**
- Target demographic responds to gamified retention and cosmetic progression.
- Team has access to frameworks, payment/payout APIs, KYC services, encryption tools.
- App-store approval without friction for marketplace and real-money exchange.
- Required licences/regulatory approvals for a real-money exchange can be obtained.

**Risks**
- Engagement mechanics failure (repetitive, unbalanced, exploitable reward loop).
- Privacy vulnerabilities / breach → loss of trust, churn.
- Market saturation (competition from established social networks).
- Monetization failure (revenue doesn't cover server/maintenance costs).
- Regulatory & financial risk (e-money, AML, gambling rules — esp. randomised chests + cash-out; KYC, tax reporting).
- Currency abuse & fraud (bot farming, multi-accounting, exploits).
- Platform compliance (app-store rejection over microtransactions / real-money exchange / insufficient UGC moderation).

**Main tasks**
1. Gamification & reward system design (reward loop, progression curves, currency economy, leaderboard, avatar progression).
2. System architecture & UI/UX design (wireframes, gamification at the centre).
3. Backend development (XP/points engine, secure DBs, E2E encryption for private chat).
4. Frontend development (live leaderboards, avatar builder, threads, comments).
5. Payment integration (store, two-way exchange, payouts, exchange-rate/fee logic, KYC, anti-fraud).
6. QA & security auditing (exploit prevention, bugs, privacy verification).
7. Deployment & launch (production release, targeted marketing).

## Next task: Assignment #2 — Stakeholder Identification

Brief: identify the most important stakeholders. For **each** stakeholder specify:
1. Involvement in the project + type of interest (**positive / negative**).
2. Knowledge and competence level.
3. Expectations towards the product.
4. Potential influence on the project.

Lecturer's example format (follow it):

> **Game publishers**
> • Type of interest: positive.
> • Involvement: will sponsor development of games and publish games for the new console.
> • Knowledge / competence: high.
> • Expectations: high initial console sales, high number of preorders, good publisher / platform owner split, measures to limit resale of used games.
> • Potential influence: high, good availability of third-party titles is important, especially at launch.

Stakeholders that follow naturally from Assignment #1 (suggestions, not yet agreed with the group): end users (males 18–35); project sponsor / investors; development team (backend, frontend, UI/UX, QA); content moderators / community managers; payment gateway & payout providers; KYC / identity-verification providers; app-store operators (Apple, Google); financial regulators (e-money, AML, gambling authorities); tax authorities; data-protection authorities (GDPR); security auditors; competing social networks (negative interest); fraudsters / bot farmers (negative interest); advertisers/marketing partners; parents & consumer-protection groups (likely negative, re: chests resembling gambling).

Include a mix of positive and negative stakeholders — the brief explicitly asks for the interest type.

## Writing conventions

- Language: **English**. Assignment #1 mostly uses British spelling ("centrepiece") but writes "Monetization" — pick one style and keep it consistent within a document.
- Tone: concise, formal project-management style; bullet points with bold lead-ins, as in Assignment #1.
- Structure each document with numbered sections matching the brief's numbered points.
- Title format: `<Assignment Name>: Com.com`.
- Length: Assignment #1 is ~2 pages; aim for similar unless the brief demands more.
- Always cross-check new content against the canonical facts above (target group, convertible currency, high privacy, chests, KYC, etc.).

## Working notes for the assistant

- Before drafting, re-read the relevant brief PDF — briefs are short and precise; answer every point they list.
- Output as a document the group can edit and submit (Word/PDF or a shared doc, as the user prefers).
- Ask before changing any canonical fact from Assignment #1; if a later assignment requires a change, update this file and GEMINI.md too.
- When an assignment is completed, update the status table above (in both CLAUDE.md and GEMINI.md).
