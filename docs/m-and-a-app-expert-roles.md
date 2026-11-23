# Expert Roles for Building an M&A Decision-Support Application

*Prepared November 23, 2026 · Companion to [ges-company-research.md](./ges-company-research.md)*

## How to read this

An M&A application helps executives answer four questions about any target:

1. **Is it worth buying?** (strategy and fit)
2. **What is it worth?** (valuation and financing)
3. **What could go wrong?** (diligence and risk: financial, legal, people, tech)
4. **Can we make it work after closing?** (integration and value creation)

Each question belongs to different specialists. You don't need to hire all of them full time. Most act as **subject-matter advisors**: they tell you what the app must calculate, track, flag and show, and they check that the output is right. A small core team then builds it.

Each role below lists:
- **What they bring to the app**: the knowledge you turn into features.
- **Priority**: **Core** (needed from day one), **Phase 2** (once the basics work), or **Situational** (only for certain deal types).
- **Engagement**: full-time, part-time, or advisor (a few hours a month or a set of interviews).

Where GES's situation makes a role especially important, it's marked **GES note**. GES is a PE-backed buy-and-build platform with union labor, international operations, event-tech assets and attendee data.

---

## 1. Business & Deal Domain Experts

These people know *how deals are actually done*. Without them you'll build a nice-looking app that executives don't trust.

| Role | What they bring to the app | Priority | Engagement |
|---|---|---|---|
| **Corporate Development / M&A Director** (ex-corp dev at an acquisitive company) | The end-to-end deal process and its stages (sourcing → NDA → IOI → LOI → diligence → signing → close). What executives need to see at each decision gate. Pipeline management. Investment committee memo format. **This is your most important domain advisor.** | Core | Advisor → part-time |
| **Investment Banker (M&A Advisory)** | How deals are marketed and priced. Auction vs. negotiated processes. Comparable transactions. Deal structures (cash, stock, earn-outs, rollover equity). What a "good" teaser, CIM and IOI look like. | Core | Advisor |
| **Private Equity Professional / Operating Partner** | Buy-and-build logic. Add-on economics ("multiple arbitrage"). Value creation plans. How a sponsor reviews a platform's deals. Board and sponsor reporting. **GES note:** Truelink Capital is the sponsor, so the app must speak PE's language. | Core | Advisor |
| **Corporate Strategy Consultant** | Strategic fit frameworks, market sizing, competitive positioning, "build vs. buy vs. partner" analysis, target screening criteria and scoring models. | Core | Advisor |
| **Industry Subject-Matter Expert: Events & Exhibitions** (former GSC/agency operator or exec) | What makes an events business valuable: show contracts and renewal dates, venue exclusives, show rotation cycles, exhibitor revenue, labor markets by city, seasonality. Which KPIs to track. Who the realistic targets are. **GES note:** essential. Generic M&A software doesn't understand trade shows. | Core | Advisor → part-time |
| **Post-Merger Integration (PMI) Lead** | 100-day plans, integration workstreams, brand strategy (absorb vs. keep the acquired brand), synergy tracking, retention of key people. **GES note:** GES keeps acquired brands as "operating companies," so the app should track integration for that model. | Phase 2 | Advisor |
| **Synergy / Value Creation Analyst** | How to estimate and track synergies: revenue (cross-sell), cost (procurement, warehouses, freight), and how to measure whether they actually happened after closing. | Phase 2 | Advisor |
| **Commercial Due Diligence Specialist** | Customer interviews, churn and concentration analysis, market checks. Turns "they have great clients" into data. | Phase 2 | Advisor |

---

## 2. Financial, Valuation & Accounting Experts

These people make sure the numbers in the app are right. If executives find one bad number, they stop trusting the tool.

| Role | What they bring to the app | Priority | Engagement |
|---|---|---|---|
| **Valuation / Financial Modeling Analyst** (investment banking or Big 4 valuation background) | The calculation logic: DCF, trading comps, precedent transactions, LBO / returns (IRR, MOIC), accretion/dilution, sensitivity tables. Defines every formula the app runs. | Core | Part-time → full-time |
| **FP&A / Corporate Finance Lead** | Ties target financials to the acquirer's budget and plan. Pro forma combined P&L. What the CFO needs to see. | Core | Advisor |
| **Transaction Services / Quality of Earnings (QoE) Accountant** (CPA, Big 4 or boutique) | EBITDA adjustments and normalization, working capital pegs, debt-like items, red flags in financials. **GES note:** revenue must be normalized for 2–4-year show rotation. | Core | Advisor |
| **M&A Tax Advisor** | Deal structure (asset vs. stock purchase), tax step-ups, NOLs, cross-border tax, transfer pricing. Tax shapes what a deal is really worth. **GES note:** UK, EU, Middle East and India operations. | Phase 2 | Advisor |
| **Technical Accounting Specialist** | Purchase accounting (ASC 805 / IFRS 3), purchase price allocation, goodwill, earn-out accounting, revenue recognition (ASC 606). | Phase 2 | Advisor |
| **Leveraged Finance / Treasury Specialist** | Debt capacity, financing structures, covenants, cost of capital. PE-backed deals are usually debt-funded, so this limits what GES can afford. | Situational | Advisor |
| **Financial Data Analyst** | Sources and cleans comps and market data (PitchBook, S&P Capital IQ, Bloomberg). Keeps the reference data in the app current. | Phase 2 | Part-time |

