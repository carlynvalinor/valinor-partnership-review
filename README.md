# Valinor Partnership Review Analyst

A Claude Code agent that produces institutional-grade HTML research documents for evaluating potential partners, counterparties, and infrastructure providers.

## What It Does

Give this agent information about any company, protocol, or counterparty — from uploaded files, API docs, GitHub repos, press releases, news, or verbal descriptions — and it produces a **single self-contained HTML reference document** in the Valinor dark-theme research format.

Each document includes tabbed navigation, visual flow diagrams, info cards, role/access analysis, comparison tables, risk ratings, and structured prose — ready for credit committee review or team circulation.

## Quick Start

1. Open this project directory in Claude Code:
   ```
   cd valinor-partnership-review
   claude
   ```

2. Tell the agent what you want reviewed:
   ```
   Review Maple Finance as a potential lending partner.
   Here's their docs: https://docs.maple.finance
   ```

3. The agent will research, analyze, and produce an HTML file in `/output/`.

4. Open the file in any browser to review.

## Directory Structure

```
/output/                  - Generated review documents (HTML)
/templates/               - Base HTML template (do not modify)
/examples/                - Example completed reviews for reference
/raw-inputs/              - Place uploaded files, PDFs, data here
/.claude/                 - Agent configuration
  /skills/                - Specialized analysis workflows
  /comms/                 - Valinor messaging guide
  /output-styles/         - Output formatting rules
```

## Document Format

Every review document uses the same design system:

- **Dark theme** (#0a0a0f background) with entity-specific accent colors
- **Tabbed interface** with 8 standard tabs (Overview, Tech Stack, Core Flow, Money Movement, Roles & Access, Security, Comps, Risks)
- **Component library**: flow diagrams, info cards, role cards, sequence tables, security layers, badges, callout boxes, code blocks
- **Valinor evaluation lens**: always framed through institutional credit, regulatory clarity, and transparent money movement

## Accent Color Guide

| Entity Type | Color | Hex |
|-------------|-------|-----|
| Payments / Stablecoins | Blue/Cyan | `#00d4ff` |
| Protocols / DeFi | Purple | `#8b5cf6` |
| Lending / Credit | Green | `#10b981` |
| Asset Management | Amber | `#f59e0b` |
| Risk / Insurance | Red/Rose | `#f43f5e` |
| Data / Analytics | Teal | `#14b8a6` |

## Example Input Types

- "Review Circle/USDC as settlement infrastructure"
- "Evaluate Maple Finance for loan origination partnership"
- "Analyze Fireblocks as our custody provider"
- "Here's the Centrifuge docs — what's the architecture?"
- [Upload a PDF pitch deck] "Review this as a potential counterparty"

## Tips

- The more specific information you provide, the better the output
- The agent will flag information gaps explicitly rather than guessing
- Open the HTML files directly in a browser — they're fully self-contained
- Each review ends with recommended diligence follow-up questions
