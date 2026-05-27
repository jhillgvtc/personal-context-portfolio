# Current Projects

*Last updated: 2026-05-27*

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

## 3. Competitor Overbuild Impact Model

**Status:** Phase 2 model built, Phase 3 (stress-test) next
**Timeline:** Active, executive deliverable for JB/PTF
**What it is:** Models what happens when a historically non-competitive GVTC subdivision gets overbuilt. Four case studies (Meyer Ranch, Vintage Oaks, Herff Ranch, Esperanza). Three scenarios: Spectrum defended (-13pp/12mo), Spectrum larger/slower (-8 to -12pp/18mo), Frontier/AT&T price-led (-18pp/12mo). Revenue-at-risk: $1.62M annualized at 12 months across top 9 communities. Three competitor archetypes: Spectrum (cable-to-fiber), Frontier ($49 price-led), AT&T (fiber + wireless bundle).
**What I'm doing:** Stress-testing raw model outputs before building the deck + report for JB.
**Done looks like:** Executive-facing deck + report that answers "what happens to Copper Ridge when it's Copper Ridge's turn."

## 4. Edge-Out Business Cases (Growth Series)

**Status:** Methodology template established, two cases in flight
**Timeline:** Granite Shoals award date 2026-06-29 (45-day cycle), Mission Hills overbuild in progress
**What it is:** A series of FTTH edge-out business cases. Johnson City established the methodology template. Granite Shoals (BZC-0476-GRANI, Lake LBJ market, Burnet County) adds seasonal-resident share analysis via homestead-exemption flags. Mission Hills is an overbuild defense case with town hall June 3/4, flyer and operating plan delivered, Google Fiber GTM playbook synthesized.
**What I'm doing:** Mission Hills: town hall execution, Copper Ridge flagged as related defensive play (600 rooftops, 96% pen, AT&T at the gate). Granite Shoals: reusing Johnson City pattern, JB-visible.
**Done looks like:** Each case stands on its own business merit; methodology is reusable for the next exchange or subdivision.

## 5. Housing Market Momentum

**Status:** Monthly brief v1 shipped GREEN to PTF
**Timeline:** Monthly cadence (next refresh: June)
**What it is:** MACD-based housing cycle detection + ETS forecasts for Comal County. Monthly brief with operational implications for GVTC rooftop planning, marketing timing, and edge-out pacing. Gonzales County removed from scope (avg 6 sales/month too small for stable signals). Comal-only for v1.
**What I'm doing:** May brief shipped. Monthly refresh cadence established. TRERC data pipeline + Playwright automation for pull. Full telco-domain audit pass cleared.
**Done looks like:** Lead indicator for GVTC's residential acquisition curve, tied to passings and edge-out timing. Monthly PTF deliverable.

## 6. Customer Growth Model

**Status:** Phase 2 active
**Timeline:** Ongoing, Q2 priority
**What it is:** Departmental project for JB. Actionable levers for customer acquisition in a slowing-organic market (real estate headwinds + competitive pressure). PTF received 2026-04-01.
**Phase 2 focus:** Rental capture, county verify, offer hooks, Mobile pitch order. BHAG framing: $200M / 75% share via RGU / ARPU / penetration / win-back (not just passings). 62/9 awareness/loyalty split = structural problem.
**Done looks like:** Data-backed recommendations JB can take to leadership and execute against.

## 7. HubSpot Integration

**Status:** Active, attribution pipeline live + CRM integrity audit in flight
**Timeline:** Ongoing
**What it is:** Standing up HubSpot as a usable system at GVTC. MCP-connected. Diagnosed cart abandon dormancy, inventoried 18 active campaigns, shipped attribution MVP for MultiGig 2026-PTF. WiFi Score audit surfaced 7 contacts in 6.5 years vs stakeholder claim of "biggest lead generator." Found 16,639 contacts mis-tagged with invisible `acct_num` field. Shipped diagnostic CSV to Anil (IT) with per-row diagnostic questions.
**What I'm doing:** Running attribution on Meyer Ranch and Code Red: Vintage Oaks. Diagnostic handoff to Anil pending (PTO + family emergency). SOP brainstorm with Maria/Megan still owed.
**Done looks like:** Reproducible attribution pipeline (one campaign ID swap), working cart abandon workflow, contact-level + subdivision-level lift methodology in place, lifecycle data integrity restored.

## 8. Plug-the-Leak / Churn Baseline

