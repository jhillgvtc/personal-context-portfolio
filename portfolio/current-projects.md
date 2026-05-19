# Current Projects

*Last updated: 2026-05-19*

## 1. Dept Restructure 2026 (Director Track)

**Status:** Peer memos drafted, three-way working session pending
**Timeline:** Active, tied to JB's first 90 days
**What it is:** John's proposed restructure to Director of Acquisition & Analytics, mapped against Maria's counter-proposal (analyst + HubSpot Specialist on her side, both of which hollow out John's A&A scope). Peer-facing memos drafted for Maria and Spencer. JB has verbally flagged a Marble Falls Market Development Coordinator as the first A&A hire (conditional on restructure approval).
**What I'm doing:** Holding the lines on A&A scope. "Why Director Tier" section pulled from structure-proposal.md after LLM Council and anti-glaze review. Waiting to send peer memos.
**Done looks like:** Director title with JB's support, based on demonstrated impact. Marble Falls coordinator role opened.

## 2. CallRail Bill Audit

**Status:** Follow-up memo drafted, Atlas cron reminder set
**Timeline:** Decision held pending Maria reply; follow-up fires 2026-06-01
**What it is:** Monthly CallRail bill is $557. Audit identified a 56-number kill list (toll-free dormant >90 days, $1,605–$2,000/yr savings) and that Conversation Intelligence is bundled but recording is OFF (unused feature). May 14 cleanup ask was ignored; 2 new toll-free + 1 more numbers were added 5/15. Maria and Megan have been non-responsive.
**What I'm doing:** Built a local CallRail MCP (TypeScript, six tools, mirrors wave-mcp pattern) to eliminate manual CSV exports for future audits. Smoke-tested 5/18.
**Done looks like:** 56 numbers removed, Conversation Intelligence either turned on or downgraded out of the plan, monthly bill back under $400.

## 3. Edge-Out Business Cases (Growth Series)

**Status:** Methodology template established, two cases in flight
**Timeline:** Granite Shoals award date 2026-06-29 (45-day cycle), Mission Hills overbuild in progress
**What it is:** A series of FTTH edge-out business cases. Johnson City established the methodology template. Granite Shoals (BZC-0476-GRANI, Lake LBJ market, Burnet County) adds seasonal-resident share analysis via homestead-exemption flags. Mission Hills is an overbuild case synthesizing Google Fiber's GTM playbook.
**What I'm doing:** Reusing the Johnson City pattern. High-profile for Granite Shoals — JB-visible.
**Done looks like:** Each case stands on its own business merit; methodology is reusable for the next exchange or subdivision.

## 4. Housing Market Momentum

**Status:** Scaffolding complete, awaiting Power BI report
**Timeline:** Greenfield (started 2026-05-19)
**What it is:** Composite z-score momentum model + dual-track forecast (Prophet/ARIMA + lagged-momentum regression) for Comal County housing. Benchmarks Guadalupe / Kendall / Hays. Full phase scaffolding, CONTEXT/DATA/KNOWLEDGE graphs done.
**What I'm doing:** Discovery phase ready. Awaiting Power BI report from current source.
**Done looks like:** Lead indicator for GVTC's residential acquisition curve, tied to passings and edge-out timing.

## 5. Customer Growth Model

**Status:** Phase 2 active
**Timeline:** Ongoing, Q2 priority
**What it is:** Departmental project for JB. Actionable levers for customer acquisition in a slowing-organic market (real estate headwinds + competitive pressure). PTF received 2026-04-01.
**Phase 2 focus:** Rental capture, county verify, offer hooks, Mobile pitch order. BHAG framing: $200M / 75% share via RGU / ARPU / penetration / win-back (not just passings). 62/9 awareness/loyalty split = structural problem.
**Done looks like:** Data-backed recommendations JB can take to leadership and execute against.

## 6. HubSpot Integration

**Status:** Active, attribution pipeline live
**Timeline:** Ongoing
**What it is:** Standing up HubSpot as a usable system at GVTC. MCP-connected. Diagnosed cart abandon dormancy, inventoried 18 active campaigns, shipped attribution MVP for MultiGig 2026-PTF.
**What I'm doing:** Running attribution on Meyer Ranch and Code Red: Vintage Oaks. Unblocking cart abandon with Megan Darlington. Hubspot-telco-consultant skill grounded in live GVTC instance data.
**Done looks like:** Reproducible attribution pipeline (one campaign ID swap), working cart abandon workflow, contact-level + subdivision-level lift methodology in place.

## 7. Plug-the-Leak / Churn Baseline

**Status:** Baseline locked, cohort comparison ready
**Timeline:** Q2 2026, recurring cadence with Alex Pina
**What it is:** Residential broadband churn baseline + propensity-to-churn work feeding the 500 Mbps upgrade rollout. TTM permanent disconnect rate locked at 8.81%; controllable/upgrade-addressable slice is 2.06%. Sub-500 cohort is stickier than 500+ — reframed the upgrade case from retention-remedial to competitive-defensive. Save-rate walked back from 85-99% to honest 40-55% after pushing back on own number (the phone-bridge view filters out disconnected phones, making the calc tautological).
**Done looks like:** Recurring cadence for Alex, recomputable SQL, cohort-level pre/post comparison for each rollout.

## 8. MVNO Launch / GVTC Mobile

**Status:** GTM blueprint v0 scaffolded
**Timeline:** Tiger Team active, JB-led
**What it is:** GVTC's mobile launch reframed by JB as a "lifecycle value architecture" — machine, not campaign. Unit of analysis: bundled CLV, not single-product P&L. Forced phone bundle was lifted Sept 2025 (SMB previously required phone with internet); 90% voice attach was policy, not preference.
**What I'm doing:** 7-segment x 4-lane x 3-phase blueprint in `2-analysis/gtm-blueprint-v0.md`. Finance pushback playbook from JB's verbatim quotes. Bundled CLV scenario model template.
**Done looks like:** Tiger Team has an aligned operational artifact. Bundled CLV locked as unit of analysis.

## 9. Project Agent Red (Atlas / Identity)

**Status:** Active redesign, Slack regression mitigated
**Timeline:** Ongoing
**What it is:** Identity redesign for the OpenClaw/Atlas agent system on EC2. v2026.3.11+ dropped Slack events; pinned v3.8. Firecrawl replaced Perplexity. Sub-agent workspaces isolated. Connection Finder weekly cron writes Cortex `connections/CONNECTIONS-YYYY-MM-DD.md` (first Karpathy-loop auto-write into the vault).
**Done looks like:** Stable, identity-coherent agent system that supports the broader AI workbench.

## 10. Practical Machines Substack

**Status:** Channel build in progress
**Timeline:** Ongoing
**What it is:** Substack publication using LinkedIn writing as the seed for an AI + telco practitioner audience. Companion to the LinkedIn content stream.
**Done looks like:** Regular cadence, audience growing, distinct voice from the corporate-comms day job.

## 11. Pressings iOS App

**Status:** Apple Developer enrollment submitted, 11-task Todoist backlog
**Timeline:** Personal side-business build
**What it is:** Vinyl record valuation app for audiophile collectors. First real side business. Personal Apple Dev enrollment under jhill387@gmail.com (NOT GVTC team), personal payment. Cloudflare DNS + Email Routing for privacy@ / hello@ → jhill387@gmail.com.
**Done looks like:** App published, monetized, first paying users.

## 12. Expense Budget FY26 (Three-Way Realignment)

**Status:** John's budget mapped, awaiting Maria's and Spencer's
**Timeline:** Q2 2026
**What it is:** Three-column line-item budget mapping under JB's restructure (Acquisition & Analytics / Lifecycle & Brand / Digital Experience & Conversion). John ~$401K envelope (DGTLsuite $118K moved from IT for FY26 = 29%). Maria ~$1.2M, Spencer small.
**What I'm doing:** Pending Maria's and Spencer's mappings for cross-column reconciliation. Realignment one-pager comes after all three are mapped.
**Done looks like:** Three-way realignment proposal goes to JB with clean column ownership and dollars.

## 13. Spencer Claude Code Onboarding

**Status:** Active onboarding under restructure
**Timeline:** Ongoing
**What it is:** Spencer takes ecommerce ownership under the proposed restructure (SHOM approved 2026-04-30). Onboarding him to Claude Code is part of the transition.
**Done looks like:** Spencer self-sufficient in Claude Code for ecommerce workflows; ecommerce handoff clean.

## Watching, Not Driving

- **NPS Sentiment Analysis pipeline** — productized as the `nps-sentiment` skill; runs on demand.
- **Ping** — launched April 2026, Q2 performance review pending.
- **Call Center Sales Analytics** — Phase 1 numbers shipped to JB; Phase 2 plan written. Weekly retention triage list as first downstream deliverable.

## No Hard Deadlines

Most have no fixed due dates. Success is measured by impact and momentum. The implicit deadline is the Director conversation under JB.
