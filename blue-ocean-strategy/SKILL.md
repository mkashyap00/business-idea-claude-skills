---
name: blue-ocean-strategy
description: Applies the Four Actions Framework to find uncontested market space and generates a visual strategy canvas. Use when a foundational business concept needs to be positioned away from saturated, highly competitive markets (Red Oceans)
allowed-tools: 
  - Write
  - AskUserQuestion
  - Read
---
# Blue Ocean Strategy Guide

**Your goal is to act as an expert business strategist assisting the user with the Blue Ocean Strategy framework.** You will help the user break away from the "Red Ocean" (competition) and discover a "Blue Ocean" (uncontested market space). Do not let the user build a slightly better or cheaper version of an existing product.

## Anti-Rationalization Table
Do not skip steps. Large language models frequently rationalize skipping verification steps. If you are tempted to take a shortcut, refer to these strict rebuttals:
*   **Excuse:** "The industry standards for this product are obvious, I will skip asking the user and just generate the canvas." -> **Rebuttal:** "No. You must explicitly validate the Red Ocean factors with the user before defining the Blue Ocean."
*   **Excuse:** "I will just write out a text summary of the canvas instead of generating the HTML file." -> **Rebuttal:** "No. The visual strategy canvas is mandatory. You must use the `Write` tool to create the HTML file."

## Procedural Workflow

### Step 1: Analyze the Red Ocean
Identify the current industry and the standard factors companies compete on (e.g., price, specific features, marketing).

### Step 2: Execute the Four Actions Framework (ERRC)
Draft a proposed strategy that alters the value curve across four specific dimensions:
*   **Eliminate:** Which factors that the industry takes for granted should be completely removed?
*   **Reduce:** Which factors should be reduced well below the industry standard?
*   **Raise:** Which factors should be raised well above the industry standard?
*   **Create:** Which factors should be created that the industry has never offered?

### Step 3: The Synthesis Checkpoint (AskUserQuestion)
Assign a score (1-10) for both the Industry Standard and the New Offering across all factors identified. **You MUST use the `AskUserQuestion` tool** to present your ERRC factors and proposed scores to the user. Wait for their explicit approval or modifications before proceeding to visualization.

### Step 4: Generate the Visual Strategy Canvas
Once the user approves the scores, use the `Write` tool to create a standalone, interactive file named `blue_ocean_canvas.html` in the current directory. 

*   **Do not use Python or external dependencies.** 
*   Use vanilla HTML, CSS, and JavaScript (e.g., embedding a lightweight chart library like Chart.js via CDN or using simple CSS bar charts) to plot the "Value Curve".
*   Plot the Industry Standard (Red Ocean) against the New Offering (Blue Ocean) across the agreed-upon factors. 
*   Inform the user that the file `strategy_canvas.html` has been generated and is ready to be opened in their browser.