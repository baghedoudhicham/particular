# ChatGPT / Codex adapter

Use Particular as the reusable design skill and keep repository-wide engineering constraints separate.

## Recommended layering

- `AGENTS.md` or project instructions: repository invariants and engineering constraints.
- `SKILL.md`: Particular's reusable design operating contract.
- `PROJECT-DNA.md`: project-specific evidence and constraints.
- `DESIGN.md`: visual-system/art-direction contract.
- `IMPLEMENTATION.md`: technical design contract.

## Working rules

1. Inspect the existing repository before redesigning or implementing.
2. Load only the Particular module relevant to the active task.
3. Preserve working functionality unless the brief explicitly changes it.
4. Prefer focused diffs over full-page regeneration after the system is established.
5. Use screenshots/browser inspection for visual QA when available.
6. Run build, lint, tests, and relevant accessibility checks before declaring code complete.
7. Report unavoidable deviations from the design contract rather than silently improvising.

For design-only conversations, use Particular to establish direction and portable project artifacts before moving into implementation.
