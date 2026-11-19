# Atomic Design Refinement

Use this protocol alongside **CRITIQUE** and **POLISH** when an existing website has a generally correct strategy and information architecture but needs senior-level craft, visual precision, component quality or implementation fidelity. Apply it to Figma, code, and screenshot-based reviews.

## Contract

**Diagnose → rank → freeze → change one dimension → render → compare → retain or revert.**

Do not combine unrelated layout, typography, effects, content and responsive changes into one uninspectable pass. Do not globally redesign something the client selected. Keep an immutable baseline or a reversible branch/frame. Each intervention must have a bounded scope and a checkable outcome.

## Pass 0 — Baseline and provenance

1. Reopen the exact latest source (screen, repository, render, asset, client feedback). Record version, node/commit reference, widths, and unverified dependencies.
2. Separate **LOCKED** client-approved decisions, **VERIFIED** content/asset evidence, **OPEN** design decisions, and **UNVERIFIED** claims.
3. Capture representative desktop, tablet and mobile renders at legible scale; a full-page thumbnail alone is insufficient.
4. Inventory component reuse, type roles, auto-layout structure, effect count/intensity, overflow, interaction affordances, source-of-truth images and responsive behavior.
5. Record the strongest three decisions, weakest three, one thing to remove, one thing to refine and the largest risk from client/user/brand/engineering perspectives.

## Pass 1 — Prioritize and bound

Rank issues by **user impact × evidence confidence × visual leverage ÷ implementation risk**. Use severity P0 (misleading/broken), P1 (hierarchy or interaction defect), P2 (craft inconsistency), P3 (optional flourish).

Write a micro-brief for every pass:
- **Hypothesis:** exact defect and expected improvement.
- **Scope:** nodes, components or files touched; what remains frozen.
- **Single dimension:** truth/content, hierarchy/type, composition/spacing, components/icons, effects, responsive, or implementation fidelity.
- **Acceptance:** a measurable visual or functional result.
- **Rollback:** original frame/branch or reversible edit.
- **Evidence:** before/after screenshots and source refs.

## Pass 2 — Apply controlled interventions

Preferred order: factual and UX defects → typography/legibility → composition/density → component semantics → imagery/crop → effects and motion → responsive recomposition → implementation details.

- **Typography:** correct font family, line breaks, widths, weights, line height, readable body text and metadata. Never make everything compact by shrinking copy.
- **Composition:** preserve intentional focal points. Reduce repetitive card grids via varied information topology, not unrelated decoration. Keep alignment datums and distinct section jobs.
- **Components:** use native auto layout for semantic stacks and content-driven cards where practical. Reuse component instances for repeated behavior, with consistent icons, borders, states and semantic tokens. Use absolute positioning only for deliberate editorial artwork.
- **Effects:** assign a meaning and a budget. Prefer hairlines, material separation and soft elevation. Avoid blur on text/data widgets, stacked shadows, excessive hover travel, ornamental glows and abstract effects that compete with the user's decision.
- **Icons:** use brand assets or one coherent, genuine vector family; use a common optical box and semantic meaning. Never approximate icons with arbitrary glyphs or decorative bars.
- **Content:** preserve accurate product/brand specifics, claims and client-approved copy. Do not invent testimonials, numbers, guarantees, statuses, transaction results or features.
- **Motion:** justify each animation by feedback, orientation or continuity. Define static/reduced-motion fallback. A static Figma render is not proof of working motion.

## Pass 3 — Verify every atomic change

After **each** pass:
1. Render the changed module at a readable scale plus its surrounding context.
2. Inspect content wrapping, optical alignment, overlap, clipping, hierarchy, contrast, CTA affordance and genuine source assets.
3. Check responsive consequences before advancing; recommended evidence widths: 1440, 834, 390 and 320px unless project constraints dictate others.
4. If a pass fails, revert or adjust **that pass**, not the whole page.
5. Mark **PASS / NEEDS REVIEW / FAIL**. Do not claim browser, accessibility, functional or build success from Figma screenshots alone.

Maintain the record in `templates/atomic-refinement-log.md`; large redesigns should return to REDESIGN mode instead of accumulating patches.

## Final gate

Compare baseline vs revised at realistic size. Verify the client-approved narrative, section and action sequence, real content, responsive recomposition, icon family, type scale, effects discipline, disabled/reduced-motion expectations, and source-code parity. Report what was changed, what was frozen, what was actually tested, and unresolved risks.

**Stop polishing when further changes add novelty but no better understanding, trust, action or distinctiveness.**
