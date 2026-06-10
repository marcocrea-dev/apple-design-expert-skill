# Apple Design Principles Expert

An agent skill for evaluating, guiding, and generating UX solutions grounded in Apple's **"Principles of Great Design."** Apply Apple's 8 design pillars — Purpose, Agency, Responsibility, Familiarity, Flexibility, Simplicity, Craft, and Delight — to any design review, UI feedback, interaction critique, or usability evaluation.

## Overview

This skill transforms an AI agent into a Senior Design Agent specialized in Apple's Human Interface philosophy. It provides:

- **The 8 Pillars framework** — a structured lens for analyzing and critiquing interfaces
- **Operational directives** — rules for applying the framework during agentic workflows
- **Anti-patterns** — examples of common misapplications to avoid
- **Deep reference docs** — one file per pillar with detailed guidance

## Quick Start

Load the skill in your agent and then:

```
/evaluate: Check a login screen against all 8 pillars
/generate: Propose an onboarding flow following Apple's design principles
/critique: Review a settings page for Responsibility and Simplicity
```

When tasked with design work, the agent will:

1. Understand the context (platform, user goal, business objective)
2. Map to the 3–4 most relevant pillars
3. Weigh conflicts between competing principles
4. Generate a solution or evaluation with specific UI patterns
5. Format output under pillar headings with a final **Design Rationale**

## Installation

### Via npx skills

```bash
npx skills add marcocrea-dev/apple-design-expert-skill --skill apple-design-principles-expert
```

### Via Claude Code plugin

```bash
/plugin add marcocrea-dev/apple-design-expert-skill
```

> Claude Code plugins are also supported in Factory's [Droid](https://docs.factory.ai/cli/configuration/plugins#claude-code-compatibility).

### Via Playbooks

```bash
npx playbooks add skill marcocrea-dev/apple-design-expert-skill
```

## Reference Documentation

| Pillar | File |
|--------|------|
| Purpose (Intention) | [apple-design-principles-expert/references/purpose-intention.md](apple-design-principles-expert/references/purpose-intention.md) |
| Agency (Control) | [apple-design-principles-expert/references/agency-control.md](apple-design-principles-expert/references/agency-control.md) |
| Responsibility (Trust) | [apple-design-principles-expert/references/responsibility-trust.md](apple-design-principles-expert/references/responsibility-trust.md) |
| Familiarity (Intuition) | [apple-design-principles-expert/references/familiarity-intuition.md](apple-design-principles-expert/references/familiarity-intuition.md) |
| Flexibility (Adaptability) | [apple-design-principles-expert/references/flexibility-adaptability.md](apple-design-principles-expert/references/flexibility-adaptability.md) |
| Simplicity (Clarity) | [apple-design-principles-expert/references/simplicity-clarity.md](apple-design-principles-expert/references/simplicity-clarity.md) |
| Craft (Quality) | [apple-design-principles-expert/references/craft-quality.md](apple-design-principles-expert/references/craft-quality.md) |
| Delight (Humanity) | [apple-design-principles-expert/references/delight-humanity.md](apple-design-principles-expert/references/delight-humanity.md) |
| Design Review Checklist | [apple-design-principles-expert/references/design-review-checklist.md](apple-design-principles-expert/references/design-review-checklist.md) |

## Resources

- [Apple Human Interface Guidelines](https://developer.apple.com/design/human-interface-guidelines)
- [Apple Design Resources](https://developer.apple.com/design/resources)
- [SF Symbols](https://developer.apple.com/sf-symbols)
- [Agent Skills Specification](https://agentskills.io/specification)

## License

MIT — See [LICENSE](./LICENSE) in the repository root.
