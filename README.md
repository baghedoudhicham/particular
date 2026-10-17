# Particular

**Evidence-led web design for AI agents.**

> Do not maximize novelty. Maximize specificity.

Particular is an open-source design operating system for AI-assisted web work. It helps agents and designers research, art-direct, critique, redesign, and implement websites that are specific to the product, brand, audience, and category—not interchangeable AI output.

It is designed to travel across **ChatGPT / Codex, Claude / Claude Code, Google AI Studio / Gemini, Stitch, Cursor, Lovable, Figma, and other agent environments**.

## Why Particular

AI can produce polished UI quickly, but speed amplifies weak judgment too. Common failure modes include generic SaaS composition, invented proof, category clichés, component-first thinking, desktop-only layouts, and visual drift between design and implementation.

Particular adds a decision layer before and after generation:

**evidence → Project DNA → design thesis → concept → system → build → critique → polish**

The goal is not unusual-looking work for its own sake. The goal is work that becomes difficult to transplant to an unrelated organization by swapping the logo, colors, and copy.

## What it does

- separates factual truth from aesthetic preference;
- extracts Brand, Reference, Client, Category, Project, and Anti-DNA;
- turns subjective direction into measurable design controls;
- treats composition before components;
- detects AI-slop and category-slop without blindly banning patterns;
- defines real interaction, content, responsive, accessibility, and performance states;
- preserves design intent when moving from design tools into code;
- critiques from client, user, brand, and engineering perspectives;
- supports focused modes instead of running a full process for every request.

## Architecture

```text
SKILL.md                 canonical operating contract
modules/                 focused workflows loaded only when needed
adapters/                environment-specific usage guidance
templates/               portable project/design/build artifacts
schema/                  structured Project DNA schema
examples/                worked examples and handoff patterns
evals/                   judgment benchmarks
docs/                    deeper methodology and validation notes
```

### Portable project layer

For substantial work, Particular can maintain three small artifacts:

```text
PROJECT-DNA.md        product, audience, evidence, constraints, anti-DNA
DESIGN.md             portable visual-system and art-direction contract
IMPLEMENTATION.md     technical contract for production builds
```

`SKILL.md` controls **how the agent thinks and works**. These project files control **what must remain true for this specific product**. This separation makes the system easier to reuse across tools without duplicating giant prompts.

## Quick start

### 1. Install or reference the skill

Clone the repository or copy it into the skill/instructions location supported by your agent environment.

```bash
git clone https://github.com/baghedoudhicham/particular.git
```

If your tool supports Agent Skills, point it to the repository's `SKILL.md`. Otherwise reference `SKILL.md` from the tool's project instructions and use the matching file in `adapters/`.

### 2. Start with the actual task

You do not need to invoke every mode manually. Example:

```text
Use Particular to redesign this homepage. Preserve the existing brand assets and working navigation. Research the supplied references, establish the strongest design thesis, then implement and critique the responsive result.
```

For a critique:

```text
Use Particular's critique mode. Do not redesign yet. Identify the three highest-leverage problems, generic AI patterns, and any mismatch with the product/category.
```

### 3. Keep project truth portable

For longer projects, create `PROJECT-DNA.md`, `DESIGN.md`, and—when code is involved—`IMPLEMENTATION.md` from the templates in `/templates`.

## Supported workflows

| Mode | Use it for |
|---|---|
| Discover | organization, audience, category, references, constraints |
| DNA | measurable design evidence and anti-DNA |
| Strategize | positioning, IA, hierarchy, design thesis |
| Concept | genuinely different compositional directions |
| Design | screens, systems, content hierarchy, states |
| Build | production implementation |
| Redesign | improve an existing experience without erasing what works |
| Critique | adversarial quality review |
| Polish | local refinement after architecture is stable |
| Contest | infer preference from selections, ratings, and feedback |
| Scroll | narrative/immersive scroll when it is justified |

## Cross-tool workflow

A useful pattern is:

```text
Stitch / Figma
   ↓ explore composition and art direction
DESIGN.md + PROJECT-DNA.md
   ↓ preserve decisions
AI Studio / Claude Code / Codex / Cursor / Lovable
   ↓ implement
Particular critique + polish
   ↓ validate specificity, UX, responsive behavior, accessibility
Production
```

The tools can change. The evidence and design thesis should not silently change with them.

See [`adapters/`](adapters/) for environment-specific guidance and [`examples/cross-tool-handoff.md`](examples/cross-tool-handoff.md) for a worked handoff.

## Core principles

1. **Truth before taste.** Never invent proof, product capabilities, or client facts.
2. **Concept before components.** Start with the experience and composition, not a card library.
3. **Category fit before trend fit.** Useful conventions are not the enemy; generic convention is.
4. **Distinctiveness is structural.** Use hierarchy, rhythm, typography, imagery, information design, and interaction before decoration.
5. **Responsive means recomposition.** Preserve priority and meaning, not desktop coordinates.
6. **Motion must communicate.** Animation should explain hierarchy, state, causality, continuity, or feedback.
7. **Accessibility is part of art direction.** Not a final compliance pass.
8. **Build less. Justify more. Resolve deeply.**

## Examples

- [`examples/brief-to-build.md`](examples/brief-to-build.md) — turning a client brief into a design/build workflow
- [`examples/project-dna.json`](examples/project-dna.json) — structured Project DNA
- [`examples/cross-tool-handoff.md`](examples/cross-tool-handoff.md) — preserving direction from design exploration into implementation

## Evaluation

Particular includes `/evals` because a design skill should be tested on judgment, not just whether a model follows formatting instructions. Benchmarks should include conflicting evidence, client preference, factual integrity, generic-pattern detection, responsive reasoning, and implementation preservation.

## Who it is for

- product and web designers using AI as a collaborator;
- frontend engineers who need better design judgment in coding agents;
- agencies and freelancers moving work between Figma, generators, and code;
- teams trying to reduce generic AI-generated interfaces without slowing down delivery.

## Status

Particular is actively evolving. The current development line focuses on portability, examples, validation, and stronger design-to-code continuity.

## Contributing

Contributions are welcome, especially:

- difficult real-world design cases;
- before/after evaluations;
- adapters for additional agent environments;
- accessibility/responsive test cases;
- examples where the obvious visual trend was the wrong answer.

See [`CONTRIBUTING.md`](CONTRIBUTING.md).

## License

MIT. See [`LICENSE`](LICENSE).

---

Created by [Hicham Baghedoud](https://github.com/baghedoudhicham).
