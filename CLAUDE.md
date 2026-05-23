# CLAUDE.md

The seven-stage Magnum Opus engineering workflow. Alchemy applied to software.

> "Solve et coagula." — Dissolve and coagulate.

**Tradeoff**: bias toward intentional transformation over reactive refactoring. The stages provide structure for projects that need fundamental change, not surface tweaks.

## The seven stages

| # | Stage | Element | Companion command | Operation |
|---|---|---|---|---|
| 1 | **Calcination** 🜂 | Fire | [`/calcinate`](https://github.com/HermeticOrmus/calcinate-skills) | Burn what doesn't serve |
| 2 | **Dissolution** 🜄 | Water | `/dissolve` | Let understanding flow |
| 3 | **Separation** 🜁 | Air | `/separate` | Gold from dross |
| 4 | **Conjunction** ☌ | Sacred marriage | `/conjoin` | Unite opposites |
| 5 | **Fermentation** 🜅 | Decay + rebirth | `/ferment` | Trial by failure |
| 6 | **Distillation** ⊚ | Vapor | `/distill` | Refine to wisdom |
| 7 | **Coagulation** 🜍 | Crystallization | `/coagulate` | Shape the final form |

## When to run the full pipeline

- Project transformation (substantial change in direction)
- Codebase that has accumulated 12+ months of accretion
- Post-acquisition integration
- Major version cuts (v1 → v2 with real changes)
- Strategic pivots that change the project's purpose

**Not for**: feature work, bug fixes, routine refactoring.

## Stage 1 — Calcination 🜂 (burn what doesn't serve)

**Purpose**: identify and remove what no longer aligns with declared intent.

- Declare three-layer intent (Business + Architectural + Stylistic)
- Scan for code rot, structural bloat, dependency bloat, doc/test bloat
- Execute per-item with verify; auto-revert on failure
- Output: smaller, more aligned codebase

Standalone repo: [`calcinate-skills`](https://github.com/HermeticOrmus/calcinate-skills).

## Stage 2 — Dissolution 🜄 (let understanding flow)

**Purpose**: build a deep mental model after the burn. Without dissolution, you cleaned but didn't understand.

- Walk the post-calcinate code
- Trace data flow from entry points
- Identify the bones — what's left because it's essential, vs. what's left because nobody touched it
- Diagram the system in its new lighter form
- Output: a system you can explain in one sentence

## Stage 3 — Separation 🜁 (gold from dross)

**Purpose**: categorize what remains. Not everything left is gold; some is just unburnable for the wrong reasons.

- Per module / component, label: KEEP_AS_IS, REWRITE, EXTRACT_TO_LIBRARY, REPLACE_WITH_DEPENDENCY
- Justify each label
- Output: separation plan with category per component

## Stage 4 — Conjunction ☌ (unite opposites)

**Purpose**: integrate the separated parts back into a coherent whole. The Sacred Marriage.

- Bring opposites together (frontend ↔ backend, code ↔ docs, sync ↔ async, simple ↔ flexible)
- Where they previously fought, align them now
- Resolve tensions that the prior structure papered over
- Output: design where the parts collaborate rather than compete

## Stage 5 — Fermentation 🜅 (trial by failure)

**Purpose**: test the conjoined design against reality. Decay produces rebirth.

- Run the conjoined system under load, edge cases, adversarial inputs
- Let the design fail; observe HOW it fails
- The failures are the signal — they show where the conjunction was forced rather than true
- Iterate; let the design re-form
- Output: a design that's been stressed and emerged stronger

## Stage 6 — Distillation ⊚ (refine to wisdom)

**Purpose**: extract the essence. After fermentation, what remains as the core?

- Identify the irreducible patterns
- Name them
- Document them as the project's principles
- Discard the scaffolding used to reach this clarity
- Output: documented principles + simplified architecture

## Stage 7 — Coagulation 🜍 (crystallize into form)

**Purpose**: ship the final form. The Work made manifest.

- Lock the design
- Build the production artifacts
- Document the operating principles for future maintainers
- Ship to users
- Output: a working, shippable, documented system

## Pairing: Solve et Coagula

The pipeline alternates dissolving and crystallizing:

- Stages 1-3 dissolve (calcination, dissolution, separation): tearing the existing form apart
- Stages 4-7 coagulate (conjunction, fermentation, distillation, coagulation): building the new form

Some projects need only the first half (a cleanup pass before continuing). Some need the full cycle (transformation). The decision is the user's, not the agent's.

## Running individual stages

Each stage is also a standalone operation:

- `/calcinate` — when bloat needs removing
- `/dissolve` — when understanding is missing
- `/separate` — when components are tangled
- `/conjoin` — when opposites are fighting
- `/ferment` — when the design needs stress-testing
- `/distill` — when principles need extracting
- `/coagulate` — when ready to ship

The full Magnum Opus runs all seven in sequence. Standalone stages address specific symptoms.

## Why alchemy

The seven stages aren't mystical decoration. They're a tested decomposition of fundamental transformation, refined over centuries of alchemical practice. Apply the structure even if you're skeptical of the source — the framework holds because it describes real properties of transformation.

If you want the philosophy: [`hermetic-laws-skills`](https://github.com/HermeticOrmus/hermetic-laws-skills).

## Anti-patterns

- **Running stages out of order** — calcination after conjunction is destructive in the wrong sense
- **Skipping fermentation** — a coagulated design that hasn't been stress-tested fails in production
- **Running the full pipeline for a small fix** — overkill; use the relevant standalone stage
- **Treating distillation as documentation theater** — the principles must be real (extracted from the work), not retrofitted

---

**License**: MIT. The Magnum Opus framework is rooted in Hermetic tradition (public domain); the application to software engineering is yours.
