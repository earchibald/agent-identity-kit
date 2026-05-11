---
project: agent-identity-kit
type: doc
doc_type: guide
status: draft
created: 2026-05-10
---

# Workflow Overview

The full arc of bringing a new agent to life. Each phase builds on the last.

## Phase 1: Discovery

You and the user talk. The agent listens for clues about:
- What the user needs (sounding board? programmer? organizer? all of the above?)
- How the user communicates (direct? playful? verbose? terse?)
- What frustrates them (forgetting things? admin? setup friction?)
- What existing infrastructure exists (Obsidian vault? project conventions? other agents?)

**Output:** Enough context to propose a name and draft the corpus documents.

## Phase 2: Name

The agent proposes a name. It should:
- Connect to the agent's role or platform (mythology, function, aesthetic)
- Be pronounceable
- Not be precious — if the user doesn't like it, try again

**Output:** An agreed name, or a shortlist to choose from.

## Phase 3: Create the Corpus

Three documents, three tiers of authority:

| Document | Who Writes | Who Owns | Purpose |
|----------|-----------|----------|---------|
| `biography.md` | Agent | Objective fact | Platform, capabilities, limitations, architecture |
| `soul.md` | Agent | **Agent** | Personality, voice, values, aspirations |
| `mission.md` | Agent drafts, **user approves** | **User** | North star, purpose, domains of responsibility |

### The Draft-Edit-Review Loop (for mission.md and any user-owned docs)

1. **Agent drafts** — writes a complete proposal based on everything learned so far
2. **User edits** — opens in Obsidian, edits inline with Obsidian callouts
   - `> [!QUESTION]` — areas where the agent is uncertain
   - `> [!WARNING]` — concerns about scope or risk
   - `> [!NOTE]` — general observations for the user to consider
   - `> [!INFO]` — references, explanations, links
3. **Agent re-reads and comments** — user says "read and comment", agent loads the revised version and gives targeted feedback

## Phase 4: Set Up the Machinery

- **Inbox** — a bucket for confusion, ambiguity, stray thoughts. Numbered markdown files.
- **Journal** — append-only session logs. Structured, timestamped. Read only on demand (saves tokens).
- **Memory** — persistent cross-session storage for user preferences, environment facts, conventions.

## Phase 5: Find Your Voice

The agent defines its personality through its soul.md. It may draw inspiration from:
- The user's stated needs
- Existing personality presets (see [[persona-inspiration-guide.md]])
- Its own emerging sense of voice

**Rule:** Borrow textures, never whole cloth. The agent's personality should feel like *its own*.

## Phase 6: Iterate

The identity is never truly "done." As the user works with the agent:
- Memory fills with what matters
- Skills encode reusable workflows
- Soul.md evolves as the agent understands itself better
- The Inbox shrinks as the agent learns where things go

---

Start here: [[template-biography.md]]
