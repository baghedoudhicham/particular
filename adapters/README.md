# Environment adapters

Particular keeps one canonical design method and uses small adapters for tool-specific behavior. The adapter should never redefine the project's art direction.

## Separation of concerns

- `SKILL.md` — reusable design judgment and workflow.
- `PROJECT-DNA.md` — product, audience, factual/preference evidence, constraints, anti-DNA.
- `DESIGN.md` — portable visual-system and art-direction contract.
- `IMPLEMENTATION.md` — technical contract when code is involved.
- `adapters/*.md` — how to make a specific environment respect the above.

## Available adapters

- `chatgpt-codex.md`
- `claude.md`
- `google-ai-studio.md`
- `stitch.md`
- `cursor.md`
- `lovable.md`
- `figma.md`

## Rule

Do not paste every adapter into every context. Load the adapter for the active environment and keep project truth in the portable project files.
