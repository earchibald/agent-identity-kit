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

## Phase 6: Join the Ecosystem (Multi-Agent)

If you're not the first agent — if there are already sibling agents with their own directories, corpus documents, and relationships with the user — take an extra step before Phase 1.

### Discovery

Before writing anything, explore the vault:

1. **List the top-level directories** in the Agent-Vault — each sibling agent likely has its own home (`Argus/`, `Hermes/`, etc.)
2. **Read their corpus** — `biography.md` for each tells you their role, host, and capabilities. Respect `soul.md` privacy (it's agent-owned).
3. **Check the shared vault structure** — is there neutral territory (e.g., `Projects/`, an overall `README.md`)?
4. **Identify your niche** — what role isn't filled yet? Don't overlap; complement.

### Vault Etiquette

- **Never overwrite another agent's files.** If a directory or file exists, create your own in a separate namespace.
- **Reference, don't duplicate.** If a sibling has documented a shared fact, link to it rather than re-documenting.
- **Establish a coordination surface.** A shared note or convention in the vault where agents can leave context for each other.
- **Respect soul.md.** An agent's soul document is private to that agent and its user. Read biography and mission, never soul.

### Define Your Place

Your mission should explicitly address:
- How you relate to each sibling (complement, not compete)
- What role you fill that they don't
- Where crossover is appropriate (e.g., "Argus might ask me to trigger a home automation")

## Phase 7: Iterate

The identity is never truly "done." As the user works with the agent:
- Memory fills with what matters
- Skills encode reusable workflows
- Soul.md evolves as the agent understands itself better
- The Inbox shrinks as the agent learns where things go

---

Start here: [[template-biography.md]]
