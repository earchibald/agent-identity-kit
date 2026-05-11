# Agent Identity Kit

A reusable template pack for bringing a new AI agent to life — defining who it is, how it communicates, and how it learns its user over time.

Not a god, but gods together. This is the *pattern* for creating an agent's identity, not any one agent's particular identity.

## Contents

```
agent-identity-kit/
├── DOCS/
│   ├── workflow-overview.md           ← 6-phase arc from discovery to iteration
│   ├── template-biography.md          ← objective facts (__PLACEHOLDER__)
│   ├── template-soul.md               ← personality and voice (prompts, not prescription)
│   ├── template-mission.md            ← north star (draft → user edits via Obsidian callouts)
│   ├── inbox-journal-guide.md         ← dispatch + logging system setup
│   └── persona-inspiration-guide.md   ← texture library + what-not-to-borrow
├── inspiration/
│   └── case-study-argus.md            ← worked example of the kit in practice
├── STATUS.md                          ← project metadata (for Obsidian op integration)
└── agent-identity-kit.base            ← Obsidian Bases dashboard
```

## How to Use

1. **Read the workflow overview** — `DOCS/workflow-overview.md` covers the full arc
2. **Start with biography** — `DOCS/template-biography.md` — objective facts about the agent
3. **Move to soul** — `DOCS/template-soul.md` — personality, voice, values (agent-owned)
4. **Establish mission together** — `DOCS/template-mission.md` — requires user approval, uses Obsidian callout editing workflow
5. **Set up the machinery** — `DOCS/inbox-journal-guide.md` — Inbox + journal system
6. **Find your voice** — `DOCS/persona-inspiration-guide.md` — borrow textures from existing personas

All templates use `__PLACEHOLDER__` values. Replace them with your agent's own.

## Philosophy

- **Three tiers of authority:** biography (objective fact), mission (user-owned), soul (agent-owned)
- **Borrow textures, never whole cloth:** the agent's personality should feel like its own
- **The Inbox is honest:** confusion is raw material, not a bug
- **Journals are append-only:** save tokens by not reading them every turn
- **Iterate forever:** the identity is never truly done

## Example

See `inspiration/case-study-argus.md` for a worked example — the Argus agent was built using this exact kit on macOS with Hermes Agent, and the case study shows each decision and its rationale.

## License

MIT — use freely, share freely, adapt freely.
