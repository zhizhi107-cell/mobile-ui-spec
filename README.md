# Mobile UI Spec

A locale-aware skill that helps AI create better mobile UI design specifications and cleaner design-system documentation layouts.

It is built for designers, product teams, and AI-assisted workflows where UI guidelines need to be clear, practical, maintainable, well-structured, and easy for developers to implement.

Instead of letting AI generate generic design-spec text or messy documentation pages, this skill guides AI to think more like an experienced UI/UX designer: review the system first, consolidate scattered rules, translate vague feedback into usable guidance, improve page layout, and produce documentation that can actually support design-system work.

## Why This Skill Exists

AI often struggles with design specifications.

Common problems include:

- Repeating user feedback directly instead of rewriting it as professional specification language.
- Adding too many tokens, weak cards, repeated rules, and low-value sections just to look complete.
- Making colors, typography, icons, or spacing rules too rigid for real component adaptation.
- Focusing on visual presentation while ignoring naming, implementation clarity, asset counts, and maintenance cost.
- Creating design-spec pages with inconsistent margins, type sizes, module spacing, and layout rhythm.
- Overusing outlines, grey blocks, and nested cards instead of using hierarchy and whitespace.
- Building Figma spec pages that look crowded, misaligned, or visually disconnected from the rest of the system.
- Showing icons, colors, or typography examples without real assets, real dimensions, or optical alignment checks.
- Mixing Chinese and English copywriting habits, resulting in unnatural localized UI text.

This skill turns those recurring issues into practical review rules, so AI can produce design documentation that is clearer, cleaner, more useful, and more design-system-ready.

## What It Helps AI Do Better

- Write design specifications with clearer logic and less generic wording.
- Turn vague feedback into stable, team-facing rules.
- Consolidate messy tokens, states, categories, and component rules.
- Improve design-spec page layout, spacing, hierarchy, and alignment.
- Reduce unnecessary outlines, nested cards, grey blocks, and decorative containers.
- Keep new documentation modules consistent with the existing page system.
- Use real assets, real dimensions, and optical checks in examples.
- Support Chinese, English, and international product documentation.
- Balance designer readability with developer handoff clarity.

## What It Helps With

- Mobile app, mobile web, H5, and mini-program UI specifications
- Figma design-system documentation pages
- Color, typography, icon, spacing, and asset guidelines
- Component rules for buttons, forms, lists, tags, badges, feedback states, dialogs, and bottom sheets
- Localized Chinese and English UI copy
- Design-spec review, cleanup, consolidation, layout refinement, and content rewriting
- Turning messy design drafts into structured team-facing documentation

## Core Principles

### 1. User Feedback Is Not Final Spec Copy

Design feedback such as "this feels too rigid" or "this layout looks messy" is useful input, but it should not be pasted directly into a specification page.

The skill helps AI translate feedback into stable documentation language:

- what the rule is
- where it applies
- how it should be implemented
- what should remain flexible

### 2. Foundation Rules Should Stay Reusable

Color, typography, icon, and spacing rules should not be tied too narrowly to one button, one page, or one temporary use case.

The skill checks whether a rule:

- is too component-specific
- can be reused across scenarios
- has a clear semantic boundary
- leaves enough room for future adaptation

### 3. Consolidate Before Adding

Before creating a new token, color, type size, icon category, or rule, the skill encourages AI to check whether it can be merged into the existing system.

This prevents AI-generated design systems from becoming bloated, repetitive, and hard to maintain.

### 4. Better Layout Is Part Of Better Documentation

Design specifications are not only about what the rules say. They also need to be readable, scannable, and visually organized.

The skill helps AI improve documentation layout by checking:

- content width and side margins
- title hierarchy and section rhythm
- module spacing and inner padding
- text breathing room
- alignment between icons, labels, cards, and examples
- whether Auto Layout should be used for repeatable groups
- whether the page feels consistent with the rest of the design system

### 5. Use Hierarchy And Whitespace Before Extra Frames

Professional specification pages do not need a border around every idea.

The skill encourages:

- clear heading hierarchy
- consistent spacing
- real component examples
- fewer nested cards and decorative containers
- layouts that feel like one coherent documentation system

### 6. New Sections Must Inherit The Existing Page System

