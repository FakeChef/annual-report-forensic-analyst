# Installation — WorkBuddy Marketplace Edition

## Marketplace installation

1. Open WorkBuddy Marketplace and choose **Install from package** (or the equivalent local-package action).
2. Select `Annual_Report_Forensic_Analyst_v2.2.4_WorkBuddy_Edition.zip`.
3. Confirm the package name and version: `annual-report-forensic-analyst-workbuddy` / `2.2.4`.
4. Enable the skill for the workspace or conversation where annual-report files will be analyzed.
5. Start with a Marketplace shortcut or a custom request using the template in `SKILL.md`.

## Quick Start Prompt

```text
Use Annual Report Forensic Analyst — WorkBuddy Edition.
Company: {{Company}}
Mode: {{Single Year Forensic Mode or Multi Year Forensic Mode}}
Period: {{Period}}
Attach and analyze the supplied annual-report files as evidence. Separate conclusions into Fact, Inference, and Analyst View. Include sources, contradictions, limitations, and investigation questions. Do not provide investment advice, valuation opinions, ratings, target prices, or unsupported forecasts.
```

## First-use and output flow

Upload the reports, declare the company and period, choose a research mode, and review the completed forensic research before requesting a deliverable.

- PDF: `Convert the completed research into a source-traceable PDF-ready report.`
- Executive slides: `Convert the completed research into a 12-slide executive briefing with one evidence-led message per slide.`
- Infographic: `Convert the completed research into an evidence-led enterprise research infographic brief.`

Each output request must preserve source references, limitations, uncertainty, and Fact / Inference / Analyst View labels.

## Recommended Workflow

The **Research Engine** performs the evidence-led analysis and produces completed research. The **Output Layer** converts that research into PDF, executive slides, or an infographic brief. Use them in this order: **Research Engine → review evidence and uncertainty → Output Layer → human review**. Do not request the output layer before the research is complete unless you already have completed research to provide.

## Executive Slide Output Layer

After the Research Engine is complete, use `prompts/executive-slide-generation-prompt_EN.md` or `prompts/executive-slide-generation-prompt_CN.md`. Provide the company, analysis period, completed research output, audience, and presentation purpose. The prompt produces an adaptable executive storyline for CFO, CEO, or strategy use; it is not an annual-report summary, investment report, or decoration template.

## Terminology and review expectations

Forensic Analysis means evidence verification, not legal investigation. Fact / Inference / Analyst View separates disclosed facts, reasoned interpretations, and independent judgment with uncertainty. PDF, Slides, and Infographic are output-conversion layers: review the generated material before formal or external use; they are not investment advice or automatically approved decision documents.

## Manual installation

If WorkBuddy supports folder-based skills, unpack the ZIP and register the `workbuddy-edition/` folder. The manifest is `skill.json`; the entrypoint is `SKILL.md`.

## Source and provenance

This package is an independent adaptation layer based on Annual Report Forensic Analyst v2.1.2. It does not require modifying the base repository's `framework/`, `workflows/`, or `prompts/` directories. Keep the included Apache License 2.0 file with the package.

## First-run checklist

- Attach the annual-report source files.
- Declare the company and analysis period.
- Choose research mode before output mode.
- Ask for source locations, limitations, and Fact / Inference / Analyst View labels.
- Confirm that no investment recommendation, valuation, rating, target price, or unsupported forecast is requested.

## Packaging for release

From the repository root, package only `workbuddy-edition/` as:

`Annual_Report_Forensic_Analyst_v2.2.4_WorkBuddy_Edition.zip`

Do not include private annual reports or generated company deliverables in the Marketplace package.
