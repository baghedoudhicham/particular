# Agent Adapters

Particular is designed to travel between tools rather than depend on one vendor.

## General pattern

1. Load `SKILL.md` as the canonical instruction layer.
2. Add only the module needed for the current task.
3. Provide a Project DNA artifact when the project spans multiple sessions or tools.
4. Keep authoritative facts and visual references attached or linked.
5. Ask the agent to preserve successful decisions between iterations.

## Figma / Figma Make

Use Particular to establish evidence, hierarchy, geometry, responsive behavior, content truth, and critique criteria before generation. Translate aesthetic language into explicit layout rules.

## Claude / agent skills

Use `SKILL.md` as a project skill and focused modules as task-specific skills. Avoid duplicating the entire system into every sub-agent.

## Codex / Cursor / Replit

Pair Particular with the repository's implementation conventions. Use the implementation contract before code generation and preserve existing components/tokens when they are sound.

## AI Studio / Stitch / other builders

Give the builder:

- source hierarchy
- Project DNA
- visual category
- design thesis
- calibration
- IA/content priorities
- geometric composition rules
- locked facts
- anti-DNA
- responsive rules

Then iterate in isolated passes rather than globally regenerating the product after every critique.

## Portability rule

Project-specific decisions belong in Project DNA, not in the global Particular skill. The global skill should remain reusable and neutral.