**Status:** Baseline locked, cohort comparison ready
**Timeline:** Q2 2026, recurring cadence with Alex Pina
**What it is:** Residential broadband churn baseline + propensity-to-churn work feeding the 500 Mbps upgrade rollout. TTM permanent disconnect rate locked at 8.81%; controllable/upgrade-addressable slice is 2.06%. Sub-500 cohort is stickier than 500+ — reframed the upgrade case from retention-remedial to competitive-defensive. Save-rate walked back from 85-99% to honest 40-55% after pushing back on own number (the phone-bridge view filters out disconnected phones, making the calc tautological).
**Done looks like:** Recurring cadence for Alex, recomputable SQL, cohort-level pre/post comparison for each rollout.

## 9. MVNO Launch / GVTC Mobile

**Status:** GTM blueprint v0 scaffolded
**Timeline:** Tiger Team active, JB-led
**What it is:** GVTC's mobile launch reframed by JB as a "lifecycle value architecture" — machine, not campaign. Unit of analysis: bundled CLV, not single-product P&L. Forced phone bundle was lifted Sept 2025 (SMB previously required phone with internet); 90% voice attach was policy, not preference.
**What I'm doing:** 7-segment x 4-lane x 3-phase blueprint in `2-analysis/gtm-blueprint-v0.md`. Finance pushback playbook from JB's verbatim quotes. Bundled CLV scenario model template.
**Done looks like:** Tiger Team has an aligned operational artifact. Bundled CLV locked as unit of analysis.

## 10. Project Agent Red (Atlas / Identity)

**Status:** Active redesign, Slack regression mitigated
**Timeline:** Ongoing
**What it is:** Identity redesign for the OpenClaw/Atlas agent system on EC2. v2026.3.11+ dropped Slack events; pinned v3.8. Firecrawl replaced Perplexity. Sub-agent workspaces isolated. Connection Finder weekly cron writes Cortex `connections/CONNECTIONS-YYYY-MM-DD.md` (first Karpathy-loop auto-write into the vault).
**Done looks like:** Stable, identity-coherent agent system that supports the broader AI workbench.

## 11. Practical Machines Substack

**Status:** Channel build in progress
**Timeline:** Ongoing
**What it is:** Substack publication using LinkedIn writing as the seed for an AI + telco practitioner audience. Companion to the LinkedIn content stream.
**Done looks like:** Regular cadence, audience growing, distinct voice from the corporate-comms day job.

## 12. Pressings iOS App

**Status:** Apple Developer approved, bundle ID + API key set, launch sprint queued
**Timeline:** Personal side-business build, Todoist tasks dated 2026-05-27
**What it is:** Vinyl record valuation app for audiophile collectors. First real side business. Personal Apple Dev enrollment approved under jhill387@gmail.com (NOT GVTC team). Bundle ID `com.pressings.app` registered, App Store Connect API key (.p8) generated. Remaining: screenshots, ASC app record + listing copy + privacy nutrition, Codemagic CI build, TestFlight smoke test, submit for review.
**Done looks like:** App published, monetized, first paying users.

## 13. Expense Budget FY26 (Three-Way Realignment)

**Status:** John's budget mapped, awaiting Maria's and Spencer's
**Timeline:** Q2 2026
**What it is:** Three-column line-item budget mapping under JB's restructure (Acquisition & Analytics / Lifecycle & Brand / Digital Experience & Conversion). John ~$401K envelope (DGTLsuite $118K moved from IT for FY26 = 29%). Maria ~$1.2M, Spencer small.
**What I'm doing:** Pending Maria's and Spencer's mappings for cross-column reconciliation. Realignment one-pager comes after all three are mapped.
**Done looks like:** Three-way realignment proposal goes to JB with clean column ownership and dollars.

## 14. Spencer Claude Code Onboarding

**Status:** Active onboarding under restructure
**Timeline:** Ongoing
**What it is:** Spencer takes ecommerce ownership under the proposed restructure (SHOM approved 2026-04-30). Onboarding him to Claude Code is part of the transition.
**Done looks like:** Spencer self-sufficient in Claude Code for ecommerce workflows; ecommerce handoff clean.

## Watching, Not Driving

- **NPS Sentiment Analysis pipeline** — productized as the `nps-sentiment` skill; runs on demand.
- **Ping** — launched April 2026, Q2 performance review pending. Lead attribution pipeline (phone-match) found unreliable (0/11 name-verified); v2 with address matching needed.
- **Call Center Insights** — Phase 1 numbers shipped to JB; Phase 2 plan written. Pre-churn signals identified (7.2x lift on inbound callers, 44x on RTC calls). Weekly retention triage list as first downstream deliverable. Operationalization gated on retention team bandwidth.

## No Hard Deadlines

Most have no fixed due dates. Success is measured by impact and momentum. The implicit deadline is the Director conversation under JB.
