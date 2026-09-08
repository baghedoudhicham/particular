# Build Module

Use BUILD when translating a validated direction into production frontend.

## Implementation contract

Before coding define:

- framework/runtime
- routing
- CMS/data model
- component ownership
- design tokens
- typography/font loading
- image pipeline
- responsive states
- interaction/animation stack
- accessibility requirements
- analytics
- SEO metadata
- loading/error/empty states

## Preserve design intent

Do not simplify away the brand-defining composition merely because a standard component is easier to code.

Do not recreate solved project components with arbitrary new abstractions.

## Production resilience

Test:

- long/short content
- missing images
- localization
- dynamic data
- slow network
- keyboard use
- reduced motion
- viewport extremes
- CMS editing

## Performance

Budget fonts, media, JS, third parties, and animation. Prefer progressive enhancement and native platform behavior where possible.

## Done

A production build is not done when it visually resembles a screenshot. It must preserve hierarchy, behavior, accessibility, responsive logic, content truth, and performance.
