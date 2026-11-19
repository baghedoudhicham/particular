# Quality Gates

Do not call the work finished until critical gates pass.

1. Factual Accuracy
2. Client Desirability
3. Category Fit
4. Brand Specificity
5. Information Architecture
6. Content Quality
7. Composition
8. Typography
9. Imagery
10. Interaction
11. Functional UX
12. Responsive
13. Accessibility
14. Performance
15. Search / Discoverability
16. Implementation
17. AI-Slop
18. Category-Slop
19. Transplant Test
20. 100% Zoom

## Adversarial review

Run four critics:

- **Client critic** — would the stakeholder actually choose it?
- **User critic** — can the intended user understand and use it?
- **Brand critic** — could this belong only to this organization?
- **Engineering critic** — can it survive implementation and real content?

Each critic returns:

- 3 strongest decisions
- 3 weakest decisions
- 1 thing to remove
- 1 thing to refine
- 1 risk

Do not defend the design while running critique.

## Screenshot-deception check

Inspect at realistic size on desktop, tablet, and mobile. Full-page thumbnails hide weak body text, bad controls, poor contrast, broken spacing, and density problems.
\n## Evidence for iterative polish\n\nFor each atomic change, record the baseline, hypothesis, scope, screenshot or node reference, change, result and rollback using [`templates/atomic-refinement-log.md`](../templates/atomic-refinement-log.md). See [`modules/atomic-refinement.md`](../modules/atomic-refinement.md).\n\nTreat these as distinct statuses: **visual QA**, **responsive QA**, **functional QA**, **build QA** and **client approval**. One passing status does not imply another. Prefer readable-size screenshots over compressed full-page thumbnails. Reject improvements that degrade critical content, contrast, source truth or user task completion.\n