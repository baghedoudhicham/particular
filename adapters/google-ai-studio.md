# Google AI Studio / Gemini adapter

Treat AI Studio primarily as a build and behavior surface, not the source of art direction.

Provide context in this order:
1. `PROJECT-DNA.md`
2. `DESIGN.md`
3. `IMPLEMENTATION.md`
4. the exact screen or feature task

## Working rules

- Preserve existing application behavior unless the brief changes it.
- Centralize design tokens instead of allowing starter styles to drift.
- Keep React/TypeScript components modular and explicit.
- Implement responsive and interaction states rather than relying on generated defaults.
- Separate secrets/server logic from client UI.
- Do not invent product capabilities or proof to make the interface look complete.
- Validate the deployed result, not only the editor preview.
- When importing from Stitch, reconcile exported structure against Project DNA and the implementation contract before extending it.
