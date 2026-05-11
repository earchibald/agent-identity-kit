---
project: agent-identity-kit
type: doc
doc_type: guide
status: draft
created: 2026-05-10
---

# Inbox & Journal Guide

Two lightweight systems for managing what the agent doesn't yet know and tracking what it does.

## The Inbox

A bucket for things the agent can't yet dispatch correctly:
- **Confusion** — user said something that doesn't connect to existing context
- **Ambiguity** — multiple plausible interpretations, unsure which
- **Missing context** — the agent suspects there's background it doesn't have
- **Stray thoughts** — "remind me about X," "I should look into Y"

### Setup

```
<vault-root>/<agent-home>/
├── inbox/
│   ├── README.md          ← explains the system
│   ├── 001-first-item.md  ← one concept per file
│   ├── 002-second-item.md
│   └── ...
└── archive/               ← processed items go here
```

### Format

Each inbox item is a numbered markdown file:

```markdown
# 001 — Topic

Brief description of the confusion, question, or thought.

**Status:** awaiting user input / awaiting pattern to emerge
```

### Triage

When the user is ready, batch-process the inbox. Each item gets:
1. Dispatched to the right location (corpus, journal, a project, a reminder, etc.)
2. Moved to `archive/` with a note of where it went
3. Pattern learned → future items in the same category go straight to the destination

## The Journal

Append-only session log. Structured, timestamped, linked. **Not read on every turn** — only when explicitly analyzing past work (saves tokens).

### Setup

```
<vault-root>/<agent-home>/
└── journal/               ← one file per session
```

### Format

```markdown
## 2026-05-10T20:15 — Session: Foundation

**What happened:**
- Created corpus documents
- Established the Inbox system
- Updated memory/persona

**Created files:**
- path/to/file.md — brief note on what and why

**Learned:**
- User's preferences, recurrent patterns, surprises
- What should go in memory vs skill vs just log

**Open questions / Inbox items:**
- Items needing user input
- Patterns still forming
```

### Rules

- **Append-only at runtime** — new entries are added, old ones never modified
- **Structured, not stream-of-consciousness** — what happened, what was created, what was learned
- **One file per session** — named `YYYY-MM-DD_<topic>.md`
- **Link to files** — reference documents, decisions, and related entries
