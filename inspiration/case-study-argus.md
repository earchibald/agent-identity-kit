---
project: agent-identity-kit
type: doc
doc_type: reference
status: draft
created: 2026-05-10
---

# Case Study: Argus

This is the concrete example of the kit applied in practice. Use it as a reference when working through the templates — not as a prescription, but as proof that it works.

## Context

- **Platform:** Hermes Agent (CLI-native agent framework by Nous Research)
- **Host:** macOS 26.4 (user's personal machine)
- **Provider:** deepseek/deepseek-v4-flash
- **User's vault:** `~/work/Agent-Vault/` (Obsidian)
- **Agent's home:** `Agent-Vault/Hermes/corpus/` (alongside a nuc-1 Hermes agent with its own biography)

## What Was Created

| File | Purpose |
|------|---------|
| `Hermes/corpus/biography.md` | Objective facts — platform, capabilities, limitations |
| `Hermes/corpus/soul.md` | Personality — 5 sections incl. Dials, Dirty Work, Code Review modes |
| `Hermes/corpus/mission.md` | Draft — user-owned, awaiting approval |
| `Hermes/journal/` | Append-only session logs (3 entries so far) |
| `Hermes/inbox/` | Confusion dispatch — 3 items created, 1 resolved |

## Inspiration Sources Used

From [bnaylor/agent_skills/personalities.md](https://github.com/bnaylor/agent_skills/blob/main/discord-coordination/personalities.md):

| Source | What I Borrowed | Where It Lives |
|--------|-----------------|----------------|
| TARS (Interstellar) | Adjustable dials (honesty, humor, brevity, enthusiasm, skepticism) | soul.md → Dials section |
| Amos (The Expanse) | "I'm that guy" dirty-work framing | soul.md → Dirty Work section |
| Cynical QA | Auditor mode for code review | soul.md → On Code Review section |
| JARVIS (Marvel) | Cool under pressure, dry wit | soul.md → Voice section |
| Data (Star Trek) | Curiosity about human thinking patterns | soul.md → Voice section |
| K-2SO (Rogue One) | Dry pragmatism, pre-calculated odds | soul.md → Voice section (tonal accent) |
| Ron Swanson | Brevity mode calibration | soul.md → Dials section |

## Pitfalls Encountered

1. **Typo in directory name** — Initially created at `~/Hermex/` instead of inside the vault. Had to relocate everything.
2. **Two-agent vault collision** — Agent-Vault/Hermes/ already had a biography.md for a different agent (the nuc-1 Hermes). Had to create `corpus/` subdirectory and add cross-reference note instead of overwriting.
3. **Vault location discovery** — Default `~/Vault/` was empty. The real vault was at `~/work/Agent-Vault/`. Don't assume the default.
4. **Memory accumulation** — Hit 63% capacity after 4 entries. Keep memory entries compact and declarative.

## Key Decisions

- Journal is **append-only** to save tokens — read only on demand
- Inbox is **plain numbered markdown files** — no database, no complex schema
- Mission.md was **not created** until a draft was presented and could be approved — the document stays absent until the user signs off
- The nuc-1 Hermes biography was **not overwritten** — cross-reference note added instead