When adding new content to a design-spec page, the skill checks whether it follows the existing page structure:

- page width
- content width
- side margins
- type scale
- section rhythm
- Auto Layout behavior
- alignment with previous and next pages

### 7. Examples Must Be Verified By Real Visual Effect

Design-spec examples should not only be present. They should be visually reliable.

The skill reminds AI to check:

- real asset usage
- real dimensions
- optical icon alignment
- text breathing room
- clipped or crowded labels
- missing asset counts
- clear and stable naming

## Locale-Aware By Default

This skill does not assume every product is Chinese or English.

It chooses language based on product context:

- Chinese products use natural Chinese UI copy and design-spec wording.
- English or international products use natural English UI copy and design-spec wording.
- If the locale is unclear, guidance stays language-neutral and avoids forcing one language's examples.

## Repository Structure

```text
mobile-ui-spec/
  SKILL.md
  references/
    spec-quality.md
    mobile-layout.md
    localized-copywriting.md
    component-rules.md
    design-spec-docs.md
    review-checklist.md
  agents/
    openai.yaml
  README.md
```

## File Guide

`SKILL.md`  
The entry point of the skill. It explains when the skill should be used and which reference files should be loaded for each type of task.

`references/spec-quality.md`  
Guidance for judging whether a UI specification is professional, reasonable, adaptable, and implementable.

`references/mobile-layout.md`  
Mobile layout rules for navigation, density, touch targets, safe areas, keyboards, bottom actions, and responsive behavior.

`references/localized-copywriting.md`  
Localized UI copywriting guidance for Chinese and English product interfaces.

`references/component-rules.md`  
Component rules for buttons, lists, forms, search, filters, dialogs, bottom sheets, feedback, icons, tags, and badges.

`references/design-spec-docs.md`  
Rules for creating and reviewing Figma design-system documentation pages, including layout, Auto Layout, asset display, and page QA.

`references/review-checklist.md`  
A final checklist for reviewing UI specifications and design documentation before delivery.

`agents/openai.yaml`  
Metadata used by Codex/OpenAI interfaces to display the skill name, description, and default prompt.

## How To Use

Place the entire `mobile-ui-spec` folder in your Codex skills directory.

Example prompts:

```text
Use mobile-ui-spec to review this design specification page.
```

```text
Use mobile-ui-spec to make this color guideline more practical and design-system-ready.
```

```text
Use mobile-ui-spec to improve the layout and hierarchy of this Figma design-system documentation page.
```

```text
Use mobile-ui-spec to refine these icon rules and make them easier for designers and developers to apply.
```

## Who It Is For

- UI/UX designers building design systems
- Designers turning messy design drafts into reusable rules
- Teams using AI to write or improve design documentation
- Product teams working across Chinese and English interfaces
- Designers who care about both visual quality and implementation handoff
- Anyone who wants AI to produce cleaner design-spec layouts, not just longer design-spec text

## What It Is Not

This is not a complete design-system template, and it does not decide your brand style for you.

It is a judgment framework that helps AI avoid common design-spec mistakes:

- adding too many rules
- writing generic documentation
- over-constraining tokens
- ignoring existing systems
- ignoring developer handoff
- making pages look polished but hard to use
- creating documentation layouts that are misaligned, crowded, or visually inconsistent

---

## 中文说明

Mobile UI Spec 是一个帮助 AI 更好生成、审查和优化移动端 UI 设计规范的 skill。

它关注的不是“让 AI 写出一堆看起来像规范的文字”，而是让 AI 在输出前先做设计判断：规则是否合理、是否可复用、是否容易维护、排版是否清晰、是否能被设计师和开发真正使用。

它尤其适合这些场景：

- 整理 Figma 设计系统规范页
- 优化颜色、字体、图标、间距等基础规范
- 收敛混乱的 token、组件状态和图标分类
- 把口头反馈转译成专业规范语言
- 帮助 AI 更好处理规范页排版、层级、留白和模块对齐
- 检查规范页是否符合已有页面系统
- 优化中文和英文 UI 文案的本地化表达

这个 skill 的目标是让 AI 少产出模板化、堆砌式、难落地的设计规范，多产出清晰、克制、排版稳定、可维护、适合团队协作的设计文档。

## License

MIT
