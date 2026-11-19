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

Synchronize durable decisions into `DESIGN.md` so coding agents and other tools can consume the same art direction without depending on the Figma file alone.


## Atomic Figma polish

When refining an existing file, follow [Atomic Design Refinement](../modules/atomic-refinement.md).

1. Open and inspect the **exact** current screen, client feedback and linked source before styling.
2. Duplicate the target screen into a clearly named review version; preserve the approved baseline.
3. Freeze the narrative, approved sections, brand, genuine assets and functional intent.
4. Make one change dimension per pass—typography, hierarchy, component geometry, restrained depth, responsive composition or accessibility—not all at once.
5. Prefer auto-layout for semantic section stacks, content cards and responsive lists. Keep explicit coordinates for intentional artwork; converting a layout is a QA event, not an automatic best-practice improvement.
6. Reuse real vector icons and source images; keep design-specific artwork editable. Avoid invented product metrics and generic decorative effects.
7. After each pass screenshot the **changed module** at a readable scale, then inspect the full page and mobile counterpart. Check that sections, content and asset fills survive.
8. Log PASS / NEEDS REVIEW / FAIL and any untested breakpoints or behavior. Figma visual QA does not validate browser interactions, responsive CSS, reduced motion, deployment or client approval.

Use `templates/atomic-refinement-log.md` as the pass record. Keep selected visual decisions in `DESIGN.md`, not just in a Figma comments thread.
