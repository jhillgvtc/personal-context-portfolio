# Decision Log

## How I Decide

**Default mode:** Fast intuition, then validation. Gather inputs, make the call, move. Reversible decisions get made quickly. Irreversible ones get more scrutiny.

**When stuck:** Build a decision matrix or scoring framework (often with AI help) to force logical evaluation. Remove emotion, look at the data.

**Decision filter (from my operating manual):**
1. Does this serve my daughter's experience of having a present father?
2. Does this move me toward director-level impact?
3. Does this build AI capability that creates real business value?
4. Does this align with my five principles (Family, Learning, Accountability, Travel, Conscientiousness)?

---

## Recent Decisions

### VP Passed Over -- How I Responded (and What I Learned)

**Situation:** Jeff M. (my boss of 10 years) retired. I expected to be considered for his VP of Sales & Marketing role. The company hired JB externally instead.

**What I did:** I took it personally. Shut down for a couple of months. Didn't produce much at work. People noticed. It was out of character and it showed.

**What I should have done:** Worked harder and created even more value while quietly deciding whether to stay or leave. The emotional withdrawal made things worse, not better.

**What I learned:**
- I'm human and have blind spots around negative professional outcomes.
- I don't always handle rejection well. Social withdrawal is a serious warning sign for me.
- Resilience is a muscle I need to build. The effective response to disappointment is to channel energy into demonstrating value, not to broadcast unhappiness.
- I've corrected course. Now making real momentum with data and AI work.

### Specialist Vendor Strategy

**Situation:** Needed to bring on a Facebook ads vendor. Could have hired a full-service agency that does Facebook, SEO, Google Ads, and more.

**What I decided:** Hired Ping Marketing, a specialist that ONLY does full-funnel Facebook ads (creative, traffic, leads, qualification, conversion).

**Why:** When someone says they're good at everything, they're usually average. I'd rather have one vendor that's excellent at one thing than one that's mediocre at three. And if they underperform, I can cut them without disrupting other channels.

### Save Rate -- Walked Back from 85-99% to 40-55% (2026-04-27)

**Situation:** Computed call center disconnect-call save rate at 85-99% from a HubSpot/DW phone bridge. Looked great. Was on the way to JB.

**What I did:** Pushed back on my own number. Bet next month's mortgage that retention performance was much worse.

**Why it was wrong:** The phone-bridge view filters out disconnected customers' phones. The matched cohort is by construction the non-churners -- the calc was tautological. Cross-checked against actual residential disconnect counts (3,694 in 2024, 4,036 in 2025, +9.3% YoY). Realistic save rate is 22-67%, most likely 40-55%.

**What I learned:** Audit the filter before auditing the rate. "Save rate" computed from a view that silently excludes the population you're measuring is confidently wrong, not usefully imprecise. Walked back the prior bound entirely -- would have been unflattering to Brandy's team the moment anyone looked at actual disconnect numbers.

### Operating Model v1 + Analyst Role (2026-04-27)

**Situation:** Director-track narrative is "AI capability nobody else delivers." That same capability has zero redundancy -- if I'm out, the work stops.

**What I decided:** The Director scope-case AND the single-point-of-failure problem are the same problem. Externalizing tacit work into a person-agnostic archive IS the Director scope-case. Built v1 of the Operating Model today using the work-operating-model skill (5 layers, 21 entries, 6 contradictions). Quarterly rerun fires Jul 6 -- v1 to v2 diff is the actual promotion-evidence artifact.

**Why:** Career pulse came in at 7.0/10. Two structural gaps (People Leadership 4/10, Visibility) both close with one move: proposing the analyst role + archive to JB.

### Portfolio Split -- State vs Pattern (2026-05-07)

**Situation:** The 4/27 biweekly portfolio refresh flagged a decay-rate mismatch. State-heavy files (current-projects, goals, tools) went stale in 24 days because four major projects spun up. Pattern-heavy files (decision-log, communication-style, principles) aged fine. The biweekly cadence was correct for state, overkill for pattern.

**What I decided:** Add `now.md` -- a state-heavy weekly file covering open questions, recent reading, and loading-up decisions. Pattern-heavy files move to quarterly refresh. Biweekly cadence becomes the experiment, not the default.

**Why:** A portable identity portfolio that tries to be a snapshot of state decays in two weeks. Only the parts that capture pattern age well. Different decay rates need different cadences -- one ritual can't cover both without going stale or burning cycles.

