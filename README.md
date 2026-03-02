# Tikanga — SaaS Essential Skills

Tikanga is an open-source library of role “skills” for running small SaaS companies with AI agents.

Each skill is a reusable, agent-friendly `SKILL.md` that turns a job function (PM, marketing, engineering, UX, etc.) into a consistent workflow with clear inputs, outputs, quality checks, and escalation points—so the agent stays useful instead of guessing.

Skills are plain Markdown (no runtime required). The collection focuses on the core capability areas most SaaS teams need: product, engineering, go-to-market, data/measurement, and user experience.

## Who this is for

- Founders and small teams who want repeatable, high-quality AI-assisted execution
- Agent builders who want a clean, standardized “skill” format to plug into their system

## What’s inside

Skills live under `skills/` (each skill is a folder containing a `SKILL.md`):

- `product-manager`
- `chief-product-officer`
- `software-engineer`
- `chief-technology-officer`
- `marketing`
- `chief-marketing-officer`
- `copywriter`
- `data-analyst`
- `prompt-engineer`
- `user-experience-designer`
- `user-researcher`

## Documents (templates)

The `documents/` folder contains reusable, generic SaaS templates you can fill in and adapt:

- `documents/brand-positioning-framework.md`: positioning worksheet (category, audience, value prop, differentiation, proof).
- `documents/go-to-market-gtm.md`: GTM plan template for a launch/expansion (messaging, enablement, timeline, success metrics).
- `documents/ideal-customer-profile-ICP.md`: ICP definition template (attributes, pains, outcomes, buying behavior, disqualifiers).
- `documents/market-research.md`: market research outline (TAM/SAM/SOM, trends, customer insights, competitive landscape, risks).
- `documents/marketing-strategy.md`: marketing strategy doc (revenue alignment, segment focus, channels, budget, quarterly priorities).

## Quick start

1. Clone the repo.
2. Point your agent/tooling at the `skills/` directory (or vendor the specific skills you want).
3. Invoke a skill by name and follow its “Inputs Needed” section before you draft.

Example prompt (tool-agnostic):

```text
Use the "copywriter" skill.
Goal: refine our README for a user-facing open-source project description.
Constraints: don’t invent proof points; keep it scannable.
Ask for any missing inputs before writing.
```

## Skill format (standardized)

Each `SKILL.md` follows a consistent structure designed for agent reliability:

- `Mission`: the one-line objective for the role.
- `Quick Workflow`: a repeatable step-by-step process.
- `Inputs Needed`: what to ask for first (to avoid guessing).
- `Outputs`: concrete artifacts to produce (briefs, specs, plans, copy, etc.).
- `Scope` / `Decision Authority` / `Interfaces`: ownership guardrails.
- `Quality Bar` + `Validation`: how to self-check work before shipping.
- `Definition of Done` + `Escalation Triggers` + `Anti-Goals`: when to stop, ask, or avoid failure modes.

## Repo layout (compatibility)

The canonical directory is `skills/`. For convenience, the repo also includes symlinks used by some agent setups:

- `.skills` → `skills`
- `.codex/skills` → `../skills`

## Contributing

Contributions are welcome—especially new roles, sharper workflows, and better output templates.

Guidelines:

- Prefer checklists, templates, and concrete outputs over narrative.
- Make assumptions explicit and add escalation triggers instead of guessing.
- Keep section names and order consistent across skills.

## License

MIT (see `LICENSE`).
