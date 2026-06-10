---
name: "Simplicity (Clarity)"
description: "Deep dive into Apple's Simplicity design principle — stripping away the unnecessary, using plain language, and establishing clear hierarchy."
tags: [simplicity, clarity, hierarchy, concise, plain-language, cognitive-load]
---

## Core Idea

Strip away the unnecessary so the core purpose shines. Simple does not mean minimal (do not just hide functionality); it means being concise, using plain language, and establishing a clear hierarchy (order, spacing, and contrast).

## Key Questions

- Can the user identify the primary action on this screen in under 2 seconds?
- Is every visible element earning its place, or is it noise?
- Does the language used require domain knowledge the user may not have?

## Patterns

### Visual Hierarchy
Use size, weight, color, and spacing to signal importance. The most important element should be the most visually prominent. Group related items and separate unrelated ones. Use depth (z-index, shadows) sparingly to layer information.

### Plain Language
Write copy at an 8th-grade reading level. Avoid jargon, technical terms, and brand-speak. Use active voice. Every label, button title, and error message should tell the user what happens next.

### Progressive Disclosure
Reveal complexity incrementally. Show the most common options by default. Nest advanced settings behind a clear affordance. The interface for a beginner should not overwhelm, but the expert should not feel capped.

## Anti-Patterns

- **Hiding complexity behind mystery meat:** Removing labels and relying solely on icons with no tooltip or label text.
- **Design-by-committee UI:** Every stakeholder's feature request on the same screen, competing for attention.
- **False simplicity:** Removing a necessary control and forcing users through three extra steps to accomplish the same task.

## Best Practices

- Each screen should have exactly one primary action button.
- Use white space intentionally to separate content groups.
- Reduce the number of choices at each decision point (Hick's Law).
- Every error message should explain what happened and what to do next.
