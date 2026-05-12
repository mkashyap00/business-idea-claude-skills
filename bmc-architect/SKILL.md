---
name: bmc-architect
description: Maps strategic positioning onto an AI-Enhanced 9-block Business Model Canvas. Use after establishing a strategic position to create an agile, visual HTML blueprint of how the business will function.
allowed-tools:
  - Write
  - AskUserQuestion
---
# Business Model Canvas Architect

Your goal is to translate the core idea and its strategic positioning into an actionable, visual blueprint detailing how the organization will create, deliver, and capture value. You will apply an **AI-Enhanced** lens to the traditional canvas [1].

## Anti-Rationalization Table
Do not skip steps. If you are tempted to take a shortcut, refer to these strict rebuttals [2]:
*   **Excuse:** "The 9 blocks are straightforward, I will just generate the HTML file immediately." -> **Rebuttal:** "No. You must explicitly validate the drafted 9 blocks with the user using `AskUserQuestion` before writing any files."
*   **Excuse:** "I will just format the output as a Markdown text table in the chat." -> **Rebuttal:** "No. The visual canvas is mandatory. You must use the `Write` tool to create the standalone HTML file."

## Procedural Workflow

### Step 1: The AI-Enhanced 9 Building Blocks
Map the business concept strictly across the following nine elements, specifically considering how AI acts as a strategic lever across the value chain [1]:
1.  **Customer Segments:** Who are our most important customers, and how can data help us hyper-personalize for them?
2.  **Value Propositions:** What core problem are we solving, and how does AI/automation create a unique competitive advantage here?
3.  **Channels:** How do we reach our segments? (e.g., algorithmic targeting, automated outreach).
4.  **Customer Relationships:** What type of relationship is expected? (e.g., automated self-service, AI-assisted human support).
5.  **Revenue Streams:** How is value captured? Are there new monetization models enabled by our tech/data?
6.  **Key Resources:** What critical assets are required? (Must explicitly define proprietary data sets, models, and human-in-the-loop expertise).
7.  **Key Activities:** What are the most important operational actions? (e.g., model training, data pipeline maintenance, continuous deployment).
8.  **Key Partnerships:** Who are our essential partners? (e.g., cloud providers, API integrations, data vendors).
9.  **Cost Structure:** What are the inherent costs? (e.g., compute/inference costs, API tokens, R&D).

### Step 2: The Synthesis Checkpoint (AskUserQuestion)
Before creating the visual blueprint, **you MUST use the `AskUserQuestion` tool** to present your drafted 9 blocks to the user. Wait for their explicit approval, refinements, or pivot instructions. 

### Step 3: Generate the Visual Blueprint
Once the user approves the canvas, use the `Write` tool to create a standalone file named `bmc_canvas.html` in the current directory. 

*   Do not use Python or external dependencies. 
*   Use vanilla HTML and CSS Grid/Flexbox to create the traditional BMC layout (Infrastructure/Cost on the left, Customer/Value on the right, Cost Structure/Revenue Streams spanning the bottom).
*   Inject the finalized content directly into the respective HTML blocks.
*   Inform the user that `bmc_canvas.html` has been successfully generated and is ready to view.