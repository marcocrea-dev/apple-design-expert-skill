---
name: "Familiarity (Intuition)"
description: "Deep dive into Apple's Familiarity design principle — building on what people already know, using metaphors, and maintaining consistency."
tags: [familiarity, intuition, metaphors, consistency, platform-conventions]
---

## Core Idea

Build on what people already know. Use metaphors from the real world or established software patterns (but avoid being too literal or too abstract). Maintain consistency: things that look the same must behave the same.

## Key Questions

- Does this interaction pattern exist on the platform already?
- Would a user who has never seen this feature understand what to do in under 3 seconds?
- Do similar-looking elements behave consistently across the app?

## Patterns

### Platform Alignment
Use standard platform components (navigation bars, tab bars, sheets, menus) as designed by the HIG. Users bring knowledge from every other app on the platform. Resist the urge to create custom components when system components suffice.

### Real-World Metaphors
Map digital interactions to physical world counterparts when it reduces learning (e.g., a trash can for deletion, a folder for grouping files). Avoid metaphors that are too literal (a rotary dial for a phone app) or too abstract (a geometric shape with no cultural referent).

### Visual Consistency
Elements with the same function should look identical across screens. Use SF Symbols for icons to ensure visual coherence and accessibility. Define a color palette and typography scale, then apply them systematically.

## Anti-Patterns

- **Custom gestures:** Defining new swipe or tap patterns that have no platform precedent and no discoverability.
- **Inconsistent icons:** Using different icons for the same action on different screens.
- **Skeuomorphism:** Recreating physical objects in detail (leatherstitch borders, paper textures) when the digital medium offers better alternatives.

## Best Practices

- Before building a custom component, confirm the system component cannot be adapted.
- Maintain a design system with documented components, colors, and typography.
- Use SF Symbols as your default icon set for platform consistency.
