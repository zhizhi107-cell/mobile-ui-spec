# Specification Quality Review

Use this file to judge whether a mobile UI specification is reasonable, professional, adjustable, localized, and broadly useful.

## Reasonableness

A reasonable specification fits real mobile behavior.

Check:
- It is mobile-first, not a desktop specification compressed into a small screen.
- It avoids complex desktop tables as the default. Prefer grouped lists, summary rows, drill-down pages, cards, or bottom-sheet controls.
- It accounts for thumb reach, safe areas, keyboard behavior, scrolling, and sticky bottom actions.
- It supports small and large phone screens.
- It distinguishes page-level actions from item-level actions and keeps the main consumer goal obvious.

## Professional Completeness

A professional mobile UI specification should cover:

- Layout grid, spacing, density, and responsive behavior
- Typography, localized line height, and truncation strategy
- Color, contrast, semantic feedback, and theme rules
- Touch target size and user-facing feedback states
- Navigation, tabs, lists, forms, dialogs, bottom sheets, search, filters, and feedback
- Loading, empty, error, disabled, unavailable, selected, confirmation, and success states
- Accessibility labels, contrast, and readable hierarchy
- Safe-area and keyboard handling

## Adjustability

The specification should adapt to business type:

- Consumer apps: low learning cost, clear next step, useful feedback, restrained visual emotion
- Commerce: product image clarity, price hierarchy, conversion actions, promotion restraint
- Content: reading comfort, title hierarchy, media quality, smooth browsing
- Community: content stream clarity, author identity, interaction entry points
- Finance, healthcare, government: trust, stability, explicit feedback, low ambiguity, conservative visual treatment
- Dashboards: summary first, drill-down details, mobile-friendly filtering and comparison

## Applicability

Good rules directly guide implementation.

Prefer:
- "Primary touch targets should be at least 44px high."
- "List rows should usually be 56-72px high, with primary text at 15-17px and secondary text at 12-14px."
- "Use a bottom sheet for multi-option mobile filtering."

Avoid:
- "Make the interface clean."
- "Keep the style consistent."
- "Use appropriate spacing."

## Revision Rules

- If a rule is abstract, make it measurable.
- If a rule is over-specific, add business or component variants.
- If a rule duplicates another rule, merge them.
- If a rule fights platform conventions, justify it or remove it.
- If a rule creates visual polish at the cost of clarity, simplify it.
- If localized copy sounds translated, rewrite it as native product language for the target locale.
