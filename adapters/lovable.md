# Lovable adapter

Use Lovable for fast product implementation after the design direction is sufficiently constrained.

Provide:
- `PROJECT-DNA.md`;
- `DESIGN.md`;
- the screen hierarchy and primary flow;
- data/state requirements;
- any implementation constraints.

## Working rules

- Lock the design thesis before broad generation.
- Iterate flow-by-flow or component-by-component once the system exists.
- Avoid repeated whole-app regeneration after the architecture is established.
- Keep backend, data, auth, and security decisions explicit rather than inferred from UI.
- Preserve responsive behavior, accessibility, and state logic during visual refinements.
- Do not allow starter-theme defaults to overwrite the project's type, spacing, color, radius, or motion logic.
