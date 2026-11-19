# Atomic Design Review & Polish

Use this module with **CRITIQUE → POLISH** when the user asks for senior-level critique, refinement, advanced effects, final quality passes, responsive cleanup, or design-to-code fidelity. Apply it to Figma, code, AI Studio, Stitch, or other website builders. It is a **method of local improvement**, not permission to reinvent the approved direction.

## 0. Choose the work lane

- **POLISH:** preserve concept, messaging, conversion paths, identity, main content hierarchy, successful interactions and accurate source assets.
- **REDESIGN:** structural change is justified by a documented issue with the direction or an explicit request; still preserve approved content and evidence.
- **ALTERNATE CONCEPT:** build independently and label it an exploration. Never silently replace the approved direction or merge incompatible hero systems.
- **PRODUCTION IMPLEMENTATION:** source code, browser verification, build, accessibility and functional QA are separate gates from static Figma visual approval.

## 1. Establish a source-backed baseline

Capture the **actual existing artifact** before editing: source Figma frame IDs, component structure, brand files, typography, product screenshots, breakpoint previews, client decisions, and relevant code. When a file or source cannot be inspected, mark it unverified.

Inspect a full-page overview **and** readable-scale crops: header/hero; first content and conversion; one representative middle section; lower 70%; CTA/footer; desktop/mobile. Use 100% zoom or equivalent for fit and typography checks. Full-page shrunk screenshots cannot alone establish quality.

Write a compact frozen list (LOCKED), a changeable list (OPEN), and a factual-source table (VERIFIED / CLIENT-SUPPLIED / UNDEFINED / PLACEHOLDER). Preserve originals using a duplicate frame, review branch, or equivalent reversible checkpoint. Record source and destination IDs/paths.

## 2. Make the senior critique falsifiable

Evaluate from four perspectives (client, user, brand, engineering) with **specific evidence**:

| Dimension | What to look for |
| --- | --- |
| Client truth | Chosen vs rejected concepts; what was explicitly liked; approved journeys |
| Conversion | Does the hero demonstrate owner benefit, not lead with tool jargon? |
| Composition | Focal point, scan path, alignment, content balance, and nonrepetitive lower-page rhythm |
| Content | Approved claims, accurate pricing/eligibility, authentic product evidence, labels, links |
| Type & legibility | Scale/measure, line breaks, dense metadata, color contrast, mobile at readable size |
| Identity | Logo fidelity, real icon family, brand accents, avoid transplantable stock patterns |
| Material & effects | Shadows, blur, grain, gradients, borders, layering, state meaning, reduced motion |
| Components | Semantic styles, spacing tokens, Auto Layout/constraints, reusable instances |
| Responsive | Recompose rather than shrink, check clipping and touch targets at key sizes |
| Implementation | Browser build, interactions, form states, keyboard navigation, performance |

For every material issue record: **symptom, location, evidence, severity (P0–P3), user/client consequence, proposed smallest fix, confidence, verification method**. P0 means false/misleading content, broken flow, inaccessible critical control, or major overflow; P1 means weak primary conversion, substantial visual imbalance, or unreadable high-signal text; P2–P3 are secondary craft.

Prioritize factual and functional risk before gradients, animation, or ornamental refinement.

## 3. Run bounded atomic passes

Use the following sequence, skipping irrelevant passes. Each pass must be **independently reviewable**, with the previous successful state retained:

1. **Truth & frozen structure:** resolve claims, approved copy, canonical assets; label concepts as explorations; no invented results, deal metrics, prices, awards, product states or testimonials.
2. **Focal hierarchy:** headline → offer/outcome → single primary CTA → concept/proof. Remove hero competition, make the object understandable, retain user journey.
3. **Geometry & typography:** align datums, text measures, line breaks, real card padding, baselines; fix tiny labels and collisions; improve rhythm without shrinking everything.
4. **Component & material system:** unify icon stroke/optical size, radii, separators, control states, shadows. Introduce only restrained, meaningful physical or branded depth.
5. **Lower-page art direction:** inspect the entire lower 70%; vary information topology (comparison, editorial proof, narrative, table, timeline, demonstrator) instead of repeating cards.
6. **Responsive recomposition:** desktop → tablet → mobile; preserve meaning with stacking/reframing/reordering; no clipped copy, fake mobile screenshot or decorative overflow.
7. **Behavior & release QA:** focus/hover/reduced motion, form validity, links, performance, product screenshot provenance, build/tests, accessible content.

### Atomic pass contract

For every pass keep a concise record:

- **Hypothesis:** what is wrong and why the change helps.
- **Scope:** exact component, section, file, or frame IDs and intentionally untouched areas.
- **Change:** at most one coherent issue family, reversible where possible.
- **Visual check:** before/after render at the relevant actual size; inspect text and bounding boxes, not just screenshots.
- **Regression check:** source content, approved routes, interactions, layout, other breakpoints and visual hierarchy.
- **Decision:** KEEP / ADJUST / REVERT with a one-line evidence-based reason.

No blind cascading changes. If a pass introduces a new conflict, fix or revert it before starting the next pass. Do not count “number of changes” as quality.

## 4. Premium effects budget

An advanced result needs **selective effects**, not more effects. Assign effects a semantic role—material hierarchy, focus, affordance, brand identity, or state feedback.

- Prefer subtle, consistent shadows on the **dominant object or elevated control**, not every card. Avoid multiple exaggerated shadows and heavy hover lift.
- Limit blur to atmospheric background or a justified material plane. Foreground text, widgets, screenshots and essential values should stay crisp.
- Gradients and grain must reinforce branded lighting/materials; they must not obscure labels, saturate all surfaces, or replace real evidence.
- Hairlines, multi-layer dossier edges, authentic geometry and editorial negative space often create more perceived quality than glow.
- Motion should show progression or causality; keep a reduced-motion static state and respect a strict performance budget.
- Validate contrast and screenshot clarity after effects; dark mode and warm/cold accents are not proof of originality.

## 5. Figma and code-specific gates

**Figma:** inspect the source frame; duplicate before major revision; use native Auto Layout for page/rows/cards when safe; use existing design-system tokens and component instances; preserve official logo vectors and authentic source image hashes; label every final/review/alternate frame distinctly. A Figma file is not production code. Never pass a whole-page screenshot off as editable UI. Confirm Auto Layout did not change positions, section extents, text wrap, and clipping.

**Code / AI Studio:** inspect the current repository and deployed preview; change components or styles in small commits, keep source maps/content, run typecheck/lint/build, verify browser at **1440 / 834 / 390 / 320 px** where supported. Validate keyboard, focus, reduced-motion, long strings, missing data, and interaction states. Screenshot diffs should isolate the modified section and spot-check untouched areas.

**Handoff:** keep a clear decision log with exact source references, file/frame IDs, changed components, accepted residual issues, and who must approve. Do not claim “deployed”, “production ready”, “fully responsive”, “accessible” or “client approved” without the matching verification.

## 6. Final gate

A direction is review-ready only if:

- It remains faithful to factual and preference evidence.
- Primary conversion is apparent without software-first explanatory clutter.
- Desktop and mobile each have coherent, deliberate composition.
- There is no clipping/overlap/illegible text, especially at the hero and lower-page CTA.
- Repeated cards have a justified information role, not merely visual convenience.
- Icons, colors, shadows and motion follow one controlled system.
- Real product screenshots are separated from illustrative concepts.
- Visual and implementation verification status is reported accurately.

**Recommended output:** (a) ranked audit findings, (b) pass ledger with KEEP/ADJUST/REVERT decisions, (c) direct links to before/after editable artifacts or review branches, (d) remaining source/QA dependencies.