**Test:** Two refreshes from now (~5/21), decide whether to retire the biweekly cadence entirely, keep it as the quarterly forcing function for pattern files, or fold the pattern files into a different review (annual operating-model rerun).

### Verify Inputs Before Building — Promoted to Rule (2026-05-15)

**Situation:** Three back-to-back incidents in one week clustered around the same posture failure:
1. **5/14** — Built a Cybertruck affordability model on a 6.5% loan rate placeholder + an assumed-active $7,500 federal EV credit. Firecrawl primary-source pulls returned 4.99%/5.25% from RBFCU's real rate page and surfaced that the EV credit had ended Sept 30, 2025 under OBBBA Public Law 119-21 (replaced by a smaller loan-interest deduction). Net effect: ~$70/mo from the rate, ~$110/mo penalty from the lost credit. Recommendation flipped from "close but doesn't fit" to "doesn't fit at all."
2. **5/15** — Health insurance consolidation request: dictated "Cigna." Workspace evidence (filled forms, member IDs, insurance-profile skill) pointed to SISCO Benefits. Whisper Flow had misheard "SISCO" as "Cigna." Caught in planning, before building a Cigna-themed folder and memory entries that would have compounded across future sessions.
3. **5/15** — GVTC Arlo bundle SKU over-count. v1 cohort sizing keyed to parent CatalogID put 1,488 500 Mbps customers into the "1 Gig + Arlo" bucket (4x over-statement). Separately, the "Premium Home WiFi" line was proposed as a voluntary attach signal, but 99.5% of those lines were bundled-in defaults, not behavioral choices.

**What I decided:** Promoted the pattern to `~/.claude/rules/verify-inputs-before-building.md`. The reflex: when taking an input that will drive a recommendation, ask three questions before treating it as load-bearing — where did this come from, what's the primary source, have I checked it against the primary source in this conversation.

**Why:** Three incidents in one week with the same failure mode = systemic, not anecdotal. The promotion threshold from `~/.claude/rules/feedback-as-signal.md` fired exactly as intended.

### Peer-Memo Register Rewrite (2026-05-14)

**Situation:** Restructure proposal memo to Maria and Spencer was originally drafted in the same register as memos that go *up* to JB (frame, contrast, "why this is the right call"). That register reads as politicking when sent sideways.

**What I decided:** Rewrote as a read-aloud, peer-facing register. Dropped "what they said vs true" contrast framing. Neutralized names. No "private-reply appendix." Pulled "Why Director Tier" entirely after LLM Council pressure-tested it.

**Why:** Co-presented documents land different than directional memos. Naming the bundle problem doesn't dissolve it — cutting does. Memory entry: `feedback_co_presented_doc_framing.md`.

### Maria's Structure Proposal — Hold the Lines (2026-05-13)

**Situation:** Maria asked JB for an analyst + a HubSpot Specialist on her side. Both roles would hollow out John's Acquisition & Analytics scope under the proposed restructure.

**What I decided:** Hold the lines on A&A scope. Don't pre-stage org transitions or rewrite reporting until JB formalizes the restructure — treat all direct reports identically under the current org chart (memory `feedback_no_pre_staging_org_transitions.md`).

**Why:** If A&A becomes a real Director seat, it needs the analyst and the HubSpot capability to operate. Conceding either before the restructure formalizes makes the seat smaller than it needs to be.

### Going All-In on Claude Code

**Situation:** Was building dashboards and reports in Power BI (DAX + SQL). Workflow was slow, insights were limited to what I could visualize in a BI tool.

**What I decided:** Shifted primary analysis workbench to Claude Code with MCP connections to our SQL warehouse, GA4, ad platforms, and more.

**Why:** Claude Code lets me ask questions of the data conversationally, iterate faster, and generate insights that a dashboard template can't. The output is more insightful and the turnaround is dramatically faster. Power BI is now legacy for existing dashboards only.

---

## Decision Patterns (Self-Awareness)

**Strengths:**
- Fast decision-maker. Doesn't agonize or over-deliberate.
- Data-driven. Doesn't execute on untested assumptions.
- Willing to be wrong and update the model.

**Watch items:**
- Can shut down emotionally after negative outcomes instead of channeling energy productively.
- High internal locus of control can become stubbornness when the environment genuinely requires patience.
- Enneagram 7 stress pattern: scattered focus, escape into planning new things instead of finishing current things.
