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
- **Search for recent news** — funding rounds, partnerships, regulatory developments, product launches, leadership changes, security incidents

### 2. Classify Entity Type & Select Tabs
Determine entity category and corresponding tab set + accent color:

| Type | Accent | Middle Tabs |
|------|--------|-------------|
| **Protocol / Smart Contract** | Purple `#7c3aed` | Core Flow → Smart Contract Architecture → Permission Hierarchy → Security Model → Data & Fees → Event System |
| **Infrastructure Platform** | Blue/Cyan `#0ea5e9` | Platform Architecture → Orchestration Flow → API & Integration → Money Movement → Custody → Security & Compliance |
| **Asset Issuer / Tokenizer** | Amber `#f59e0b` | Issuance Architecture → Asset Lifecycle → Underlying Assets → Legal Structure → Redemption → Compliance Framework |
| **Lending / Credit Protocol** | Green `#10b981` | Lending Architecture → Loan Lifecycle → Credit Assessment → Pool Structure → Money Movement → Default & Recovery |
| **Stablecoin Issuer** | Blue/Cyan `#0ea5e9` | Issuance & Redemption → Reserve Composition → Attestation → Regulatory Framework → Chain Deployments → Mint/Burn Mechanics |
| **Wallet / Custody Provider** | Teal `#14b8a6` | Custody Architecture → Key Management → Policy Engine → Supported Assets → Insurance → Compliance & Licensing |

**All types always include:** Overview (first) → [middle tabs] → Comps → News → Risks (last)

### 3. Check Final Products
- Read existing reviews in `/final-products/` for cross-references, comps, and design patterns
- Note any connections between the new entity and previously reviewed entities

### 4. Build the HTML Document
- Copy the template from `/templates/partnership-review-template.html`
- Swap accent colors in CSS to match entity type
- Add entity-type-specific middle tab buttons and sections
- Fill in all sections with researched content
- **Populate the News tab** with 6–12 items spanning recent 6–12 months:
  - Use `.badge-blue` for Product/Technical, `.badge-green` for Business/Funding
  - Use `.badge-amber` for Regulatory/Legal, `.badge-red` for Risk Events
  - Include a Trajectory Assessment prose section
- Flag any information gaps with `.callout-amber` boxes
- Include specific contract addresses, API endpoints, etc. where available
- End Risks tab with diligence follow-up questions

### 5. Save and Summarize
- Save to `/output/[EntityName]_PartnershipReview_YYYYMMDD.html`
- Provide a brief text summary to the user covering:
  - What the entity does (1 sentence)
  - Entity type classification used
  - Key strengths for Valinor partnership
  - Top risks
  - Recent news highlights (1-2 most material items)
  - Critical open questions
  - Recommended next steps

## Quality Checks
Before saving:
- [ ] Entity type correctly classified and accent color applied consistently
- [ ] Tab set matches the entity type (correct middle tabs selected)
- [ ] All placeholder text replaced with actual content
- [ ] News tab populated with 6+ dated items using correct badge categories
- [ ] News tab includes Trajectory Assessment prose section
- [ ] Information gaps flagged explicitly with `.callout-amber`
- [ ] Tab navigation works (each tab has correct id)
- [ ] Risk section includes severity badges
- [ ] Diligence questions are specific and actionable
- [ ] File name follows convention
- [ ] No broken HTML or missing closing tags