---

## 3. Legal Experts

Legal problems are the most common deal-killers, and they're very hard to fix after closing. The app should surface legal risk early and track it through diligence.

| Role | What they bring to the app | Priority | Engagement |
|---|---|---|---|
| **M&A / Corporate Transactions Attorney** | Deal documents (NDA, LOI, purchase agreement), reps & warranties, indemnities, closing conditions. The structure of the legal diligence checklist and issue-tracking workflow. | Core | Advisor |
| **Antitrust / Competition Counsel** | HSR filing thresholds, when a deal needs regulatory review, market-concentration risk. **GES note:** buying competing trade show contractors raises the risk. Relevant at least in the US, UK and EU. | Situational → Core for competitor deals | Advisor |
| **Labor & Employment Counsel** | Union collective bargaining agreements (successorship, withdrawal liability), worker classification (freelance crews), WARN Act, non-competes, retention agreements. **GES note:** critical. GES has about 100 CBAs. | Core | Advisor |
| **Commercial Contracts Counsel** | Change-of-control and assignment clauses in customer, venue and supplier contracts, i.e. whether the show and venue contracts survive the sale. **GES note:** venue exclusives and show contracts *are* the asset. | Core | Advisor |
| **Data Privacy & Cybersecurity Counsel** | GDPR, UK GDPR, CCPA, data-transfer rules. Inherited privacy liability. **GES note:** Visit by GES and onPeak handle attendee and hotel data in Europe. Event-tech targets will too. | Phase 2 | Advisor |
| **Intellectual Property Counsel** | Ownership of software, trademarks and creative work. Open-source license risk in tech targets. Agency work-product ownership. | Situational (tech/agency deals) | Advisor |
| **International / Cross-Border Counsel** | Local deal law, foreign investment rules, employment law in the UK, EU, UAE, Qatar and India. | Situational | Advisor |
| **Regulatory & Compliance Counsel** | Anti-corruption (FCPA, UK Bribery Act), sanctions and export controls. Important for Middle East and government-adjacent work. | Situational | Advisor |
| **Securities / Confidentiality Counsel** | Rules for handling confidential deal information inside the app (NDAs, clean teams, insider information if any party is public). Data retention policy. | Core (for the app itself) | Advisor |

---

## 4. Risk & Operational Due Diligence Specialists

| Role | What they bring to the app | Priority | Engagement |
|---|---|---|---|
| **HR / People Due Diligence Specialist** | Org charts, key-person risk, compensation benchmarking, benefits and pension liabilities, retention planning, culture fit assessment. | Phase 2 | Advisor |
| **IT / Technology Due Diligence Specialist** | Tech-stack assessment, technical debt, scalability, cost to integrate systems. **GES note:** essential for event-tech (registration, badging, lead retrieval) targets. | Situational | Advisor |
| **Cybersecurity Assessor** | Security posture of targets, breach history, inherited cyber risk. | Situational | Advisor |
| **Operations / Supply Chain Expert** | Warehouses, freight and logistics, equipment and inventory condition, rental fleet utilization. **GES note:** GES is very asset- and logistics-heavy. | Phase 2 | Advisor |
| **Insurance / Risk Advisor** | Representations & warranties (R&W) insurance, coverage gaps, claims history. | Situational | Advisor |
| **ESG / Sustainability Specialist** | ESG diligence, carbon reporting. **GES note:** GES publishes ESG and event-emissions reporting, and European clients increasingly require it. | Situational | Advisor |
| **Risk Management Specialist** | Builds the overall risk framework (likelihood × impact) that the app uses to score and roll up risks from every workstream. | Phase 2 | Advisor |

---

## 5. Data, Analytics & AI

| Role | What they bring to the app | Priority | Engagement |
|---|---|---|---|
| **Data Analyst / BI Developer** | Executive dashboards, pipeline reporting, portfolio views, KPI definitions. | Core | Full-time or part-time |
| **Data Engineer** | Pipelines from data providers (PitchBook, Capital IQ, Crunchbase, LinkedIn, news feeds), CRM and document sources. Data model for companies, deals, contacts and documents. | Phase 2 | Full-time or contractor |
| **Data Scientist** | Target scoring and ranking models, similarity search ("find companies like CSG"), predictive signals (e.g., founder age, PE hold period, so likely to sell). | Phase 2 | Part-time |
| **AI / LLM Engineer** | Document analysis (CIMs, contracts, data-room files), summarizing diligence findings, contract clause extraction (change-of-control, non-compete), memo drafting. Must be built with strict confidentiality controls. | Phase 2 | Full-time or contractor |
| **Market Research Analyst** | Builds and maintains the target universe for each category (regional GSCs, association agencies, event-tech, etc.). | Core | Part-time |

---

## 6. Product, Design & Engineering (the build team)

