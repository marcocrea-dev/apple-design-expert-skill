---
name: "Flexibility (Adaptability)"
description: "Deep dive into Apple's Flexibility design principle — adapting across contexts, devices, abilities, and supporting personalization."
tags: [flexibility, adaptability, accessibility, responsive, personalization, inclusion]
---

## Core Idea

Design for diverse contexts (mobile, desktop, hands-free) and wide ranges of abilities (inclusion and accessibility). Support personalization, allowing users to rearrange or hide controls to fit their own workflow.

## Key Questions

- Does this design work on the smallest and largest screen sizes for this platform?
- Can every function be accessed via keyboard, voice, and touch?
- Can users customize the interface to match their workflow?

## Patterns

### Responsive Layout
Use Auto Layout or SwiftUI's built-in adaptive layout to support all screen sizes. Test on the smallest and largest devices. Content should reflow, not simply scale.

### Accessibility First
Design with VoiceOver, Dynamic Type, and Reduced Motion in mind from the start — not as an afterthought. Every interactive element must have a descriptive accessibility label. Support full keyboard navigation on iPad and Mac.

### User Customization
Allow users to rearrange toolbars, reorder tabs, or hide infrequently used controls. Store preferences in iCloud so they sync across devices. Respect the user's choices as intentional signals.

## Anti-Patterns

- **Fixed-width layouts:** Designing only for one screen size and ignoring others.
- **Inaccessible animations:** Using motion that cannot be disabled or that conveys information without a text alternative.
- **Rigid navigation:** Forcing all users through the same menu structure with no reordering or hiding options.

## Best Practices

- Test with Dynamic Type at the largest accessibility size.
- Ensure all touch targets are at least 44x44 points.
- Provide alternate interaction methods for every action (e.g., drag-and-drop and a menu option).
- Support Split View and Stage Manager on iPad.
