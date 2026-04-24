---
name: issue-reporting
description: Use this skill whenever the user wants to file, write, or fill out a bug report, issue report, or problem report. Trigger when someone says "report a bug", "log an issue", "something is broken", "write up this problem", "fill in the issue template", or shares details about a technical problem they want documented. Also trigger when a support agent or QA tester needs to capture issue details from a user. Even if the user doesn't say "issue report" explicitly, use this skill whenever they describe a bug or malfunction and seem to need it written up.
---

# Issue Reporting Skill

Helps users produce complete, well-structured issue reports by gathering required information and filling in the standard template.

## Steps

1. **Gather information** — Review what the user has already shared. Identify which of the 10 fields are missing or incomplete.
2. **Ask for gaps** — If key fields are missing (especially Summary, URL, Steps to Reproduce, Expected vs Actual), ask for them before drafting. Group questions to avoid back-and-forth.
3. **Fill the template** — Use the template in `assets/template.md`. Populate every section with the user's details. Leave a section blank or marked "Not provided" if the user doesn't have it.
4. **Infer priority if not stated** — If the user describes something that sounds critical (e.g., data loss, login failure, complete outage), suggest a priority and ask them to confirm.
5. **Output** — Present the filled report as a clean markdown block, ready to copy or save.

## Field guidance

| Field | Required? | Notes |
|---|---|---|
| Summary | Yes | One clear sentence |
| Page URL | Yes | Exact URL, not just "the dashboard" |
| Login state | Yes | Logged in/out + account if logged in |
| Browser details | Yes | Name, version, normal/incognito |
| Steps to reproduce | Yes | Numbered, specific |
| Expected vs Actual | Yes | Both sides needed |
| Screenshots | Recommended | Remind user to attach if not mentioned |
| Date & Time | Yes | Include timezone/country |
| Additional notes | Optional | Recurrence, affected users |
| Priority | Yes | Critical / High / Medium / Low |

## Priority definitions (use as a guide)

- **Critical** — System down, data loss, security issue, affects all users
- **High** — Core feature broken, major workflow blocked, affects many users
- **Medium** — Partial functionality broken, workaround exists
- **Low** — Minor UI glitch, cosmetic issue, edge case

## Template location

See `assets/template.md` for the full report structure to populate.
