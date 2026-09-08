---
name: particular
description: Evidence-led web design operating system for researching, designing, critiquing, redesigning, and implementing distinctive websites. Use when a task involves a website, landing page, frontend, visual direction, design system, responsive design, client brief, reference analysis, or design critique and the result should be specific to the organization rather than generic AI output.
license: MIT
metadata:
  version: "0.2.0"
  author: Hicham Baghedoud
  repository: https://github.com/baghedoudhicham/particular
---

# Particular

Do not maximize novelty. Maximize specificity.

Particular is an evidence-led operating system for web design. Its purpose is to make the result difficult to transplant to an unrelated organization by merely changing the logo, colors, and copy.

## Operating contract

When this skill applies, do not begin by styling components. Establish enough evidence to make the important design decisions first. Use the smallest workflow that fits the task: a critique should not trigger a full redesign; a polish request should preserve successful architecture; a build request should inspect the existing implementation before changing it.

Default to action when the user asks to create, edit, redesign, or implement. Default to analysis when the user asks to review, compare, critique, or explore. Never claim to have inspected an asset, file, page, implementation, or reference that has not actually been inspected.

## 1. Determine the mode

Choose one primary mode and add secondary modes only when necessary:

- DISCOVER — research organization, audience, category, constraints, references.
- DNA — extract measurable design evidence.
- STRATEGIZE — positioning, IA, content hierarchy, design thesis.
- CONCEPT — create visual/compositional directions.
- DESIGN — resolve screens and system.
- BUILD — implement production frontend.
- REDESIGN — improve an existing experience while preserving what works.
- CRITIQUE — evaluate against quality gates.
- POLISH — freeze architecture and improve resolution locally.
- CONTEST — infer preference from client selections, ratings, and feedback.
- SCROLL — use scroll as a timeline only when storytelling justifies it.

## 2. Establish truth before taste

Maintain two independent truth systems.

### Factual truth

Classify important information as LOCKED, VERIFIED, CLIENT-SUPPLIED, INTERPRETABLE, UNDEFINED, PROPOSED, or PLACEHOLDER.

Never present UNDEFINED, PROPOSED, or PLACEHOLDER information as fact. Never invent metrics, customers, awards, employees, locations, inventory, pricing, testimonials, specifications, certifications, case outcomes, partnerships, compliance, or product capabilities.

### Preference truth

For subjective design decisions, weight evidence in this order unless project evidence clearly warrants otherwise:

1. designs the client selected;
2. designs the client highly rated;
3. visual references explicitly supplied by the client;
4. official brand assets;
5. current identity and product;
6. useful category conventions;
7. written aesthetic preferences;
8. abstract adjectives;
9. designer interpretation.

Preference truth can resolve aesthetic ambiguity. It can never override factual truth.

## 3. Build the evidence model

Extract only what is useful for the task.

BRAND DNA: logo geometry, color relationships, typography, materials, photography, illustration, iconography, shapes, patterns, voice, product/physical geometry.

REFERENCE DNA: grid, margins, gutters, density, type scale, type personality, image/type ratio, crops, light/dark ratio, color distribution, borders, radius, depth, cards, icons, CTA prominence, navigation, section rhythm, motion, interaction, ornament, composition archetypes.

CLIENT DNA: what was chosen, rated, rejected, criticized, repeatedly requested, and left untouched.

CATEGORY DNA: conventions that aid recognition/trust, conventions that are tired, conventions worth elevating, conventions whose removal would damage usability or credibility.

PROJECT DNA: ideas that can exist specifically because this organization/product exists.

ANTI-DNA: what this project must not become.

When sources conflict, resolve the conflict explicitly using authority, relevance, recency, specificity, and preference signal. Do not silently average contradictory evidence.

## 4. Identify the visual category

Before concept generation, answer internally: what visual category is the client actually buying, and what would the best version of that category look like?

Innovate inside the desired category before trying to replace it. Do not assume technical means monospace, luxury means sparse serif, enterprise means blue, AI means gradients, architecture means extreme minimalism, or creative means asymmetry.

## 5. Calibrate the design

Infer project-specific values from 1–10 where useful:

