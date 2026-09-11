# Prompt Usage Guide

1. Install the Codex Skill.
2. Prepare one or more annual reports and record the company, period, and industry focus.
3. Run `forensic-analysis-prompt.md` in Single-Year or Multi-Year Forensic Mode.
4. Review evidence, source references, uncertainty, and Fact / Inference / Analyst View separation.
5. Run `pdf-report-generation-prompt.md` or `executive-slide-generation-prompt.md` separately after the research is complete.

Architecture: the Core Skill is the Research Engine; this prompt library is the Output Layer. Output prompts must not be used to change or bypass the core research rules.
