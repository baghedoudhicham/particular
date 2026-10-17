# Claude / Claude Code adapter

Install or reference Particular as a reusable Agent Skill and keep repository instructions separate from design truth.

## Recommended layering

- `CLAUDE.md`: repository-operating constraints only.
- `SKILL.md`: Particular workflow and judgment.
- `PROJECT-DNA.md`: project truth.
- `DESIGN.md`: visual system and art direction.
- `IMPLEMENTATION.md`: implementation contract.

## Working rules

1. Inspect existing patterns before adding dependencies or replacing primitives.
2. Load only the Particular module needed for the current task.
3. Prefer system-level fixes over patching one screen when the issue is systemic.
4. Keep visual-polish changes scoped; do not trigger unrelated refactors.
5. Use browser/screenshot feedback loops when available.
6. Verify functional behavior after design changes.
7. Preserve responsive, accessibility, content, and state requirements from the project contract.
