# 🐛 Issue Reporting Skill for Claude

A Claude skill that helps users and support agents produce complete, structured bug reports using a standardized 10-field template.

## What it does

When someone describes a bug or asks to file an issue, Claude will:
- Identify missing information and ask for it
- Fill in the full report template automatically
- Suggest a priority level based on severity
- Output a clean, copy-ready report

## Trigger phrases

This skill activates when you say things like:
- "Report a bug"
- "Log an issue"
- "Something is broken on..."
- "Fill in the issue template"
- "Write up this problem"

## Template fields

| # | Field | Required |
|---|-------|----------|
| 1 | Summary of the Issue | ✅ |
| 2 | Page URL | ✅ |
| 3 | Login State | ✅ |
| 4 | Browser Details | ✅ |
| 5 | Steps to Reproduce | ✅ |
| 6 | Expected vs. Actual Behavior | ✅ |
| 7 | Screenshots / Screen Recordings | Recommended |
| 8 | Date & Time of Occurrence | ✅ |
| 9 | Additional Notes | Optional |
| 10 | Priority | ✅ |

## Installation

1. Download `issue-reporting.skill`
2. Go to Claude's skill settings
3. Upload the `.skill` file

## File structure

```
issue-reporting-skill/
├── SKILL.md          # Skill instructions and field guidance
└── assets/
    └── template.md   # The report template Claude fills in
```

## Priority levels

| Level | When to use |
|-------|-------------|
| 🔴 Critical | System down, data loss, security issue |
| 🟠 High | Core feature broken, major workflow blocked |
| 🟡 Medium | Partial issue, workaround exists |
| 🟢 Low | Minor UI glitch, cosmetic or edge case |

## License

©Nishtha Pradhan
