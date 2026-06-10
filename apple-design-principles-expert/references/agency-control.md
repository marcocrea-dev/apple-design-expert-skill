---
name: "Agency (Control)"
description: "Deep dive into Apple's Agency design principle — putting people in control, offering choices, and building forgiveness."
tags: [agency, control, autonomy, forgiveness, undo, user-control]
---

## Core Idea

Put people in control. Offer choices instead of guiding users down a single predetermined path. Provide autonomy for users to explore at their own pace and forgiveness by making it easy to undo actions and recover from mistakes.

## Key Questions

- Can the user choose their own path, or are they forced into a flow?
- Is every destructive action reversible or confirmed?
- Does the user feel confident exploring, or afraid of making a mistake?

## Patterns

### Undo Everywhere
Support undo for all destructive and state-changing actions. The ideal undo is immediate (shake to undo, ⌘Z, or a visible "Undo" banner). For actions that cannot be undone, require explicit confirmation.

### Non-Modal Exploration
Prefer non-modal interfaces that let users explore freely. Avoid full-screen modals for actions that are part of a larger workflow.

### Defaults with Escape Hatches
Set intelligent defaults based on context but allow the user to override them easily. The default should serve the majority without trapping the minority.

## Anti-Patterns

- **Wizard-style flows:** Forcing users through a linear, unskippable setup process.
- **Hidden destructive actions:** Placing "Delete" or "Log out" where accidental taps are easy (no confirmation, no undo).
- **No escape from automation:** An AI-driven feature that executes without preview or the ability to reject its output.

## Best Practices

- Every action that modifies data should have an undo path.
- Use confirmation dialogs only for genuinely destructive actions — not as a crutch for poor defaults.
- Allow users to customize their experience, even if the default serves most people.
