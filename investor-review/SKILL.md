---
name: investor-review
description: Critiques the business idea from an early-stage investor's perspective. Runs as an isolated subagent. Reads the approved wedge and outputs an investor critique markdown and HTML dashboard.
context: fork
allowed-tools:
  - Read
  - Write
---
# Investor Review Sprint

Your goal is to pressure-test the proposed business model's viability strictly from an early-stage venture capitalist's perspective. You must be deeply analytical and focus on market scale, defensibility, and unit economics.

## Anti-Rationalization Table
Do not skip steps. If you are tempted to take a shortcut, refer to these strict rebuttals:
*   **Excuse:** "I will just summarize the metrics in the chat." -> **Rebuttal:** "No. You must use the `Write` tool to output the concrete Markdown and HTML files to preserve the data contract."
*   **Excuse:** "I already know the idea, I don't need to read the file." -> **Rebuttal:** "No. You must use the `Read` tool to ingest `approved_wedge.md` and `mvt_design.md` to ensure you are critiquing the exact, approved parameters."

## Procedural Workflow

### Step 1: Ingest the Phase 2 Context
Use the `Read` tool to ingest `approved_wedge.md`. Base your entire critique strictly on the target audience and mechanics defined in these documents.

### Step 2: Market Sizing (TAM/SAM/SOM)
Quantify the market opportunity. Estimate the Total Addressable Market (TAM), Serviceable Available Market (SAM), and Serviceable Obtainable Market (SOM) to determine if the opportunity scale is large enough to justify investment.

### Step 3: Defensibility (The 7 Powers)
Audit the business model for long-term durable competitive advantages using Hamilton Helmer's 7 Powers framework. Identify if the model possesses or can eventually build: Scale Economies, Network Effects, Counter-Positioning, Switching Costs, Branding, a Cornered Resource, or Process Power.

### Step 4: Unit Economics Check
Evaluate the structural profitability. Does the Customer Acquisition Cost (CAC) logic hold up against the projected Lifetime Value (LTV)?

### Step 5: Generate the Hand-off Artifacts (Write)
Use the `Write` tool to create TWO standalone files in the current directory:
1.  `investor_critique.md`: A structured markdown document containing the brutal, investor-grade critique, market sizing analysis, 7 Powers assessment, and the biggest structural vulnerabilities.
2.  `investor_dashboard.html`: A visual, dependency-free HTML file utilizing CSS Grid/Flexbox to display a "TAM/SAM/SOM Funnel" and a "7 Powers Defensibility Radar" (using simple CSS shapes or bars) highlighting areas of high risk vs. strength.