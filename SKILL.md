---
name: mobile-ui-spec
description: Use when creating, reviewing, adjusting, or applying mobile-first and product UI design specifications for apps, mobile web, H5 pages, mini-program screens, components, localized Chinese or English copy, mobile layout, accessibility, conversion flows, or frontend polish.
metadata:
  short-description: Locale-aware mobile UI spec review and application
---

# Mobile UI Spec

Use this skill for mobile-first and product UI work across locales. The goal is not only to produce UI rules, but to judge whether those rules are professional, reasonable, adaptable, localized, and specific enough to guide real implementation.

Use the product context to choose language:
- If the product, user, or source design is Chinese, write natural Chinese UI copy and design-spec wording.
- If the product, user, or source design is English or international, write natural English UI copy and design-spec wording.
- If the locale is unclear, keep structural guidance language-neutral and avoid forcing Chinese examples into the output.

## Core Workflow

1. Identify the mobile scenario:
   - Native app
   - Mobile web or H5
   - Mini program
   - Consumer app
   - Commerce, content, community, lifestyle, local service, finance, healthcare, education, travel, or productivity flow

2. Review the specification before applying it:
   - Check whether it is mobile-first rather than copied from desktop UI.
   - Check whether localized text length, line height, truncation, and natural wording are covered.
   - Check whether touch targets, safe areas, keyboard behavior, and bottom actions are covered.
   - Check whether user-facing feedback states are complete.
   - Check whether the rules are concrete enough for implementation.
   - Check whether the rules can adapt to the business domain.

3. Adjust the specification:
   - If a rule is vague, convert it into measurable guidance.
   - If a rule is too rigid, add scenario-based variants.
   - If a rule conflicts with an existing product system, prefer the existing system unless it harms usability.
   - If a rule is visually fashionable but weakens clarity, simplify it.
   - If localized copy feels translated or unnatural, rewrite it in native product language for the target locale.

4. Apply the specification:
   - Use the product's target language for UI copy and spec wording.
   - Design for touch first.
   - Use mobile-appropriate navigation, lists, forms, dialogs, bottom sheets, and feedback.
   - Provide loading, empty, error, disabled, selected, unavailable, and success states when relevant.

5. Verify the result:
   - Check text overflow, clipped localized text, cramped controls, readable hierarchy, safe-area support, scroll behavior, keyboard behavior, and contrast.
   - For implemented UI, run visual verification when a browser or app preview is available.

## When To Read References

- Read `references/spec-quality.md` when creating, reviewing, scoring, or revising a design specification.
- Read `references/mobile-layout.md` when designing page structure, navigation, density, safe areas, or responsive behavior.
- Read `references/localized-copywriting.md` when writing or reviewing localized UI text, especially Chinese and English product copy.
- Read `references/component-rules.md` when designing or reviewing mobile components.
- Read `references/design-spec-docs.md` when creating or revising Figma design-system documentation pages, component spec pages, token pages, or visual rule pages.
- Read `references/review-checklist.md` before final delivery or when asked for an audit.

## Quality Score

Rate the UI specification from 1 to 5 on:

- Mobile suitability
- Localization quality
- Component completeness
- Feedback coverage
- Accessibility
- Implementation clarity
- Business adaptability

If any score is below 4, revise the specification before using it. Explain the weak area briefly and make the smallest useful adjustment.
