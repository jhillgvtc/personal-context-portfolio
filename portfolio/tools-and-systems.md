# Tools and Systems

*Last updated: 2026-05-19*

## Primary Workbench

**Claude Code** — main tool for data analysis, reporting, automation, and AI-assisted work. Two surfaces:

1. **Red (local)** — Windows laptop with VPN + mssql + Drive vault access. All SQL/VPN/local-file work runs here regardless of subject.
2. **Atlas (EC2)** — OpenClaw on EC2 for 24/7 uptime, Slack delivery, public-internet tasks, cron-scheduled work, and Telegram pairing. Local `atlas/` is authoring-only; all operational changes happen on EC2 via SSH.

The split is by network access, not subject.

## MCP Servers

| MCP | Purpose | Notes |
|-----|---------|-------|
| **mssql** | Direct SQL queries against the GVTC data warehouse | Windows Auth, local sessions only. Silently caps at 10K rows; bypass via pyodbc for larger pulls. Blocks SUBSTRING/CONVERT as "obfuscation." |
| **HubSpot** | Live CRM, campaigns, workflows, contact-level identification | Preferred over web UI |
| **Obsidian** | Vault management, note capture, knowledge graph | Local REST API plugin |
| **Filesystem** | File operations across local and Drive paths | Fallback when Obsidian app is closed |
| **GA4** | Google Analytics 4 | CPAO framework via ga4-analyst skill |
| **Meta Ads / Google Ads** | Campaign management and analytics | |
| **Firecrawl** | Primary-source verification, scraping, structured extraction | Default for research subagents (not WebSearch+WebFetch) |
| **Notion** | Wave meeting notes, project pages | Patch-page for updates; create new pages manually |
| **CallRail** | Local custom MCP (TypeScript, built 2026-05-18) | Six tools: list_accounts, list_companies, list_tracking_numbers, list_calls, calls_summary, dump_audit_csvs |
| **Wave** | Wave.ai meeting fetch | Drives wave-meeting-sweep skill |
| **Todoist** | Task and project management | Workspace insights, productivity stats |
| **ec2-atlas SSH** | Atlas/OpenClaw operations on EC2 | All Atlas config/cron edits go through here |
| **vault-search** | Smart Connections embeddings bridge | 30K vectors, local MCP at `_system/vault-index/` |
| **Comet bridge / OpenCLI** | Authenticated-Chrome browser automation | Paywall research, live web sessions |
| **Playwright** | Browser automation for monthly exports (TRERC, etc.) | |
| **Outlook (COM)** | Direct read/draft via local desktop app | Faster and unbounded vs. Zapier round-trips |

## Data Sources

| Source | What It Has | How I Access It |
|--------|-------------|-----------------|
| SQL Data Warehouse | Customer data, billing, service orders, product subscriptions, trouble tickets | mssql MCP or SSMS exports |
| iVUE Service (NISC) | Billing system — the central nervous system of the company. Everything customer-related. | Direct UI + SQL warehouse |
| Google Analytics 4 | Website traffic, ecommerce conversions, user behavior | GA4 MCP or web UI |
| Google Ads | Paid search campaigns, performance data | Google Ads MCP or web UI |
| Meta Ads | Facebook/Instagram ad campaigns, lead gen | Meta Ads MCP or web UI |
| HubSpot | CRM, campaigns, workflows, contact-level identification | HubSpot MCP (preferred), web UI |
| CallRail | Call tracking, transcription, attribution | CallRail MCP (custom local build) |
| Wave.ai | Meeting recordings + transcripts | Wave MCP via wave-meeting-sweep |
| TRERC | Texas real estate/housing activity data (Comal County, neighbors) | Playwright automation, monthly export |
| FRED | Macroeconomic indicators (rates, employment, housing) | Standard API |

## GVTC Knowledge Surface

`3-resources/gvtc-context-profile/` — seven sub-profiles loaded on demand:
- `gvtc-financial-profile/` — P&L, OROIC, dividend programs, FY26 budget
- `gvtc-sales-marketing-profile/` — JB plan, sales capacity, Code Red, exposed base
- `gvtc-products-profile/` — SKUs, tiers, price-lock, channel lineup, MVNO
- `gvtc-footprint-profile/` — subdivisions, exchanges, rooftops, FTTH/HFC/DSL coverage
- `gvtc-competitor-profile/` — Spectrum, AT&T, Frontier, T-Mobile FWA, GVEC, BEAD
- `gvtc-cooperative-model-profile/` — MDP/CDP/Capital Credits, governance, 501(c)(12), Foundation
- `gvtc-glossary/` — vocabulary disambiguation

Audit skills:
- `telco-domain` — operator blind spots (churn denominators, gross vs net adds, ARPU mix, Simpson's paradox)
- `telco-finance-audit` — CFO-lens pressure test before any deliverable going to JB / finance / board

## Other Daily Tools

- **Microsoft Teams** — primary internal communication
- **Outlook** — email (COM automation via Claude Code for reading/sending)
- **Power BI** — legacy dashboards (DAX + SQL). Replaced by Claude Code for ad-hoc reporting; existing dashboards only.
- **SSMS (SQL Server Management Studio)** — query writing and data export when not using MCP
- **Obsidian** — personal knowledge management ("second brain"), PARA methodology. Vault mirror at `github.com/jhillgvtc/obsidian2026-vault`.
- **GitHub** — version control for Claude Code projects, skills, configurations, and this portfolio
- **Todoist** — task management, daily/weekly planning

## Evaluating / Exploring

- **Codex (terminal)** — exploring as a second-opinion AI to check Claude Code's assumptions and catch over-agreeableness
- **Substack** — building out Practical Machines publication for AI + telco thought leadership
- **LinkedIn** — content platform for professional thought leadership
