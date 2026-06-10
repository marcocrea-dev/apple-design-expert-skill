---
name: "Responsibility (Trust)"
description: "Deep dive into Apple's Responsibility design principle — acting in the user's best interest, prioritizing privacy, and implementing AI safeguards."
tags: [responsibility, trust, privacy, safety, ai-safeguards, transparency]
---

## Core Idea

Act in the user's best interest. Prioritize privacy (ask for data only when necessary and be transparent) and safety. For AI-driven features, anticipate unexpected or inaccurate outputs and implement safeguards (previews, confirmations, or disclaimers) to prevent real-world harm.

## Key Questions

- Does this feature need this data, or is the request optional?
- Is the user aware of what data is being collected and why?
- What is the worst plausible outcome of an AI feature misbehaving, and is there a safeguard?

## Patterns

### On-Device Processing
Prefer on-device machine learning over cloud-based processing when possible. This reduces data exposure and improves responsiveness. When cloud processing is required, anonymize and minimize the data sent.

### Granular Permissions
Ask for permissions in context, not at first launch. Use purpose strings that explain why access is needed. Support granular toggles (e.g., "Allow once" vs. "Allow while using").

### AI Transparency
Label AI-generated or AI-assisted content clearly. Provide a way for users to understand what the AI did and why. Include a feedback mechanism for incorrect outputs.

## Anti-Patterns

- **Permission shotgun:** Requesting all permissions at first launch before the user understands value.
- **Dark patterns:** Using confusing language or UI tricks to get users to consent to data collection.
- **Black-box AI:** An AI feature that makes decisions or generates content without showing its reasoning or offering a manual override.

## Best Practices

- Request permissions only when the user triggers a feature that needs them.
- Write permission purpose strings that are specific and human-readable.
- For AI features, always provide a preview of what will happen before execution.
- Log and review AI output failures to continuously improve safeguards.
