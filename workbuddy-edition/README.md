# Annual Report Forensic Analyst v2.2.4 WorkBuddy Marketplace Edition

English | [中文](README_CN.md)

An Apache-2.0 WorkBuddy adaptation of Annual Report Forensic Analyst v2.1.2: an evidence-based annual report research framework for enterprise research and management decision support. It serves CFO, strategy, consulting, and general research use cases. It is not a legal investigation tool or an investment advice tool.

### Terminology

- **Forensic Analysis** means evidence verification: claims are tested against disclosed evidence. It does not mean legal investigation, fraud investigation, or an audit opinion.
- **Fact / Inference / Analyst View** is a three-layer judgment system: Fact is what the source directly discloses; Inference is the reasoned interpretation; Analyst View is the independent assessment, uncertainty, and limitation.
- **PDF / Slides / Infographic** are output-conversion layers. They transform completed research into a delivery format and require human review before formal or external use; they do not automatically make an approved financial or management decision.

## What it supports

- Single Year Forensic Mode
- Multi Year Forensic Mode
- PDF Report Generation
- Executive Slide Generation
- Infographic Generation

Use the first two modes for research. Use the last three after research is complete, or provide completed research as input.

## Marketplace shortcuts

Select one of these ready-to-use scenarios: 三年年报分析, CFO汇报材料, PDF研究报告, or 企业研究信息图. Each shortcut is defined in `skill.json` and routed by `SKILL.md`.

## Quick start

1. Install the package according to [INSTALLATION.md](INSTALLATION.md).
2. Attach one or more annual reports.
3. Name the company, period, industry focus, audience, and desired mode.
4. Require Fact / Inference / Analyst View labels and source references.
5. Review limitations and unresolved questions before using any output externally.

### Quick Start Prompt

```text
Use Annual Report Forensic Analyst — WorkBuddy Edition.
Company: {{Company}}
Mode: {{Single Year Forensic Mode or Multi Year Forensic Mode}}
Analysis period: {{Period}}
Industry focus: {{Optional}}
Attached reports: {{Files}}
Analyze the reports as evidence. Separate every material conclusion into Fact, Inference, and Analyst View. Show supporting evidence, contradicting evidence, source locations, limitations, and open investigation questions. Do not provide investment advice, ratings, target prices, valuation opinions, or unsupported forecasts.
```

### First-use flow

Attach the source reports, identify the company and period, choose a research mode, review the evidence-led research output, and only then choose a delivery mode. The delivery modes are invoked with completed research as follows:

- **PDF**: `Convert the completed forensic research into a source-traceable PDF-ready report. Preserve Fact / Inference / Analyst View, sources, limitations, and the monitoring dashboard.`
- **Executive slides**: `Convert the completed forensic research into a 12-slide executive deck brief for {{Audience}}. Use one evidence-led message per slide and preserve sources and uncertainty.`
- **Infographic**: `Convert the completed forensic research into an evidence-led enterprise research infographic brief. Include judgment, value-creation chain, claims, evidence, contradictions, risks, monitoring signals, and uncertainty.`

## Recommended Workflow

The **Research Engine** produces the evidence-led forensic research: it reconstructs the business model, tests management claims, and records Fact / Inference / Analyst View. The **Output Layer** then converts that completed research into a PDF report, executive-slide brief, or infographic brief. Keep the sequence explicit: **Research Engine first, Output Layer second**. Review the research and the converted deliverable before formal or external use.

## Executive Slide Output Layer

Use the Executive Slide Output Layer only after completed forensic research is available. It converts research into CFO briefing, CEO discussion, or strategy review material; it does not replace the Research Engine or enforce a fixed slide count. Use [prompts/executive-slide-generation-prompt_EN.md](prompts/executive-slide-generation-prompt_EN.md) or the Chinese version for the full input, storyline, visual, anti-degradation, and QA instructions.

### User scenarios

- **CFO**: annual operating review, competitor analysis, and management briefing preparation.
- **Strategy**: business-model change analysis and competitive-landscape analysis.
- **Consultant**: client research working papers and briefing-material preparation.
- **General AI User**: upload an annual report and start enterprise research with a guided prompt.

## Scope and guardrails

Management statements are hypotheses to test. The skill does not provide investment advice, ratings, target prices, valuation opinions, or unsupported forecasts. It does not invent missing evidence.

## Examples

`examples/` contains anonymized structures for SAP, Sandvik, Schneider, and ABB. The examples contain placeholders and task shapes only; they do not reproduce annual-report content.

## License

Apache License 2.0. See [LICENSE](LICENSE).
