---
name: "Purpose (Intention)"
description: "Deep dive into Apple's Purpose design principle — starting with intention, focusing on what matters, and knowing what not to build."
tags: [purpose, intention, focus, prioritization, human-centered]
---

## Core Idea

Start with intention. Focus on what matters most to people and build features they truly value. Identify what to build by deciding what not to include; do not waste user time, attention, or trust.

## Key Questions

- What problem does this feature solve, and is it a problem worth solving?
- Who is the primary user, and what is their core goal?
- What features can we explicitly **not** build to preserve focus?

## Patterns

### Feature Selection
Every feature asks for a person's time, attention, and trust. Evaluate each potential feature against a clear product north star. If a feature does not directly serve the user's primary goal, deprioritize it.

### Progressive Disclosure
Show only what is needed at each step. Reveal advanced options when the user signals readiness (e.g., tapping "More options" or after completing a primary action).

### Onboarding as Purpose
The onboarding experience should communicate the app's purpose in seconds. Avoid feature-dump tutorials. Instead, let users accomplish a meaningful task immediately.

## Anti-Patterns

- **Feature creep:** Adding features to match competitors without evaluating user value.
- **Blank slate:** Leaving new users with an empty interface and no guidance on what to do first.
- **Notification overload:** Pushing irrelevant updates that train users to ignore notifications entirely.

## Best Practices

- Define a single primary action per screen.
- Remove or hide features that fewer than 10% of users access.
- Test whether removing a feature negatively impacts core task completion before finalizing.
