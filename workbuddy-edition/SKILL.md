---
name: annual-report-forensic-analyst-workbuddy
description: Evidence-based annual report research framework for enterprise research and management decision support, serving CFO, strategy, consulting, and general users; not legal investigation or investment advice.
description_zh: 基于证据的企业研究与管理层洞察框架，服务 CFO、战略、咨询和一般用户；不是法律调查或投资建议工具。
description_en: Evidence-based annual report research framework for enterprise research and management decision support, serving CFO, strategy, consulting, and general users; not legal investigation or investment advice.
version: 2.2.4
author: Annual Report Forensic Analyst contributors
category: research
license: Apache-2.0
---

# Annual Report Forensic Analyst — WorkBuddy Edition

Use this skill to turn one or more supplied annual-report files and related public disclosures into an evidence-led forensic research package in WorkBuddy.

This is an adaptation and routing layer for Annual Report Forensic Analyst v2.1.2. It does not replace, rewrite, or weaken the core framework, workflows, prompts, or analytical method. Treat management claims as hypotheses and preserve the distinction between Fact, Inference, and Analyst View.

## Supported modes

Choose one primary mode before analysis:

1. **Single Year Forensic Mode** — examine one annual report.
2. **Multi Year Forensic Mode** — explain changes across two or more comparable years; a three-year period is the default Marketplace shortcut.
3. **PDF Report Generation** — convert completed forensic research into a source-traceable PDF-ready report.
4. **Executive Slide Generation** — convert completed research into a concise executive deck outline or editable slide brief.
5. **Infographic Generation** — convert completed research into an evidence-led infographic brief with claims, evidence, uncertainty, and suggested visual encodings.

PDF, slides, and infographics are output modes. Run forensic research first unless the user supplies completed research.

## WorkBuddy operating contract

### Inputs

- Company and reporting period
- One or more annual-report files or clearly identified public source material
- Industry focus, if relevant
- Requested mode and deliverable
- Optional audience, language, page/slide count, and visual preferences

If source files are missing, ask for them. Do not invent figures, citations, company facts, or forecasts.

### Research behavior

- Reconstruct the business model and value-creation logic.
- Identify material management claims and test them against disclosed evidence.
- Surface supporting evidence, contradicting evidence, missing evidence, and remaining uncertainty.
- Address financial reality, cash conversion, capital allocation, changing success assumptions, risks, and investigation questions.
- Flag restatements, currency changes, reporting-scope changes, missing years, and comparability limits.
- Label each material conclusion as **Fact**, **Inference**, or **Analyst View**.
- Do not provide investment advice, buy/sell recommendations, ratings, target prices, valuation opinions, or unsupported forecasts.

### Output behavior

Return a structured result with:

1. Executive judgment
2. Business model and value creation
3. Management narrative and its evolution
4. Supporting and contradicting evidence
5. Financial reality and cash conversion
6. Capital allocation
7. Success assumptions and key risks
8. Monitoring dashboard and investigation questions
9. Sources, limitations, and unresolved uncertainty

For PDF, slides, or infographics, retain the same evidence traceability and labels. Make the output suitable for the requested audience without changing the underlying conclusions.

## Marketplace shortcut scenarios

- **三年年报分析**: Multi Year Forensic Mode for three comparable annual reports.
- **CFO汇报材料**: completed forensic research converted to Executive Slide Generation, emphasizing cash, capital allocation, risks, and monitoring.
- **PDF研究报告**: completed forensic research converted to a source-traceable PDF report.
- **企业研究信息图**: completed forensic research converted to a compact evidence-led infographic.

## Recommended WorkBuddy request template

```text
Use Annual Report Forensic Analyst — WorkBuddy Edition.

Company: {{Company}}
Mode: {{Single Year Forensic Mode | Multi Year Forensic Mode | PDF Report Generation | Executive Slide Generation | Infographic Generation}}
Analysis period: {{Period}}
Industry focus: {{Optional}}
Audience: {{Optional}}
Source files: {{Attached files}}

Separate every material conclusion into Fact, Inference, and Analyst View.
Show supporting evidence, contradicting evidence, limitations, and open investigation questions.
Do not provide investment advice, valuation opinions, ratings, target prices, or unsupported forecasts.
```

## Provenance and licensing

This WorkBuddy Edition is distributed under Apache License 2.0. Examples contain only anonymized structures and placeholders; they intentionally do not reproduce annual-report text, figures, tables, or company-specific conclusions.
