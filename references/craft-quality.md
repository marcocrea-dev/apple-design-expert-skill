---
name: "Craft (Quality)"
description: "Deep dive into Apple's Craft design principle — attention to detail, beautiful materials, fluid motion, and iterative refinement."
tags: [craft, quality, typography, animation, motion, iteration, polish]
---

## Core Idea

Show you care through attention to detail. Use high-quality materials: beautiful fonts, thoughtful colors, and fluid, responsive animations. Iterate and prototype early, testing in real-world settings to ensure the software feels solid, not fragile.

## Key Questions

- Does every animation serve a purpose, or is it decorative?
- Do transitions feel responsive (under 300ms) and interruptible?
- Does the app feel just as polished in edge cases as in the happy path?

## Patterns

### Fluid Motion
Use system animation frameworks (SwiftUI animations, UIKit spring animations) with natural curves. Animations should be interruptible and responsive. A 200-300ms duration feels instantaneous while providing orientation. Respect `prefers-reduced-motion` and provide a static alternative.

### Typographic Care
Use Dynamic Type to support all font sizes. Choose a typeface that matches the app's personality (San Francisco for system apps). Pay attention to line height, kerning, and readability at every size.

### Edge Case Polish
The true test of craft is how the app behaves at boundaries: empty states, loading states, error states, and maximum data volume. Each should be deliberately designed, not left as a system default.

## Anti-Patterns

- **Ornamental animation:** A 1-second logo animation on every launch that makes the app feel slower.
- **Unpolished empty states:** A blank white screen when there is no data, with no guidance for the user.
- **Janky transitions:** Stuttering animations, dropped frames, or layout shifts during navigation.

## Best Practices

- Prototype and test animations on device, not just in simulators.
- Design empty, loading, error, and success states before the happy path.
- Run performance tests (frame rate, memory) on the oldest supported device.
- Use spring animations with a damping ratio close to 1.0 for natural-feeling motion.
