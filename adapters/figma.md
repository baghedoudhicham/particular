# Figma adapter

Use Figma as the high-fidelity source of truth when the project benefits from deliberate manual art direction, design-system work, or collaborative review.

Suggested page structure:
- Direction
- Foundations
- Components
- Patterns
- Screens / Product
- Prototype
- Handoff

Use Particular for evidence, concept selection, critique, and system decisions. Do not turn the file into a component inventory without screen-level composition.

For senior QA and polish, run [Atomic Design Review & Polish](../modules/atomic-review.md). Duplicate source frames before substantial changes; make bounded edits and verify readable-scale hero, lower-page and mobile screenshots. Use native Auto Layout and stable components/tokens where justified, check for unintended reflow, and keep separate approved/review/alternate concept frames.

Synchronize durable decisions into `DESIGN.md` so coding agents and other tools can consume the same art direction without depending on the Figma file alone.
