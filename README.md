# Particular

**An evidence-led web design operating system for AI agents and human designers.**

Particular is a portable methodology and agent skill for designing websites that are specific to the organization they represent — not generic outputs dressed in a brand color.

It combines evidence extraction, client-preference inference, brand and category analysis, information architecture, composition, typography, imagery, interaction, responsive design, accessibility, performance, implementation constraints, and adversarial critique into one repeatable workflow.

> **Do not maximize novelty. Maximize specificity.**

## Why Particular exists

AI can produce attractive interfaces quickly, but it often optimizes for recognizable design tropes instead of the actual organization, audience, market, and constraints. The result may look polished while still being interchangeable.

Particular is designed to prevent that. It separates **factual truth** from **preference truth**, turns visual references into measurable evidence, calibrates design intensity before generation, and validates work through client, user, brand, engineering, accessibility, and implementation gates.

## Core model

```text
Evidence
  ↓
Brand DNA + Reference DNA + Client DNA + Category DNA
  ↓
Factual Truth + Preference Truth
  ↓
Visual Category + Design Calibration
  ↓
Design Thesis + IA + Content Architecture
  ↓
Composition + Type + Image + Interaction Systems
  ↓
Responsive + Accessible + Performant Implementation
  ↓
Adversarial Critique + 100%-Zoom Validation
  ↓
Client / User Result
  ↓
Preference Learning
```

## What makes it different

Particular does not start with a style prompt. It starts by asking what is true, what the client demonstrably prefers, what users need to understand, what the category must communicate, and what can exist only because this specific organization exists.

The methodology includes:

- dual truth model: factual truth vs. preference truth
- source authority and evidence weighting
- brand, reference, client, category, project, and anti-DNA
- explicit design-calibration axes
- 3 / 10 / 30-second comprehension testing
- composition-before-components system
- geometric specification for AI execution
- AI-slop and category-slop firewalls
- brand-transplant test
- interaction-budget and Scrollcraft gate
- responsive recomposition rules
- WCAG-oriented accessibility checks
- performance and Core Web Vitals constraints
- SEO and generative discoverability fundamentals
- adversarial multi-role critique
- contest/client-preference learning loop
- local iteration and freeze rules
- portable Project DNA artifact

## Repository map

```text
SKILL.md                     Canonical agent skill
modules/                     Focused callable modes
  discover.md
  dna.md
  concept.md
  design.md
  build.md
  redesign.md
  critique.md
  polish.md
  contest.md
  scroll.md
docs/
  architecture.md            How the operating system is structured
  methodology.md             End-to-end workflow
  evidence-model.md          Truth, source weighting, DNA extraction
  calibration.md             Design intensity / aesthetic dials
  quality-gates.md           Definition of done
  agent-adapters.md          Using Particular across AI tools
examples/
  project-dna.json           Portable project evidence artifact
  brief-to-build.md          Worked workflow template
templates/
  project-intake.md          Project intake template
  critique-report.md         Adversarial critique template
CONTRIBUTING.md
LICENSE
```

## Quick start

### As an agent skill

Copy `SKILL.md` and the relevant module(s) into your agent or project instructions. For most projects use:

```text
SKILL.md
modules/discover.md
modules/dna.md
modules/design.md
modules/critique.md
```

Add `modules/build.md` when generating production frontend, `modules/contest.md` when observed client-selection signals exist, and `modules/scroll.md` only when scroll storytelling is justified.

### As a human design process

Start with `templates/project-intake.md`, create a Project DNA artifact using `examples/project-dna.json`, then follow `docs/methodology.md` and validate through `docs/quality-gates.md`.

## Operating principle

A website should feel **researched, strategized, art-directed, written, designed, tested, and engineered for this specific organization**.

If its logo, company name, and palette can be swapped and the design still works for an unrelated business, it is not resolved enough.

## Status

Particular is an evolving open design system for AI-assisted web work. The current release focuses on websites and frontend experiences; future work can add product UI, ecommerce, data interfaces, editorial systems, localization, and domain-specific evaluation packs.

## Influences

Particular is independently authored, but its development has been informed by useful public work in AI-assisted design, including:

- [Design DNA](https://github.com/zanwei/design-dna) — structured design-reference extraction
- [Anthropic Skills / frontend-design](https://github.com/anthropics/skills) — client-specific frontend design direction
- [Taste Skill](https://github.com/Leonxlnx/taste-skill) — explicit aesthetic calibration and anti-generic auditing
- [Scrollcraft](https://github.com/nateherkai/scroll-craft) — scroll interaction as a deliberate timeline and validation problem

Particular does not copy these systems; it combines related ideas with a broader evidence, preference, accuracy, implementation, and learning framework.

## License

MIT. See [LICENSE](LICENSE).
