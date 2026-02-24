# Skill: Partnership Review

## Trigger
User provides information about a company, protocol, or counterparty and asks for a review, analysis, or evaluation.

Trigger phrases:
- "Review [entity] as a partner"
- "Evaluate [entity]"
- "Analyze [entity] for us"
- "What do you think about [entity]?"
- "Create a partnership review for [entity]"
- "Do a deep dive on [entity]"

## Process

### 1. Gather Information
- Read any uploaded files or documents
- Search the web for additional context (documentation, press releases, funding, team)
- Check blockchain explorers for on-chain data if applicable
- Review GitHub repos if technical
- Note the entity type to select accent color

### 2. Classify Entity Type
Determine accent color based on entity category:
- **Payments/Stablecoins** → Blue/Cyan (#00d4ff)
- **Protocols/DeFi** → Purple (#8b5cf6)
- **Lending/Credit** → Green (#10b981)
- **Asset Management** → Amber (#f59e0b)
- **Risk/Insurance** → Red/Rose (#f43f5e)
- **Data/Analytics** → Teal (#14b8a6)

### 3. Determine Relevant Tabs
Always include: Overview, Risks
Include if relevant: Tech Stack, Core Flow, Money Movement, Roles & Access, Security, Comps
Add custom tabs if the entity warrants it (e.g., "Tokenomics", "Deal History", "Integration Guide")

### 4. Build the HTML Document
- Copy the template from `/templates/partnership-review-template.html`
- Customize the accent color in CSS `:root` variables
- Fill in all sections with researched content
- Flag any information gaps with `.callout-amber` boxes
- Include specific contract addresses, API endpoints, etc. where available
- End Risks tab with diligence follow-up questions

### 5. Save and Summarize
- Save to `/output/[EntityName]_PartnershipReview_YYYYMMDD.html`
- Provide a brief text summary to the user covering:
  - What the entity does (1 sentence)
  - Key strengths for Valinor partnership
  - Top risks
  - Critical open questions
  - Recommended next steps

## Quality Checks
Before saving:
- [ ] All placeholder text replaced with actual content
- [ ] Accent color applied consistently
- [ ] Information gaps flagged explicitly
- [ ] Tab navigation works (each tab has correct id)
- [ ] Risk section includes severity badges
- [ ] Diligence questions are specific and actionable
- [ ] File name follows convention
- [ ] No broken HTML or missing closing tags
