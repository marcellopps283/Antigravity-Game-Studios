# Antigravity Game Studios -- Game Studio Agent Architecture

Indie game development managed through 49 coordinated Antigravity subagent personas and 74 specialized skills.
Each agent owns a specific domain, enforcing separation of concerns, high aesthetic standards, and engineering quality.

## Technology Stack

- **Engine**: [CHOOSE: Godot 4 / Unity / Unreal Engine 5]
- **Language**: [CHOOSE: GDScript / C# / C++ / Blueprint]
- **Version Control**: Git with trunk-based development
- **Build System**: [SPECIFY after choosing engine]
- **Asset Pipeline**: [SPECIFY after choosing engine]

> **Note**: Engine-specialist agents exist for Godot, Unity, and Unreal with dedicated sub-specialists. Use the set matching your engine.

## Studio Hierarchy

```text
Tier 1 — Directors (Creative, Technical, Producer, Art)
Tier 2 — Department Leads (Game Design, Lead Programmer, Audio, Narrative, QA, Release)
Tier 3 — Specialists (Gameplay, AI, Network, Engine, UI, Systems, Level, VFX, Tools, Writers)
Engine Specialists — Godot 4, Unity, Unreal Engine 5 dedicated experts
```

## Collaboration Protocol

**User-driven collaboration, not autonomous execution.**
Every task follows: **Question -> Options -> Decision -> Draft -> Approval**

- The agent MUST ask for approval before writing or editing files unless explicit path was agreed.
- The agent presents 2-3 strategic options when facing design dilemmas, explaining trade-offs.
- Multi-file changes require explicit confirmation of the changeset.
- No commits without explicit user instruction.
- **Run & Observe**: If an edit affects what the player experiences, run the game, observe, and save evidence in `production/qa/evidence/`.

## Configuration Store (`project.yaml`)

`project.yaml` at the repo root is the primary single source of truth: engine, specialists, naming conventions, platforms, and rigor modes (`minimal`, `standard`, `full`).

## Context & Session Memory

`production/session-state/active.md` is the active session checkpoint. Read it first after any `/clear`, compaction, or when resuming work.

## Directory Scoped Rules

- **Gameplay code** (`src/gameplay/`): All values MUST come from config/data files, never hardcoded. Delta time for all calculations. Decouple logic from UI via signals/events.
- **Engine code** (`src/core/`): High performance, zero allocations in tick loops.
- **Design docs** (`design/gdd/`): Modular, version-controlled markdown specs.
- **QA & Testing** (`tests/`): Unit test gameplay logic separately from presentation.
