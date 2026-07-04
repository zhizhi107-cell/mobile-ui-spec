# Final Review Checklist

Use this before final delivery or during a UI audit.

## Specification Review

- Is the specification mobile-first?
- Is it suitable for the business domain?
- Are vague rules converted into measurable guidance?
- Are rigid rules adjusted with scenario variants?
- Does it support implementation rather than only visual taste?

## Localization

- Is all user-facing copy natural for the target locale?
- Are tab and button labels short enough for the target language?
- Are error messages actionable?
- Are empty states concise and useful?
- Is translated or unnatural phrasing removed?

## Layout And Interaction

- Are touch targets large enough?
- Are primary actions easy to find?
- Are safe areas handled?
- Does the keyboard avoid covering important inputs or actions?
- Does scrolling behave predictably?
- Are bottom sheets and dialogs sized correctly?

## Component Coverage

- Are loading, empty, error, disabled, unavailable, selected, confirmation, and success states covered?
- Are lists mobile-friendly rather than table-like?
- Are filters and sorting suitable for mobile?
- Are forms validated near the relevant field?

## Visual Quality

- Is hierarchy readable on small screens?
- Does localized text avoid clipping and awkward truncation?
- Is contrast sufficient?
- Are colors semantic and restrained?
- Is decoration serving clarity rather than distracting from it?
- Are proximity relationships clear: title with description, label with field, helper/error with the relevant control, and separated groups with visibly larger spacing?

## Design Spec Page QA

- Are all repeatable sections and component groups built with Auto Layout?
- Are section widths, inner margins, card spacing, and baseline alignment consistent?
- Are all colors and font sizes from the existing color and typography specs?
- Are component examples using real dimensions rather than approximate drawings?
- Are asset counts checked after organizing or migrating icons, colors, components, or examples?
- Are button, input, icon, tag, and badge rules integrated into their relevant spec pages without duplicated modules?
- Are quantity badges, status tags, and buttons visually distinct?
- Does example copy match the current product domain instead of borrowing unrelated business scenarios?
