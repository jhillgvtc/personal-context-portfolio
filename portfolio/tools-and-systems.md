# Tools and Systems

## Primary Workbench

**Claude Code** -- my main tool for data analysis, reporting, automation, and AI-assisted work. Connected to:
- **mssql MCP server** -- direct SQL queries against our data warehouse (Windows Auth, local sessions only)
- **Obsidian MCP** -- vault management, note capture, knowledge graph
- **Google Workspace CLI** -- email, calendar, Drive operations
- **Filesystem MCP** -- file operations across local and Drive paths
- **Meta Ads / Google Ads / GA4 / GSC MCP servers** -- campaign management and analytics

## Data Sources

| Source | What It Has | How I Access It |
|--------|-------------|-----------------|
| SQL Data Warehouse | Customer data, billing, service orders, product subscriptions, trouble tickets | mssql MCP or SSMS exports |
| iVUE Service (NISC) | Billing system -- the central nervous system of the company. Everything customer-related. | Direct UI + SQL warehouse |
| Google Analytics 4 | Website traffic, ecommerce conversions, user behavior | GA4 MCP or web UI |
| Google Ads | Paid search campaigns, performance data | Google Ads MCP or web UI |
| Meta Ads | Facebook/Instagram ad campaigns, lead gen | Meta Ads MCP or web UI |
| HubSpot | CRM, some marketing automation | Web UI (less frequent) |
| TRERC | Texas real estate/housing activity data (Comal County) | Playwright automation, monthly export |

## Other Daily Tools

- **Microsoft Teams** -- primary internal communication
- **Outlook** -- email (COM automation via Claude Code for reading/sending)
- **Power BI** -- legacy dashboards (DAX + SQL). Increasingly replaced by Claude Code for ad-hoc reporting.
- **SSMS (SQL Server Management Studio)** -- query writing and data export when not using MCP
- **Obsidian** -- personal knowledge management ("second brain"), PARA methodology
- **GitHub** -- version control for Claude Code projects, skills, and configurations
- **Todoist** -- task management, daily/weekly planning

## Evaluating / Exploring

- **Codex (terminal)** -- exploring as a second-opinion AI to check Claude Code's assumptions and catch over-agreeableness
- **Substack** -- building out Practical Machines publication for AI + telco thought leadership
- **LinkedIn** -- content platform for professional thought leadership
