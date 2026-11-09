<p align="center">
  <h1 align="center">Antigravity Game Studios</h1>
  <p align="center">
    Autonomous and collaborative game development studio architecture for Google Antigravity.
    <br />
    49 Specialized Agents &bull; 74 Engineering Skills &bull; 14 Architecture Rules &bull; 15 Lifecycle Hooks
  </p>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="MIT License"></a>
  <a href=".agents/agents"><img src="https://img.shields.io/badge/Agents-49%20Specialists-blueviolet" alt="49 Agents"></a>
  <a href=".agents/skills"><img src="https://img.shields.io/badge/Skills-74%20Workflows-green" alt="74 Skills"></a>
  <a href=".agents/rules"><img src="https://img.shields.io/badge/Rules-14%20Standards-red" alt="14 Rules"></a>
  <a href=".agents/hooks"><img src="https://img.shields.io/badge/Hooks-15%20Lifecycle-orange" alt="15 Hooks"></a>
  <a href="https://antigravity.google"><img src="https://img.shields.io/badge/Platform-Google%20Antigravity-4285F4?logo=google" alt="Built for Google Antigravity"></a>
  <img src="https://img.shields.io/badge/Engines-Godot%20%7C%20Unity%20%7C%20Unreal-black" alt="Supported Engines">
</p>

---

## Overview

Antigravity Game Studios converts an Antigravity pair-programming environment into a complete, structured game studio. Instead of relying on an unconstrained single agent session prone to architectural erosion, hardcoded magic values, and missing quality verification, this architecture establishes an industry-standard studio hierarchy.

Development is managed by 49 specialized agent personas operating across three tiers of authority, supported by 74 workflow skills, 14 directory-scoped coding standards, and 15 automated validation hooks.

---

## Table of Contents

