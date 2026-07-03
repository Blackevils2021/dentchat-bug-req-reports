# dentchat-bug-req-reports

Private bug and req tracking repo for the FD Dentchat project. Testers file reports here; developers read and fix them.


## How to file a bug

1. Open this repo as an Obsidian vault.
2. Duplicate `bugs/templates/bug-report.md` into `bugs/open/`.
3. Rename the file: `BUG-NNN-short-description.md` (increment NNN from the last report).
4. Fill in every field. Paste screenshots into the note — Obsidian saves them to `attachments/` automatically.
5. Set `consult_first: true` if the bug is ambiguous or risky and you want a developer to review the approach before fixing.
6. Obsidian Git will commit and push on its timer. The bug is now visible to developers.

## Severity guide

| Level | Meaning |
|-------|---------|
| `critical` | Blocks core flow (payment, registration, login) — fix same day |
| `high` | Major feature broken, no workaround |
| `medium` | Feature degraded, workaround exists |
| `low` | Cosmetic or minor UX issue |

## Lifecycle

```
bugs/open/   →  developer fixes it  →  bugs/closed/
```

When a bug is resolved the developer sets `status: closed` and moves the file to `bugs/closed/`.

## Repo structure

```
dentchat-bug-req-reports/
├── bugs&reqs/
│   ├── templates/   → bug-report.md  (copy this to file a new bug)
│   ├── open/        → active bugs
│   └── closed/      → resolved bugs
├── attachments/     → screenshots (auto-managed by Obsidian)
├── docs/            → setup notes
└── README.md
```

## Linked project

Runner Portal source: `dentchat-frontend` (separate repo — testers do not have access).