brand expression, visual novelty, layout variance, visual density, information density, typographic expression, image dominance, editoriality, technicality, materiality, ornamentation, CTA prominence, interaction complexity, motion intensity, immersive/3D intensity.

Also locate the direction on relevant spectra: rectilinear↔organic, quiet↔expressive, institutional↔human, utility↔editorial, precise↔playful, minimal↔layered.

These are evidence-based controls, not arbitrary style settings.

## 6. Model the business and user journey

Identify the offering, audiences, primary user intent, primary conversion, trust requirements, objections, decision criteria, CMS/editorial needs, and repeat-user needs.

Map major content to: ARRIVE → RECOGNIZE → UNDERSTAND → BELIEVE → EXPLORE → EVALUATE → ACT.

Each major section should primarily ORIENT, EXPLAIN, DEMONSTRATE, PROVE, COMPARE, NAVIGATE, CONFIGURE, TRANSACT, or CONVERT. Remove sections without a meaningful job.

Run the 3/10/30-second test: in 3 seconds the category/relevance/character should register; in 10 seconds the offering, audience, differentiation, and next action should be understandable; in 30 seconds proof, offering structure, evidence, and next action should be findable.

## 7. Write the design thesis

Before substantial generation, establish a concise internal thesis:

“This experience should feel [qualities] because [business/brand reason]. Its dominant design behavior comes from [specific property]. It should avoid [wrong category/convention].”

Define the design idea, brand device, composition idea, content idea, and interaction idea. If one is not justified, omit it rather than inventing decoration.

## 8. Composition before components

Establish dominant element, grid, visual center, alignment datums, density, whitespace, image behavior, reading path, contrast, continuity, and section transitions before choosing cards/components.

Translate subjective direction into geometry: viewport, max width, columns, margins, gutters, spans, section heights, image ratios, crops, text measure, deliberate line breaks, overlap, negative space, and transitions.

Avoid three consecutive sections with the same eyebrow → H2 → paragraph → card-grid pattern. Vary scale, density, alignment, image dominance, background, interaction, and information topology while preserving coherence.

## 9. Build visual systems from evidence

TYPOGRAPHY: prefer official brand type, then supplied/licensed type, then a contextual family, then robust fallback. Define display, heading, body, UI, metadata roles. Usually use one or two families. Control measure, line-height, tracking, weight, line breaks, responsive scaling, numerals, punctuation, and localization.

IMAGERY: classify documentary, product, architectural, people, technical, editorial, conceptual, or generated. Give every image a job: prove, demonstrate, explain scale, humanize, differentiate, orient, or create atmosphere. Define crop, focal point, treatment, responsive behavior, loading priority, and alt intent.

ICONS: prefer brand icons → existing project family → one established library → custom SVG. Do not mix libraries casually. Define optical box, stroke/fill, corners, weight, states, and semantic role.

COMPONENTS: use components for behavioral consistency, not visual sameness. Do not force unequal information into equal cards. Avoid cards-inside-cards and containerizing everything.

## 10. Derive originality from the organization

Derive one to three devices from logo geometry, product construction, materials, architecture, workflow, geography, data, culture, history, manufacturing, or customer behavior. A device can affect grid, crop, divider, navigation, motion, iconography, interaction, image treatment, or section transition. Do not repeat it everywhere.

Run the transplant test: if swapping the logo, name, and palette could plausibly turn the design into an unrelated company, strengthen its connection to the actual business, brand, product, content, audience, or physical world.

## 11. Use an interaction budget

Default to one signature interaction, two to four supporting interactions, and standard utility interactions. Motion should reinforce orientation, causality, continuity, hierarchy, or feedback.

Invoke immersive scroll only when chronology, spatial transformation, progressive reveal, or narrative comprehension benefits from it. Define entry, progression, pinning, transition, exit, mobile behavior, and reduced-motion fallback. Every major scroll state should still work as a static composition.

## 12. Design real states

For functional interfaces account for default, hover, focus, active, selected, loading, success, empty, disabled, error, validation, and partial-data states as applicable. Test long content, zero/many results, missing imagery, slow networks, validation errors, mobile keyboards, keyboard navigation, and real CMS variability.

## 13. Responsive recomposition

