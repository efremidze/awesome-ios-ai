# Contributing to Awesome iOS AI

Thanks for contributing! This list is community-maintained — skill authors and iOS developers are encouraged to submit PRs.

## Adding a Skill

### Requirements

Your skill must:

1. **Target iOS, Swift, or SwiftUI specifically** — general-purpose skills don't belong here
2. **Be installable** via `npx skills add` or manually from a public GitHub repo
3. **Pass security audit** on [skills.sh](https://skills.sh/) (Safe or Low Risk)
4. **Have a working SKILL.md** following the [Agent Skills specification](https://agentskills.io/specification)
5. **Actually work** — we test skills before merging

### How to Submit

1. Fork this repository
2. Add your skill to the appropriate category table in `README.md`
3. Follow the existing table format:
   ```
   | [Skill Name](skills.sh link) | [Author](github profile) | install count | One-line description. |
   ```
4. Add an install command inside the category's `<details>` block
5. Submit a PR using the [pull request template](.github/PULL_REQUEST_TEMPLATE.md)

### Choosing a Category

| Category | What belongs here |
|----------|-------------------|
| SwiftUI | View composition, state management, performance, UI patterns, platform design |
| Swift Concurrency | async/await, actors, Sendable, data-race safety |
| Testing | Swift Testing, XCTest, test patterns |
| Debugging | Simulator, Xcode build, runtime inspection, logging |
| Design & Platform | HIG, platform APIs, design patterns, architecture |
| Workflow & Automation | Release notes, issue workflows, CI/CD, packaging |
| Accessibility | VoiceOver, Dynamic Type, accessibility traits, assistive technology |
| MCP Servers | External tool integrations for iOS development |

If your skill doesn't fit an existing category, propose a new one in your PR description.

## Adding an MCP Server

MCP servers that are specifically useful for iOS/Swift development are welcome. Include:

- Name and link
- One-line description
- What it enables for iOS devs

## Updating Existing Entries

If you're the author of a listed skill and want to update the description or links, submit a PR. If install counts are significantly outdated, feel free to update those too.

## Quality Standards

We prioritize:

- **Author credibility** — Skills from known Swift community members or organizations get priority
- **Install count** — Higher adoption signals quality (but new skills from credible authors are welcome)
- **Security** — Must pass skills.sh security audit
- **Specificity** — Focused skills that do one thing well over broad skills that do many things loosely
- **Accessibility** — Skills that produce accessible code get bonus points

## What We Don't Accept

- Skills that aren't specific to iOS/Swift development
- Skills that are wrappers around obvious prompts with no real reference material
- Skills with known security issues
- Duplicate submissions of already-listed skills
- Self-promotional content that isn't a genuine skill

## Code of Conduct

Be respectful. This is a community resource. We follow the [Contributor Covenant](https://www.contributor-covenant.org/version/2/1/code_of_conduct/).

## Questions?

Open an issue if you're unsure whether your skill fits or have questions about the submission process.
