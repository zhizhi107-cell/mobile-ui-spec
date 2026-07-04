# Mobile Component Rules

Use these rules when designing or reviewing mobile components across product locales.

## Required Feedback States

For consumer-facing mobile UI, prioritize clear feedback after user actions rather than detailed control micro-states.

- Default
- Disabled
- Unavailable or sold out
- Loading
- Selected
- Empty
- Error
- Success
- Confirmation needed

## Navigation

- Top bar: page title, back or close action, optional page-level action.
- Bottom tabs: 3-5 persistent sections with short localized labels.
- Avoid deep navigation without a visible return path.
- For C-end flows, keep the current section and next action obvious.

## Buttons

- Use clear action verbs for labels. In Chinese, use concise verbs such as 保存、提交、确认、筛选、编辑、删除. In English, use direct verbs such as Save, Submit, Confirm, Filter, Edit, Delete.
- Primary buttons should clearly support the current consumer goal, such as 立即购买、去支付、预约、领取、发布、下一步, or Buy now, Pay, Book, Claim, Publish, Continue in English products.
- Destructive actions should require clear confirmation when risk is high.
- Icon-only actions should be familiar or paired with clear context.
- Tap feedback may be subtle, but loading, success, failure, and disabled feedback should be explicit.
- Button colors should come from the current product's color specification. Do not assume orange, green, black, or any other hue as the default primary pattern unless the product system defines it.
- Primary, secondary, destructive, disabled, and loading button states should map to the product's semantic color tokens instead of one-off local colors.
- Accent buttons may support recommendation, benefit, or promotion scenarios, but they should not compete with the main submit action.
- Do not show desktop-style pressed states as a required mobile button state unless the product explicitly needs it. Default, loading, and disabled are usually enough for mobile spec pages.
- Loading state must differ from default through text or visual treatment, such as 处理中, 加载中, Loading, Processing, or a spinner.
- Button text should follow the typography spec: L/M commonly use 16px Medium; S commonly uses 14px Medium.
- Include full-width bottom primary buttons when documenting forms, checkout, publishing, or onboarding flows.

## Lists

- Prefer grouped lists, summary rows, or cards over dense desktop tables.
- A row should have one main purpose.
- Keep right-side actions limited.
- Use status tags, metadata, and hierarchy instead of cramming many columns.

## Forms

- Show validation close to the field.
- Keep labels and placeholders natural.
- Avoid using placeholder text as the only label for complex forms.
- Use appropriate keyboards for phone, number, email, and search fields.
- Use real mobile dimensions in form specs. For a 375px screen with 15px side margins, field width is 345px.
- Common single-line input height is 44px. Keep input text 14px Regular and labels/helper/error copy aligned to the typography spec.
- Do not wrap every input example in a heavy grey container. Use framing only when showing a grouped form area.
- Required states: default, focus, filled, error, disabled, and readonly.
- Error copy stays near the field and explains the correction. Do not replace field validation with a toast.
- Form examples should match the current product domain. Do not reuse procurement, approval, commerce, or social copy unless that is the actual scenario.

## Search And Filters

- Use a search bar for keyword entry.
- Use chips or compact filter entry points for common filters.
- Use bottom sheets for multi-option filters and sorting.
- Show selected filters clearly and allow quick clearing.

## Dialogs And Bottom Sheets

- Use dialogs for confirmation, alerts, and short decisions.
- Use bottom sheets for selection, filters, action menus, and mobile-friendly configuration.
- Keep primary and secondary actions clear.
- Ensure content can scroll when it exceeds the available height.

## Feedback

- Toasts are suitable for lightweight success or failure feedback.
- Inline errors are better for form validation.
- Empty states should explain the state and offer one next action when useful.
- Loading states should preserve layout when possible.
- Purchase, booking, payment, publishing, and deletion flows should provide clear completion or failure feedback.

## Icons

- Icon components should contain only the graphic body. Do not bake background, color, or hit area into the icon itself.
- Use an Icon Slot or container to control size, color, disabled state, selected state, and touch area.
- Use 24px as a common editable source asset size when the product needs a unified icon drawing baseline.
- Display sizes should follow the product scale, preferably a 4px step such as 16, 20, 24, 32, and 36px. Special component scenarios may define exceptions.
- Do not force all display sizes to be equal-scaled from the 24px source. Larger sizes may need independent optical calibration, including stroke weight, detail density, and visual center.
- For 24px icon drawing specs, a 20px drawing area and 2px safe area can be used as a baseline, but keylines are references rather than mandatory templates.
- Icon drawing guidance should show only necessary construction lines: canvas, safe area, centerline, and keyline body. Avoid noisy colors or decorative grids.
- Keep imported icon geometry intact when the user asks for exact library icons.

## Tags And Badges

- Separate relationship tags, content tags, quantity badges, and red-dot badges. They are not interchangeable.
- Tags identify status or category; badges show counts or unread reminders.
- Quantity badges should not replace status labels. Do not mix “已关注”, “热门”, “新”, and “99+” as one component type.
- Numeric badges use semantic red with white text, such as 3, 12, and 99+.
- Red-dot badges must be circular and used only for unread or notification prompts.
- Tags and badges should use existing color and typography rules instead of one-off orange or green capsules.
