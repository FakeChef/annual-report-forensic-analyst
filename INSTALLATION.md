# Installation Guide

Annual Report Forensic Analyst v2.1.1 is distributed in two forms: a Codex runtime package and this GitHub repository.

## Codex Users

Download:

Annual_Report_Forensic_Analyst_v2.1.1_Codex_Skill_Install_Package.zip

Extract the release ZIP to:

`~/.codex/skills/`

Expected structure:

`annual-report-forensic-analyst/SKILL.md`

Restart Codex.

Verify:

`$annual-report-forensic-analyst`

## Developers

Clone repository:

git clone <repository-url>

Review:

- framework/
- workflows/
- prompts/
- tests/

The repository is the source of truth for methodology and documentation. The Codex package is intentionally smaller and contains only runtime instructions and metadata.
