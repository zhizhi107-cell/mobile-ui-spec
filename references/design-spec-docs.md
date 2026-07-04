# Design Specification Pages

Use this reference when creating or reviewing Figma design-system documentation pages for mobile-first or product UI systems across locales.

This file is for design-system documentation pages, not the production app screen itself. Prioritize clear rule expression, asset organization, maintainability, and team handoff. Choose Chinese or English wording according to the product locale and source material.

## Page Structure

- Organize documentation pages in a stable sequence: principles, design variables or size rules, component assets, composition rules, and review checklist.
- Do not create a new page for every small revision. If the content belongs to an existing component or foundation spec, integrate it into the existing page rhythm.
- Keep page width, content width, module width, and side margins consistent across the documentation set.
- When content grows, let the page extend vertically through Auto Layout while preserving the same page width, content width, and alignment.
- Use the same outer margin rule across all documentation pages. Do not change side margins just because one page contains more content.
- Keep consistent inner padding for similar module types, such as example cards, component groups, notes, rule blocks, and checklists.
- Keep consistent vertical spacing between repeated modules. When content changes, let Auto Layout extend naturally instead of manually shifting local elements.
- Align bottom notes, usage guidance, annotations, and checklists to the same content width as the main content.
- Prefer a small number of clear modules over many weak cards. If an example already explains the rule, remove duplicated explanation.
- Use real component dimensions in examples instead of approximate placeholder drawings.

## Specification Judgment Principles

- Treat user feedback as design input, not final spec copy. Rewrite comments, preferences, and revision requests into stable team-facing rules with clear scope and implementation meaning.
- Do not directly repeat informal user wording in the spec page. Translate it into professional documentation language for the target team and locale.
- Keep foundation specs broadly reusable. Color, type, spacing, icon, and asset rules should describe semantics and boundaries first, instead of binding tokens to overly narrow scenarios or single components.
- Consolidate before adding. When a new color, size, icon category, state, or rule is requested, first check whether it can be merged into the existing system; remove or combine duplicated, low-frequency, or unclear items.
- Use hierarchy and whitespace as the primary grouping tools. Avoid nested cards, stacked outlines, heavy grey blocks, or decorative containers unless they directly improve comprehension.
- New modules must inherit the existing page system: page width, content width, side margins, type scale, section rhythm, and alignment. Complexity in one page is not a reason to invent a separate layout pattern.
- Verify asset examples by real visual effect. Use real assets and real dimensions; check visible optical alignment, complete asset counts, clear naming, text breathing room, and whether icons or labels appear off-center.

## Auto Layout Requirements

- Build sections, cards, rows, and component grids with Auto Layout.
- Avoid hand-positioned elements for repeatable layouts.
- Use consistent vertical rhythm: heading to description, description to examples, examples to notes.
- Align text, icons, buttons, and badges to a shared row or column baseline.
- Do not let text touch borders, overlap frames, or sit under selection lines.
- Before delivery, inspect the page at zoomed-in card level, not only full-page thumbnails.

## Visual Restraint

- Avoid decorative vertical bars, ornamental capsules, heavy grey boxes, or extra outlines unless they clarify grouping.
- Do not use pill-shaped labels as section tags when they can be mistaken for buttons.
- Use cards for examples and component assets, not for every sentence.
- Keep page backgrounds quiet. Let typography, spacing, and real components carry the structure.
- If a rule is hard to understand in text, replace the explanation with a small diagram.

## Color And Type Consistency

- Reuse the existing color and typography specification. Do not introduce temporary greys, reds, greens, or non-standard font sizes.
- Do not use 13px unless the product's typography spec explicitly includes it.
- Common spec text should use the established 12px or 14px body sizes. Component labels and button text should follow the component rule, not the page designer's preference.
- Error, badge, warning, success, neutral, and disabled examples must use semantic colors from the color spec.

## Mobile Size Rules

- When using 375px as the mobile reference width, state the exact page margin and content width.
- If margin is 15px, content width is 345px. All grids, forms, and full-width controls on that page must follow that width.
- Column widths and gaps should be integers. Avoid fractional widths in the written spec.
- Prefer even or system spacing tokens, but if 375px arithmetic requires adjustment, choose integer layout values over visually hidden fractional widths.

## Spec Page Review

- Check whether repeatable sections, card groups, and asset grids use Auto Layout instead of loose manual positioning.
- Check whether page width, content width, and module width remain consistent.
- Check whether long pages extend only vertically while preserving shared page width, content width, and side alignment.
- Check whether similar module types use consistent inner padding.
- Check whether repeated modules use consistent vertical spacing.
- Check whether bottom notes, annotations, usage guidance, and checklists align to the same width as the main content.
- Check for clipped text, text touching borders, overlapping labels, or crowded examples.
- Check whether adjacent sections repeat the same rule and can be merged.
- Check whether every example uses real component dimensions instead of approximate drawings.
- Check whether original asset counts, category counts, and final displayed counts match after organizing or migrating assets.
- Check whether another designer can understand and use the page without repeated clarification.
