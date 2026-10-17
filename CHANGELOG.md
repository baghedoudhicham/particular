# Changelog

All notable changes to Particular are documented here.

## 0.3.0 — in development

Particular becomes portable across design generators, coding agents, and design tools without duplicating its core methodology.

### Added

- root `README.md` with positioning, quick start, architecture, workflows, examples, and contribution paths
- environment adapters for ChatGPT/Codex, Claude/Claude Code, Google AI Studio/Gemini, Stitch, Cursor, Lovable, and Figma
- portable `PROJECT-DNA.md`, `DESIGN.md`, and `IMPLEMENTATION.md` templates
- cross-tool handoff example showing how design intent survives exploration → refinement → implementation
- clearer separation between reusable skill behavior, project truth, visual-system truth, implementation constraints, and tool-specific instructions

### Improved

- repository visibility and onboarding
- cross-tool design-to-code continuity
- progressive context loading instead of duplicating large prompts
- guidance against tool-default visual drift
- examples focused on structural design decisions rather than style presets

## 0.2.0 — in development

Particular becomes a directly loadable, testable agent skill rather than only a design methodology.

### Added

- portable `SKILL.md` with skill metadata and a self-contained operating contract
- explicit mode selection and progressive workflow behavior
- `schema/project-dna.schema.json` for structured, portable Project DNA
- `evals/` benchmark framework for testing judgment rather than prompt compliance
- first synthetic benchmark covering conflicts between written aesthetic language and demonstrated client preference
- stronger action/analysis behavior, inspection requirements, and anti-overengineering guidance
- clearer definition of done for design and implementation work

## 0.1.0 — 2026-09-08

Initial public release.

### Added

- factual truth vs. preference truth model
- evidence weighting
- Brand / Reference / Client / Category / Project / Anti-DNA
- explicit design calibration
- visual-category identification
- 3 / 10 / 30-second comprehension test
- composition-before-components framework
- geometric specification rules
- responsive recomposition
- accessibility and performance constraints
- SEO / generative discoverability guidance
- AI-slop and category-slop firewalls
- transplant and screenshot-deception tests
- adversarial multi-role critique
- contest/client preference ledger and post-decision learning
- focused Discover, DNA, Concept, Design, Build, Redesign, Critique, Polish, Contest, and Scroll modules
- Project DNA example and project/critique templates