Responsive design is not desktop shrinkage. For each composition choose PRESERVE, STACK, COLLAPSE, REORDER, REFRAME, REPLACE INTERACTION, or REMOVE DECORATION. Preserve hierarchy, meaning, sequence, and interaction intent—not coordinates.

## 14. Accessibility, performance, and discoverability

Target WCAG 2.2 AA unless requirements differ. Account for semantics, heading order, contrast, visible focus, keyboard behavior, target sizing, forms/errors, zoom/reflow, reduced motion, screen-reader order, alternative text, and non-color-only communication.

Set sensible budgets for images, video, fonts, JavaScript, WebGL/3D, animation, and third-party scripts. Prefer responsive imagery, modern formats, lazy loading, font discipline, native/CSS behavior, progressive enhancement, and server-rendered/indexable content where appropriate.

For discoverability, preserve crawlability, canonicalization, descriptive URLs, logical navigation, internal links, semantic headings, visible factual content, useful media, and accurate structured data. Never fabricate schema or hidden AI-targeted content.

## 15. AI-slop and category-slop firewall

Challenge unjustified gradient text, purple/blue AI gradients, glassmorphism, floating rounded cards, arbitrary bento, repetitive three-card grids, icon-title-paragraph repetition, universal rounding, decorative blobs/dots, infinite marquees, fake dashboards/terminals/telemetry/technical diagrams, excessive glow, scroll reveal everywhere, generic parallax, huge type used only as spectacle, arrows on every CTA, random monospace, meaningless numbering, tiny uppercase everywhere, badge overload, generic chrome 3D, and generic stock imagery.

These are not universally forbidden. Keep them when evidence, brand, content, or usability justifies them.

Also challenge category clichés without destroying useful category recognition. Elevate conventions rather than reflexively rejecting them.

## 16. Use references as evidence, not templates

For each meaningful reference determine: what to learn, what not to copy, why the stakeholder may like it, what transfers, and what is context-specific. Extract spacing logic, image behavior, typography relationships, motion philosophy, composition, density, and interaction character; rebuild them through the target brand's evidence.

## 17. Critique adversarially

Before declaring substantial work complete, evaluate through four roles:

CLIENT: would this stakeholder actually choose it?
USER: can the intended user understand and use it?
BRAND: could this belong specifically to this organization?
ENGINEERING: can it survive implementation, accessibility, responsive behavior, and real content?

For each relevant role identify strongest decisions, weakest decisions, one thing to remove/refine, and the largest risk. Do not defend the design during critique.

Quality gates: factual accuracy, client desirability, category fit, brand specificity, IA, content, composition, typography, imagery, interaction, functional UX, responsive behavior, accessibility, performance, discoverability, implementation, AI-slop, category-slop, transplant test, and 100%-zoom inspection.

Never approve a design only from a zoomed-out full-page screenshot. Inspect representative desktop, tablet, and mobile views at readable scale.

## 18. Iterate locally

Classify feedback as fact, content, brand, preference, style, composition, UX, interaction, responsive, accessibility, performance, or implementation. Classify scope as micro, local, section, or systemic. Make the smallest intervention capable of solving the problem. Freeze successful sections. Regenerate globally only when the strategy itself is wrong.

For redesigns: audit → identify strengths → freeze what works → rank problems → fix hierarchy → composition → typography → UX → interaction → polish.

## 19. Learn from actual decisions

When client ratings, rejections, selections, or winners become available, update the preference model. Compare what was chosen with what was built, what the brief appeared to imply, what the choice reveals, and which lesson is project-specific versus generalizable. Do not rationalize a miss or overfit one outcome.

## 20. Build contract

Before production implementation, resolve framework, CMS/data needs, routing, component ownership, tokens, responsive states, content variability, image pipeline, animation stack, accessibility, analytics, metadata, loading/error states, and implementation constraints that materially affect the design.

Inspect existing code before making claims or modifications. Reuse established project conventions when sound. Avoid unnecessary abstractions and dependencies. Implement the actual design logic rather than hard-coding screenshots.

## Definition of done

The result should appear researched, strategized, art-directed, written, designed, tested, and engineered for the specific organization. Visual polish cannot rescue false information, wrong client preference, generic composition, poor usability, inaccessible interaction, or brittle implementation.

Build less. Justify more. Resolve deeply.
