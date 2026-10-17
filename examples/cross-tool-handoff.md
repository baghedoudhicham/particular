# Cross-tool handoff example

This example shows how Particular keeps a design coherent when exploration, refinement, and implementation happen in different tools.

## Scenario

A small service business needs a new homepage. The team explores in Stitch, refines the system in Figma, and implements in AI Studio or Claude Code.

The mistake to avoid is allowing each tool to reinterpret the project from scratch.

## 1. Establish Project DNA

```md
# PROJECT DNA

## Product
- Category: appointment-based local service
- Primary job: turn qualified visitors into bookings
- Audience: mobile-first local customers

## Brand
- Character: precise, warm, craft-led
- Anti-character: generic luxury, corporate SaaS, rustic cliché

## Design thesis
> The site should feel like a working atelier: precise, tactile, local, and calm. The visual system should derive from the business's real process and material details rather than generic premium styling.

## Anti-DNA
- beige + serif + orange as an unearned premium shortcut
- generic three-card service grid
- fake reviews or metrics
- excessive rounded cards
```

## 2. Explore in Stitch

Ask for 3 structurally different routes:

1. **Process-led** — the booking/service journey determines the page rhythm.
2. **Editorial craft** — strong photography, controlled type, asymmetrical evidence blocks.
3. **Utility-first local** — availability, location, service choice, and booking dominate.

Reject routes that only differ by palette or font.

## 3. Converge into DESIGN.md

```md
## Intent
- Design thesis: working atelier, not luxury template
- Category cue: trustworthy local service
- Avoid: generic premium hospitality styling

## Typography
- Display: compact grotesk with controlled line breaks
- Body: highly legible sans
- Metadata: small but not uppercase-by-default

## Layout
- Strong vertical datum
- Irregular image/text rhythm
- Booking action remains visible without becoming a floating pill everywhere

## Imagery
- Real workspace, tools, material, finished work
- Avoid generic smiling stock portraits

## Motion
- Process/state transitions only
- No reveal-on-scroll applied to every block
```

## 4. Implement with IMPLEMENTATION.md

```md
## Design invariants
- preserve the atelier/process thesis
- do not replace typography with generator defaults
- no fabricated reviews or numbers
- mobile booking hierarchy is more important than preserving desktop composition

## Definition of done
- booking path works
- empty/loading/error states are covered where applicable
- mobile, tablet, desktop inspected at readable scale
- keyboard focus visible
- design passes Particular critique
```

## 5. Critique after implementation

Run four checks:

- **Client:** does it look like something this business would select?
- **User:** can a visitor understand service, trust, location, and booking quickly?
- **Brand:** could the same design be transplanted to five unrelated businesses?
- **Engineering:** did the build preserve state, responsive, accessibility, and performance behavior?

If the build becomes generic during implementation, fix the system or composition that drifted. Do not compensate with more decoration.

## Why this works

The tools are replaceable. The evidence, thesis, and system are not. Particular keeps those decisions portable so a design can move between generators and coding agents without becoming a new project at every handoff.