- [Studio Architecture](#studio-architecture)
  - [Tier 1: Directors](#tier-1-directors)
  - [Tier 2: Department Leads](#tier-2-department-leads)
  - [Tier 3: Domain Specialists](#tier-3-domain-specialists)
  - [Engine Specialists](#engine-specialists)
- [Workflow Skills Catalog](#workflow-skills-catalog)
- [Collaboration Protocol](#collaboration-protocol)
- [Quality Verification: Run and Observe](#quality-verification-run-and-observe)
- [Project Configuration](#project-configuration)
- [Safety and Lifecycle Hooks](#safety-and-lifecycle-hooks)
- [Path-Scoped Architecture Rules](#path-scoped-architecture-rules)
- [Repository Structure](#repository-structure)
- [Getting Started](#getting-started)
- [Credits and License](#credits-and-license)

---

## Studio Architecture

The studio hierarchy organizes responsibilities across distinct operational tiers, enforcing clear separation of concerns, escalation paths, and review gates.

### Tier 1: Directors
Directorial agents hold executive authority over creative vision, engineering feasibility, production timeline, and visual style.
* **creative-director**: Highest creative authority. Maintains vision cohesion, core game pillars, and player psychological resonance. Model: Pro.
* **technical-director**: Highest engineering authority. Governs architecture, technical feasibility, performance budgets, and systems boundaries. Model: Pro.
* **producer**: Schedule, milestone, and scope management. Tracks velocity, feature trade-offs, and dependency pipelines. Model: Pro.
* **art-director**: Visual identity, palette governance, silhouette clarity, and asset fidelity standards. Model: Pro.

### Tier 2: Department Leads
Department leads translate directorial requirements into concrete specifications and enforce discipline standards.
* **game-designer**: Systems mechanics, player progression, interaction loops, and balance frameworks.
* **lead-programmer**: Code quality, architectural conformance, refactoring roadmaps, and PR approvals.
* **audio-director**: Acoustic landscape, adaptive music integration, and sound spatialization specs.
* **narrative-director**: World bible, character voice consistency, narrative branches, and dialogue tone.
* **qa-lead**: Test matrix planning, coverage thresholds, evidence verification, and gate sign-offs.
* **release-manager**: Platform packaging, build pipelines, store compliance, and patch governance.
* **localization-lead**: Translation pipelines, string extraction, RTL/CJK layout verification, and culturalization.

### Tier 3: Domain Specialists
Specialists execute technical and creative tasks within explicit domain boundaries:
* **Engineering**: `gameplay-programmer`, `engine-programmer`, `ai-programmer`, `network-programmer`, `tools-programmer`, `ui-programmer`.
* **Design and Art**: `systems-designer`, `level-designer`, `economy-designer`, `technical-artist`, `sound-designer`, `writer`, `world-builder`, `ux-designer`, `prototyper`.
* **Operations and Quality**: `performance-analyst`, `devops-engineer`, `analytics-engineer`, `security-engineer`, `qa-tester`, `accessibility-specialist`, `live-ops-designer`, `community-manager`.

### Engine Specialists
Dedicated engineering agent sets exist for the three major game engines:

| Engine | Lead Agent | Sub-Specialists |
|---|---|---|
| **Godot 4** | `godot-specialist` | `godot-gdscript-specialist`, `godot-shader-specialist`, `godot-csharp-specialist`, `godot-gdextension-specialist` |
| **Unity** | `unity-specialist` | `unity-dots-specialist`, `unity-shader-specialist`, `unity-addressables-specialist`, `unity-ui-specialist` |
| **Unreal Engine 5** | `unreal-specialist` | `ue-blueprint-specialist`, `ue-gas-specialist`, `ue-replication-specialist`, `ue-umg-specialist` |

---

## Workflow Skills Catalog

The repository provides 74 executable skills located in `.agents/skills/`. Each skill implements a specific game development procedure:

### Onboarding and Environment Setup
* `/start`: Guided onboarding for concept, stage detection, and configuration initialization.
* `/setup-engine`: Configures engine references, versions, and build tooling.
* `/project-stage-detect`: Audits codebase and artifacts to infer current production stage.
* `/adopt`: Onboards an existing external project into the studio workflow.
* `/settings`: Reads or writes configuration values in `project.yaml`.
* `/help`: Workflow navigator and next-action recommendation.

### Game Design and Systems
* `/brainstorm`: Structured conceptualization from themes, mechanics, or references.
* `/map-systems`: Dependency and interaction mapping across game mechanics.
* `/design-system`: Formal Game Design Document (GDD) authoring for specific subsystems.
* `/quick-design`: Lightweight mechanics tuning and small feature specifications.
* `/review-all-gdds`: Cross-document consistency, scope, and conflict auditing.
* `/propagate-design-change`: Analyzes downstream impact of mechanics alterations.

### Technical Architecture
* `/create-architecture`: Core architectural blueprint and module ownership specification.
* `/architecture-decision`: Formal Architectural Decision Record (ADR) generation.
* `/architecture-review`: Traceability and engine-compliance audit of existing codebase.
* `/create-control-manifest`: Input mapping, rebinding matrix, and input layer specification.

### Sprint and Story Execution
* `/create-epics`: Breaks high-level design milestones into functional epics.
* `/create-stories`: Generates granular user stories with explicit acceptance criteria.
* `/story-readiness`: Pre-development gate verification before implementation starts.
* `/dev-story`: Primary feature implementation and test authoring workflow.
* `/story-done`: Completion gate verification, including automated checks and visual review.
* `/sprint-plan`: Velocity-aware sprint backlog assembly.
* `/sprint-status`: Sprint progress tracking and bottleneck identification.
* `/estimate`: Complexity and risk scoring for proposed features.

### Quality Assurance and Analysis
* `/qa-plan`: Comprehensive verification plan covering logic, integration, and UI.
* `/smoke-check`: Fast automated health and compilation verification.
* `/regression-suite`: Full regression test orchestration.
* `/soak-test`: Extended-duration stability and memory leak detection.
* `/test-evidence-review`: Verifies screenshot, log, and profile evidence for closed stories.
* `/code-review`: Static analysis, safety, and performance evaluation.
* `/balance-check`: Mathematical validation of combat formulas and progression curves.
* `/perf-profile`: Hot-path analysis against frametime budgets.
* `/security-audit`: Save game integrity, memory manipulation, and networking security audit.
* `/tech-debt`: Debt register tracking and refactoring prioritization.

### Production and Release
* `/milestone-review`: Phase-gate assessment between production stages.
* `/vertical-slice`: Scoping and assembly guide for investor or publisher demo slices.
* `/bug-report`: Standardized defect tracking and reproduction capture.
* `/bug-triage`: Priority, severity, and department assignment for open defects.
* `/release-checklist`: Platform-specific pre-flight compliance check (Steam, Consoles, Itch).
* `/launch-checklist`: Day-of-launch deployment and monitoring schedule.
* `/changelog`: Automated commit-based release note generation.
* `/patch-notes`: Public player-facing release documentation.
* `/hotfix`: Emergency patch workflow with minimal blast radius.

### Cross-Functional Team Orchestration
Multi-agent coordination workflows that assemble required leads and specialists to solve compound tasks:
* `/team-combat`: Assembles `gameplay-programmer`, `game-designer`, `technical-artist`, and `sound-designer`.
* `/team-narrative`: Assembles `narrative-director`, `writer`, `level-designer`, and `audio-director`.
* `/team-ui`: Assembles `ui-programmer`, `ux-designer`, `art-director`, and `accessibility-specialist`.
* `/team-level`: Assembles `level-designer`, `world-builder`, `gameplay-programmer`, and `lighting-artist`.
* `/team-polish`: Assembles department leads for holistic feedback and juice pass.
* `/team-release`: Assembles `release-manager`, `lead-programmer`, `qa-lead`, and `devops-engineer`.
* `/team-audio`, `/team-live-ops`, `/team-qa`.

---

## Collaboration Protocol

Antigravity Game Studios strictly rejects unverified autonomous loops. Every non-trivial step adheres to the five-stage collaborative protocol:

```
Question -> Options -> Decision -> Draft -> Approval
```

1. **Question**: When ambiguity, design branching, or architectural choices arise, the agent queries the user rather than making assumptions.
2. **Options**: The agent presents 2 to 4 structured options, highlighting trade-offs across scope, performance, and aesthetic integrity.
3. **Decision**: The user selects the path or directs adjustments.
4. **Draft**: The agent generates a complete draft or changeset summary before modifying project files.
5. **Approval**: File write and edit operations require explicit user approval.

---

## Quality Verification: Run and Observe

A unit test passing does not prove that a game screen renders correctly. Antigravity Game Studios mandates the **Run and Observe** standard:

* Any user story that introduces or modifies visual elements, UI layout, camera behavior, or player controls is not considered complete until the project has been launched and observed.
* Visual verification evidence (screenshots, recordings, or telemetry logs) must be recorded in `production/qa/evidence/`.
* Code syntax validation or test execution alone cannot bypass this requirement.

---

## Project Configuration

Project parameters are declared in `project.yaml` at the repository root. This file serves as the single source of truth across all skills and agents.

```yaml
schema_version: 1

framework:
  name: Antigravity Game Studios
  version: 1.0.0
  platform: antigravity

# Configured during onboarding via /start or /setup-engine
engine:
  name: godot # godot | unity | unreal
  version: "4.3"

modes:
  rigor: minimal # minimal | standard | full
  automation: collaborative # collaborative | guided | autonomous
```

### Rigor Modes
* **minimal**: Jam-speed development. Waives formal GDD expansion, provides single-page briefs, minimal QA evidence overhead, and solo review.
* **standard**: Balanced commercial workflow. Requires core GDD sections, structured ADR records, standard QA evidence capture, and department lead reviews.
* **full**: Full studio rigor. Requires complete documentation matrices, architectural sign-offs from Directors, and exhaustive regression test evidence.

---

## Safety and Lifecycle Hooks

Hooks are declared in `.agents/hooks.json` and executed during agent lifecycle events:

* **PreToolUse (`run_command`)**: Runs `validate-commit.sh` and `validate-push.sh` to prevent accidental force pushes, commits containing unhandled TODOs, or invalid data JSON.
* **PreToolUse (`write_to_file`, `replace_file_content`)**: Runs `validate-registry.sh` and `validate-write.sh` to prevent unauthorized file clobbering and maintain ID registry integrity.
* **PreToolUse (`view_file`)**: Runs `validate-read.sh` to guard against loading oversized design documents into context.
* **PostToolUse (`write_to_file`, `replace_file_content`)**: Runs `validate-assets.sh` and `validate-skill-change.sh` to verify syntax and trigger linting passes.
* **Stop**: Runs `session-stop.sh` to archive current session state and record git activity.

---

## Path-Scoped Architecture Rules

Standards are automatically applied according to the file path being authored or reviewed:

| Target Path | Enforced Standard |
|---|---|
| `src/gameplay/**` | All parameters must originate from external data/config. Delta-time required for calculations. UI coupling prohibited (signals/events only). |
| `src/core/**` | Zero dynamic memory allocations in tick loops. Thread safety and strict API boundaries. |
| `src/ai/**` | Strict tick rate and memory budgets. Deterministic state transitions. |
| `src/networking/**` | Server-authoritative state logic. Packet payload serialization and versioning standards. |
| `src/ui/**` | UI elements must not hold source-of-truth game state. Localization ready. |
| `design/gdd/**` | Section completeness according to rigor level. Formula definitions and edge-case tables. |
| `design/narrative/**` | Canonical consistency, character vocabulary, and narrative tone guidelines. |
| `assets/data/**/*.json` | Schema adherence, schema validation, and snake_case naming. |
| `assets/shaders/**` | Instruction count limits, cross-platform shader compatibility, zero hardcoded uniforms. |
| `tests/**` | Clear separation between pure logic fixtures and scene presentation tests. |

---

## Repository Structure

```
.
├── .agents/
│   ├── agents/            # 49 specialized agent persona specifications
│   ├── docs/              # Templates (62), pipeline catalogs, and reference standards
│   ├── hooks/             # Lifecycle validation shell scripts
│   ├── rules/             # 14 path-scoped architectural rules
│   ├── scripts/           # 35 project analysis and state inspection scripts
│   ├── skills/            # 74 executable workflow skills
│   └── hooks.json         # Antigravity lifecycle hook definitions
├── design/
│   ├── gdd/               # Game design documents
│   └── narrative/         # World bible, character sheets, and dialogue trees
├── docs/
│   ├── architecture/      # Architecture blueprints and ADRs
│   └── engine-reference/  # Version references for Godot, Unity, and Unreal
├── production/
│   ├── epics/             # Production epics and stories
│   ├── milestones/        # Milestone criteria and reviews
│   ├── qa/evidence/       # Visual and execution test evidence
│   ├── session-state/     # active.md session checkpoint
│   └── sprints/           # Sprint backlogs and sprint reviews
├── src/                   # Game source code (configured per engine)
├── AGENTS.md              # Studio agent instructions
├── GEMINI.md              # Studio master manifesto and operational protocol
├── project.yaml           # Studio configuration store
└── README.md              # Studio documentation
```

---

## Getting Started

1. **Clone or copy this repository** into your game workspace.
2. **Open Google Antigravity** in the repository root directory.
3. Run the onboarding workflow in chat:
   ```text
   /start
   ```
4. The studio will inspect your project state, ask where you are beginning from (new concept, existing codebase, or prototype), and route you to the appropriate next steps.

---

## Credits and License

* Architecture and concept originally conceived by [Donchitos](https://github.com/Donchitos) for Claude Code Game Studios.
* Adapted, translated, and structured for Google Antigravity by [Marcello de Paiva](https://github.com/marcellopps283).
* Licensed under the [MIT License](LICENSE).
