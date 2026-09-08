# Particular

**An evidence-led web design operating system for AI agents and human designers.**

Particular helps turn briefs, references, brand assets, client feedback, and implementation constraints into websites that feel specific to the organization they represent — not generic outputs wearing a brand color.

> **Do not maximize novelty. Maximize specificity.**

## What it does

Particular combines:

- factual truth vs. preference truth
- source authority and evidence weighting
- Brand / Reference / Client / Category / Project / Anti-DNA
- explicit design calibration
- visual-category identification
- information architecture and content hierarchy
- composition-before-components
- typography, imagery, iconography, and interaction systems
- responsive recomposition
- accessibility and performance
- implementation constraints
- SEO and generative discoverability fundamentals
- adversarial critique and quality gates
- client-selection learning and local iteration

## Ready-to-use skill

The canonical skill is [`SKILL.md`](SKILL.md).

For most AI agents, start by loading only that file. It is intentionally self-contained and can be used directly as project or agent instructions.

Use the optional focused modules only when the task needs extra depth:

```text
modules/discover.md   research and source audit
modules/dna.md        reference / brand / client DNA extraction
modules/concept.md    concept generation
modules/design.md     screen and system design
modules/build.md      production frontend implementation
modules/redesign.md   improve an existing experience
modules/critique.md   adversarial design review
modules/polish.md     local refinement without redesign
modules/contest.md    client-rating / selection intelligence
modules/scroll.md     justified scroll-driven interaction
```

### Minimal setup

Give the agent:

1. `SKILL.md`
2. the actual project brief / source documents
3. brand assets
4. relevant references or screenshots
5. existing product/code if applicable
6. known client feedback or selection signals

Then ask it to begin in the appropriate operating mode.

Example:

```text
Use Particular for this project.
Start in DISCOVER mode.
Treat the attached brief as the factual source of truth.
Treat the supplied references and client ratings as preference evidence.
Do not design until the source hierarchy, Project DNA, visual category,
design calibration, and design thesis are established.
```

## Core workflow

```text
Evidence
  ↓
Factual Truth + Preference Truth
  ↓
Brand DNA + Reference DNA + Client DNA + Category DNA
  ↓
Visual Category + Design Calibration
  ↓
Design Thesis + IA + Content Architecture
  ↓
Composition + Typography + Imagery + Interaction
  ↓
Responsive + Accessible + Performant Implementation
  ↓
Adversarial Critique + Quality Gates
  ↓
Iteration + Preference Learning
```

## Repository map

```text
SKILL.md                     Canonical self-contained skill
modules/                     Optional focused operating modes
docs/
  architecture.md            System structure
  methodology.md             End-to-end workflow
  evidence-model.md          Truth, weighting, and DNA extraction
  calibration.md             Explicit design-intensity model
  quality-gates.md           Definition of done
  agent-adapters.md          Cross-tool usage guidance
examples/
  project-dna.json           Portable project-state example
  brief-to-build.md          Example workflow
templates/
  project-intake.md          Intake template
  critique-report.md         Review template
CONTRIBUTING.md
CHANGELOG.md
LICENSE
```

## Design principle

A strong result should look and behave as if it was researched, strategized, art-directed, written, designed, tested, and engineered for this specific organization.

If you can swap the logo, company name, and palette and the same design works for an unrelated business, it is not resolved enough.

## Portability

Particular is intentionally tool-agnostic. The same Project DNA and decision logic can travel between design tools, coding agents, site builders, and human teams.

Project-specific decisions should live in the project context or Project DNA artifact — not inside the global skill.

## Status

Early public release. The current focus is web design and frontend experiences. The structure is intended to evolve through real project use, critique, and measured outcomes.

## License

MIT. See [LICENSE](LICENSE).
