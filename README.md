# Annual Report Forensic Analyst

English | [中文](README_CN.md)

Version v2.1.2 · Apache License 2.0

## Overview

Annual Report Forensic Analyst is a research analysis engine for testing how companies create value and whether management narratives are supported by disclosed evidence. It is designed for annual reports, multi-year research, and executive communication.

The research chain is:

```text
Annual Report Evidence
        ↓
Business Model Reconstruction
        ↓
Management Narrative Testing
        ↓
Financial Reality Analysis
        ↓
Capital Allocation Review
        ↓
Future Success Assumptions
```

This is not an investment advice tool, stock recommendation tool, valuation model, or financial prediction engine. It does not provide buy/sell recommendations, stock ratings, target prices, valuation opinions, or unsupported forecasts.

## Research Workflow

```text
Annual Reports
        ↓
Annual Report Forensic Analyst
        ↓
Forensic Research Output
        ↓
Output Layer
        ↓
PDF Report / Executive Slides / Internal Briefing
```

The core skill generates analytical research. PDF and slide generation are separate output processes that transform completed research into a delivery format.

## Analytical Principles

Every conclusion separates:

- Fact: information directly disclosed in the source material.
- Inference: a reasoned interpretation based on disclosed facts.
- Analyst View: an independent assessment with stated limitations.

Management claims are treated as hypotheses to test, not conclusions to repeat.

## Modes

- Single-Year Forensic Mode: analyze one annual report.
- Multi-Year Forensic Mode: explain business model, narrative, financial, and capital allocation changes across years.
- Executive Slide Mode: convert research conclusions into evidence-led executive communication.

## Quick Start

Example: SAP, Multi-Year Forensic Mode, using the 2023, 2024, and 2025 annual reports.

```text
Analyze the following annual reports using Annual Report Forensic Analyst v2.1.1.

Company: SAP
Mode: Multi-Year Forensic Mode
Reports: 2023 Annual Report; 2024 Annual Report; 2025 Annual Report

Focus on:
1. Business model reconstruction
2. Value creation logic
3. Management narrative evolution
4. Evidence supporting management claims
5. Evidence challenging management claims
6. Financial reality
7. Capital allocation
8. Future success assumptions

Separate every conclusion into Fact, Inference, and Analyst View.
Do not provide investment recommendations, target prices, stock ratings,
or unsupported predictions.
```

Provide the annual reports as files or clearly identified source material. For Multi-Year Forensic Mode, provide comparable reports for the selected period and state any missing years, restatements, currency changes, or scope differences.

## Installation and Use

Codex users should download the Codex Skill Install Package from Releases and follow [INSTALLATION.md](INSTALLATION.md). Developers can clone this repository and review the framework, workflows, prompts, examples, and tests directly.

After the skill is installed:

1. Prepare one or more annual reports.
2. Choose Single-Year or Multi-Year Forensic Mode.
3. Use the forensic analysis prompt template.
4. Review evidence, uncertainty, and Fact / Inference / Analyst View separation.
5. Use the separate PDF or executive slide prompt only after the research is complete.

## Repository Structure

- `framework/`: core methodology and analytical principles
- `workflows/`: repeatable research processes
- `prompts/`: analysis and output-layer prompt templates
- `examples/`: public example guidance
- `tests/`: validation records
- `docs/`: repository and architecture documentation

## Limitations

This project is a research and reasoning framework, not investment advice. It does not provide investment recommendations, buy/sell recommendations, stock ratings, target prices, valuation opinions, financial forecasts, or certainty beyond the available evidence.

## License

Apache License 2.0. See [LICENSE](LICENSE) and [NOTICE](NOTICE).

## Version

Current release: v2.1.2
