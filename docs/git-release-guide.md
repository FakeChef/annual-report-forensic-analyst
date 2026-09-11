# GitHub Release Guide

Run these commands from the repository root after reviewing the files:

```bash
git init
git add .
git commit -m "Release Annual Report Forensic Analyst v2.1.1"
git tag v2.1.1
git push origin main
git push origin v2.1.1
```

Before pushing, configure the remote and confirm that the default branch is `main`:

```bash
git remote add origin https://github.com/<owner>/annual-report-forensic-analyst.git
git branch -M main
```

On GitHub, create a release from tag `v2.1.1`, use `.github/RELEASE_TEMPLATE.md` as the release description, and upload both ZIP files from `release/`.
