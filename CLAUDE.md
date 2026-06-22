# ScaffoldX AU Brief — Routine Notes

## Email formatting

When creating the Gmail draft via `mcp__Gmail__create_draft`, always pass the brief as **HTML** using the `htmlBody` parameter. Do not use the plain `body` parameter alone — it strips all formatting.

Use the following HTML conventions:
- Section headings (`1. CULTURE & GENERAL` etc.) → `<h3>`
- Bullet lead-in labels (e.g. company names, signal titles) → `<strong>`
- Bullet points → `<ul><li>` lists
- Fit tags → `<strong>Fit: High</strong>` or `<strong>Fit: Medium</strong>`
- Section dividers → `<hr>`
- Also pass a plain-text `body` fallback for email clients that don't render HTML

## Brief file location

Save each brief to `briefs/YYYY-MM-DD.md` inside this repo, then commit and push to the active development branch before emailing.

## Avoiding repetition

Before writing, read the most recent file in `briefs/` to avoid repeating items from the previous day.
