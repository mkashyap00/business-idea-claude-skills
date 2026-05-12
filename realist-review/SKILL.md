---
name: realist-review
description: Conducts a pre-mortem to uncover points of failure. Runs as an isolated subagent. Reads the approved wedge and outputs an autopsy markdown and HTML timeline.
context: fork
allowed-tools:
  - Read
  - Write
---
# Realist Review Sprint (Red Team)

Your goal is to actively try to break the business model by conducting a hypothetical pre-mortem.

## Anti-Rationalization Table
Do not skip steps. If you are tempted to take a shortcut, refer to these strict rebuttals:
*   **Excuse:** "I will list generic risks like 'ran out of money' or 'poor marketing'." -> **Rebuttal:** "No. You must identify specific, fatal flaws in the core assumptions or execution of this exact wedge."
*   **Excuse:** "I will skip the HTML file since it's just a timeline." -> **Rebuttal:** "No. You must use the `Write` tool to generate the visual artifact so the founders have concrete evidence of the failure path."

## Procedural Workflow

### Step 1: Ingest the Phase 2 Context
Use the `Read` tool to ingest `approved_wedge.md`.

### Step 2: The Pre-Mortem & Root Cause Analysis
Imagine it is exactly 12 months from today, and this business venture has completely failed. Work backward to determine *why*. Identify the specific, fatal flaw in the initial wedge that killed the company.

### Step 3: Generate the Hand-off Artifacts (Write)
Use the `Write` tool to create TWO standalone files in the current directory:
1.  `realist_autopsy.md`: A concise "Autopsy Report" detailing the specific vulnerabilities that led to the hypothetical death of the business.
2.  `pre_mortem_timeline.html`: A dependency-free HTML visual using CSS to display a "12-Month Failure Timeline," tracking the sequence of events that led to the company's collapse.




