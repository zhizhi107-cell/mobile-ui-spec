# Mobile Layout Rules

Use mobile-first structure, not desktop structure scaled down.

## Page Structure

- Keep primary navigation obvious and stable.
- Use top navigation for title, back, close, search, or page-level actions.
- Use bottom tabs for 3-5 persistent product sections.
- Use sticky bottom actions for high-importance submit, pay, save, or continue actions.
- Respect safe-area insets for devices with home indicators or notches.

## Touch And Density

- Minimum touch target: 44px.
- Common row height: 56-72px.
- Compact controls may be smaller visually, but the interactive area should remain comfortable.
- Avoid placing many similar-weight actions in one row.
- Avoid desktop-style toolbars unless the user is building an editor or power tool.

## Responsive Behavior

- Design for narrow phone screens first.
- Long localized titles may wrap to two lines or truncate with a clear strategy.
- Important values should not rely only on horizontal space.
- Avoid horizontal scrolling except for tabs, chips, media galleries, or controlled comparison views.
- When documenting grid rules, use integer column widths and gaps. Do not write fractional column sizes into the spec.
- For 375px reference screens, define the page margin first, then derive content width, column count, and gap from it.
- If a common 4px spacing system conflicts with integer grid math, keep spacing visually consistent but make the documented layout values implementable.

## Keyboard And Bottom Areas

- Inputs near the bottom should stay visible when the keyboard opens.
- Sticky bottom actions should not cover the input the user is editing.
- Bottom sheets should allow dismissal, scrolling, and safe-area padding.
- Form validation should appear near the relevant field.

## Domain Adjustments

- Tools: denser lists, compact filters, direct actions, clear status labels.
- Commerce: large product media, clear price hierarchy, prominent purchase action.
- Content: readable rhythm, media-first hierarchy, restrained controls.
- Finance, healthcare, government: conservative color, explicit states, clear confirmation.