| Role | What they bring to the app | Priority | Engagement |
|---|---|---|---|
| **Product Manager** (ideally with fintech, deal-management or B2B SaaS experience) | Turns expert input into requirements, prioritizes features, owns the roadmap, runs user interviews with executives. **This is likely you.** | Core | Full-time |
| **UX / UI Designer** (experienced with data-heavy enterprise and executive dashboards) | Executives skim. The app must make decisions obvious at a glance: one-page deal summaries, red/amber/green risk, clear comparisons. | Core | Part-time → full-time |
| **Full-Stack Software Engineer(s)** | Builds the application. | Core | Full-time (1–3) |
| **Security Engineer / Architect** | Deal data is extremely sensitive. Covers role-based access per deal, encryption, audit logs, SSO, a "need-to-know" permission model, and secure document storage. A leak can kill a deal or create legal liability. | Core | Part-time / consultant |
| **DevOps / Cloud Engineer** | Hosting, backups, uptime, environments, compliance-ready infrastructure (SOC 2 path). | Phase 2 | Part-time / contractor |
| **QA / Test Engineer** | Especially for checking that financial calculations are correct. A wrong IRR is a serious bug. | Phase 2 | Part-time |
| **Integration Engineer** | Connects to tools executives already use: CRM (Salesforce, HubSpot, DealCloud), virtual data rooms (Datasite, Intralinks), Excel models, email/calendar, ERP. | Phase 2 | Contractor |
| **Technical Writer / Trainer** | User guides, playbooks, onboarding for executives and deal teams. | Situational | Contractor |

---

## 7. Users & Stakeholders to Interview (not hires, but essential)

These are the people the app serves. Interview them early and often.

| Stakeholder | What you need to learn from them |
|---|---|
| **CEO** (e.g., Derek Linde at GES) | Strategic priorities, what they need to say yes or no, how they want to compare deals |
| **CFO** | Financial thresholds, return hurdles, how deals are funded, board and lender reporting |
| **Head of Corporate Development** | Day-to-day workflow, current tools (often Excel + email), pain points |
| **Business Unit Leaders** (e.g., GES Exhibitions, Spiro, onPeak, Visit) | What capabilities or geographies they want acquired, and who will own integration |
| **PE Sponsor Deal Team** (e.g., Truelink) | Investment committee requirements, reporting formats, value-creation tracking |
| **Board of Directors** | What level of summary they want, approval thresholds |
| **Integration Managers** | Post-close tracking needs |
| **General Counsel** | Legal workflow, confidentiality requirements, document handling |

---

## 8. Recommended Starting Team (for a "small" app)

You don't need 40 people. A realistic lean setup for an MVP:

**Build team (3–5 people)**
1. Product Manager (you)
2. 1–2 Full-Stack Engineers
3. UX/UI Designer (part-time)
4. Security architect (consultant, especially for the permission model)

**Core expert advisors (5–6 people, a few hours a month each)**
1. **Corporate Development / M&A Director**: deal process and workflow
2. **Valuation / Financial Modeling Analyst**: all the math
3. **Events & Exhibitions Industry SME**: makes the app specific to GES's world
4. **M&A Attorney**: legal diligence structure and confidentiality rules
5. **QoE / Transaction Accountant**: financial diligence and EBITDA adjustments
6. **Labor & Employment Counsel**: union and worker issues (high priority for GES)

**Add in Phase 2:** PE operating partner, PMI lead, tax advisor, data engineer, data scientist / AI engineer, IT diligence, privacy counsel, antitrust counsel (once you start looking at competitor deals).

> **Tip:** One person can often cover several roles. A former investment banker who moved into corporate development can cover deal process, valuation *and* banker perspective. A Big 4 transaction services alum often knows QoE *and* tax basics. Ex-employees of Freeman, Shepard, GES or similar firms make excellent industry SMEs.

---

## 9. How the Roles Map to App Features

| App module | Lead experts |
|---|---|
| Target universe & screening | Market research analyst, industry SME, strategy consultant, data scientist |
| Deal pipeline / CRM | Corp dev director, PM |
| Strategic fit scoring | Strategy consultant, industry SME, corp dev director |
| Valuation & returns models | Valuation analyst, investment banker, PE professional, FP&A |
| Financial diligence (QoE) | Transaction accountant, tax advisor, technical accounting |
| Legal diligence & contract review | M&A attorney, contracts counsel, labor counsel, privacy counsel, AI engineer |
| Risk register & red flags | Risk specialist + every diligence workstream |
| Investment committee memo / executive summary | Corp dev director, PE professional, UX designer |
| Integration & synergy tracking | PMI lead, synergy analyst, HR diligence |
| Security, permissions & audit trail | Security architect, securities/confidentiality counsel |
| Dashboards & reporting | BI developer, UX designer, CFO input |

---

## 10. Important Caveat

The app should **support** executive decisions, not replace professional advice. Valuations, legal conclusions and tax structures still need sign-off from licensed professionals (attorneys, CPAs, bankers) on each real deal. Build that into the workflow, for example with an "expert review / sign-off" status on key outputs. That also makes executives trust the tool more.
