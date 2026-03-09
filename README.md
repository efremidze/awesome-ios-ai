# Awesome iOS AI [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> AI agent skills, agent teams, MCP servers, and tools that make AI coding assistants better at Swift and iOS development.

Your AI coding tools write Swift like it is 2020. They use `ObservableObject` when `@Observable` exists. They ignore actor isolation. They produce views with no accessibility modifiers. They have never heard of Apple Foundation Models.

**Skills and agent teams fix that.** They give GitHub Copilot, Claude Code, Cursor, and Codex expert-level Swift and iOS knowledge on demand — so your AI writes modern, accessible, concurrent Swift the way it should be written.

We started this list while building the Swift Agent Team and realized no central resource existed for any of this. The skills listed here help us every day. This is a community effort — contributions welcome.

## Contents

- [What Are Skills](#what-are-skills)
- [How to Install](#how-to-install)
- [Skills](#skills)
  - [SwiftUI](#swiftui)
  - [Swift Concurrency](#swift-concurrency)
  - [Testing](#testing)
  - [Debugging](#debugging)
  - [Design & Platform](#design--platform)
  - [Workflow & Automation](#workflow--automation)
  - [Accessibility](#accessibility)
- [Agent Teams](#agent-teams)
- [MCP Servers](#mcp-servers)
- [Notable Authors](#notable-authors)
- [Resources](#resources)

## What Are Skills

[Agent Skills](https://agentskills.io/) are an open standard for giving AI coding agents specialized knowledge. A skill is a folder containing instructions, reference docs, and scripts that an agent loads on demand when it detects a relevant task.

Skills work across multiple tools — GitHub Copilot, Claude Code, Cursor, Codex, and many more.

## How to Install

Install any skill with a single command using the [skills CLI](https://skills.sh/docs/cli):

```bash
# Install a single skill globally (available in all projects)
npx skills add <owner/repo@skill-name> -g -y

# Install ALL skills from an author's repo at once
npx skills add <owner/repo> --all

# Search for skills
npx skills find swift
npx skills find swiftui
npx skills find ios
```

Browse all skills at **[skills.sh](https://skills.sh/?q=swift)**.

### Install Everything

Want the full iOS AI skill stack? Run these three commands to install all skills from the top authors:

```bash
# All skills from Antoine van der Lee (SwiftUI Expert, Concurrency, Testing)
npx skills add avdlee/swiftui-agent-skill --all
npx skills add avdlee/swift-concurrency-agent-skill --all
npx skills add avdlee/swift-testing-agent-skill --all

# All 10 skills from Thomas Ricouard (Performance, Liquid Glass, View Refactor, Debugger, and more)
npx skills add dimillian/skills --all

# SwiftUI Pro from Paul Hudson
npx skills add twostraws/swiftui-agent-skill --all
```

The `--all` flag installs every skill in the repo globally with no prompts.

### One-Command Install (Everything)

Install every skill from this list with a single command:

```bash
curl -fsSL https://raw.githubusercontent.com/techopolis-group/awesome-ios-ai/main/install.sh | bash
```

Or clone and run locally:

```bash
git clone https://github.com/techopolis-group/awesome-ios-ai.git
cd awesome-ios-ai
./install.sh
```

This installs all skills from Antoine van der Lee, Thomas Ricouard, and Paul Hudson — the complete iOS AI skill stack.

---

## Skills

### SwiftUI

| Skill | Author | Description |
|-------|--------|-------------|
| [SwiftUI Expert](https://skills.sh/avdlee/swiftui-agent-skill/swiftui-expert-skill) | [Antoine van der Lee](https://github.com/AvdLee) | State management, view composition, performance, iOS 26+ Liquid Glass. The most installed Swift skill. |
| [SwiftUI Pro](https://skills.sh/twostraws/swiftui-agent-skill/swiftui-pro) | [Paul Hudson](https://github.com/twostraws) | Comprehensive review covering modern APIs, accessibility, data flow, navigation, and performance. |
| [SwiftUI Performance Audit](https://skills.sh/dimillian/skills/swiftui-performance-audit) | [Thomas Ricouard](https://github.com/Dimillian) | Diagnose slow rendering, janky scrolling, excessive view updates, and layout thrash. |
| [SwiftUI View Refactor](https://skills.sh/dimillian/skills/swiftui-view-refactor) | [Thomas Ricouard](https://github.com/Dimillian) | Consistent view structure, MV patterns, @Observable usage, dependency injection. |
| [SwiftUI UI Patterns](https://skills.sh/dimillian/skills/swiftui-ui-patterns) | [Thomas Ricouard](https://github.com/Dimillian) | Component references for TabView, NavigationStack, Sheets, and view composition. |
| [SwiftUI Liquid Glass](https://skills.sh/dimillian/skills/swiftui-liquid-glass) | [Thomas Ricouard](https://github.com/Dimillian) | iOS 26+ Liquid Glass API — `glassEffect`, `GlassEffectContainer`, availability fallbacks. |

<details>
<summary><strong>Install all SwiftUI skills</strong></summary>

```bash
npx skills add avdlee/swiftui-agent-skill@swiftui-expert-skill -g -y
npx skills add twostraws/swiftui-agent-skill@swiftui-pro -g -y
npx skills add dimillian/skills@swiftui-performance-audit -g -y
npx skills add dimillian/skills@swiftui-view-refactor -g -y
npx skills add dimillian/skills@swiftui-ui-patterns -g -y
npx skills add dimillian/skills@swiftui-liquid-glass -g -y
```

</details>

### Swift Concurrency

| Skill | Author | Description |
|-------|--------|-------------|
| [Swift Concurrency](https://skills.sh/avdlee/swift-concurrency-agent-skill/swift-concurrency) | [Antoine van der Lee](https://github.com/AvdLee) | async/await, actors, Sendable, strict concurrency. |
| [Swift Concurrency Expert](https://skills.sh/dimillian/skills/swift-concurrency-expert) | [Thomas Ricouard](https://github.com/Dimillian) | Swift 6.2+ focused. Actor isolation, data-race safety, minimal-change fixes for compiler errors. |

<details>
<summary><strong>Install all Concurrency skills</strong></summary>

```bash
npx skills add avdlee/swift-concurrency-agent-skill@swift-concurrency -g -y
npx skills add dimillian/skills@swift-concurrency-expert -g -y
```

</details>

### Testing

| Skill | Author | Description |
|-------|--------|-------------|
| [Swift Testing Expert](https://skills.sh/avdlee/swift-testing-agent-skill/swift-testing-expert) | [Antoine van der Lee](https://github.com/AvdLee) | Modern Swift Testing framework — `#expect`, `#require`, traits, tags, parameterized tests, XCTest migration. |

<details>
<summary><strong>Install</strong></summary>

```bash
npx skills add avdlee/swift-testing-agent-skill@swift-testing-expert -g -y
```

</details>

### Debugging

| Skill | Author | Description |
|-------|--------|-------------|
| [iOS Debugger Agent](https://skills.sh/dimillian/skills/ios-debugger-agent) | [Thomas Ricouard](https://github.com/Dimillian) | Build, run, and debug iOS apps on simulators via XcodeBuildMCP. UI interaction, log capture, screenshots. |

<details>
<summary><strong>Install</strong></summary>

```bash
npx skills add dimillian/skills@ios-debugger-agent -g -y
```

</details>

### Design & Platform

| Skill | Author | Description |
|-------|--------|-------------|
| [iOS HIG](https://skills.sh/johnrogers/claude-swift-engineering/ios-hig) | johnrogers | Apple Human Interface Guidelines compliance. |
| [iOS 26 Platform](https://skills.sh/johnrogers/claude-swift-engineering/ios-26-platform) | johnrogers | iOS 26 platform APIs and patterns. |
| [Mobile iOS Design](https://skills.sh/wshobson/agents/mobile-ios-design) | wshobson | iOS design patterns and architecture. |

<details>
<summary><strong>Install all Design skills</strong></summary>

```bash
npx skills add johnrogers/claude-swift-engineering@ios-hig -g -y
npx skills add johnrogers/claude-swift-engineering@ios-26-platform -g -y
npx skills add wshobson/agents@mobile-ios-design -g -y
```

</details>

### Workflow & Automation

| Skill | Author | Description |
|-------|--------|-------------|
| [App Store Changelog](https://github.com/Dimillian/Skills/tree/main/app-store-changelog) | [Thomas Ricouard](https://github.com/Dimillian) | Generate App Store release notes from git history. |
| [GH Issue Fix Flow](https://github.com/Dimillian/Skills/tree/main/github) | [Thomas Ricouard](https://github.com/Dimillian) | End-to-end GitHub issue resolution — read, fix, build, test, push. |
| [macOS SwiftPM Packaging](https://github.com/Dimillian/Skills/tree/main/macos-spm-app-packaging) | [Thomas Ricouard](https://github.com/Dimillian) | Scaffold, build, and package SwiftPM macOS apps without Xcode. |
| [Swift MCP Server Generator](https://skills.sh/github/awesome-copilot/swift-mcp-server-generator) | [GitHub](https://github.com/github/awesome-copilot) | Generate MCP servers in Swift. |

<details>
<summary><strong>Install all Workflow skills</strong></summary>

```bash
npx skills add dimillian/skills@app-store-changelog -g -y
npx skills add dimillian/skills@github -g -y
npx skills add dimillian/skills@macos-spm-app-packaging -g -y
npx skills add github/awesome-copilot@swift-mcp-server-generator -g -y
```

</details>

### Accessibility

| Skill | Author | Description |
|-------|--------|-------------|
| [iOS Accessibility](https://skills.sh/dpearson2699/swift-ios-skills/ios-accessibility) | dpearson2699 | iOS accessibility patterns and VoiceOver support. |
| [Swift Accessibility](https://skills.sh/madebyecho/agent-skills/swift-accessibility) | madebyecho | Swift accessibility guidance. |

> **Note:** The SwiftUI Pro and SwiftUI Expert skills listed above also include accessibility coverage (Dynamic Type, VoiceOver labels, Reduce Motion, button traits).

---

## Agent Teams

Skills give agents knowledge. Agent teams take it further with coordinated specialists and an orchestrator that routes tasks to the right expert automatically. If you have built an agent team for iOS or Swift development, submit it.

- **[Swift Agent Team](https://github.com/techopolis-group/swift-agent-team)** — 16 orchestrated specialists covering concurrency, SwiftUI, accessibility, security, testing, StoreKit, SwiftData, visionOS, Core ML, MLX, Foundation Models, and more. A swift-lead routes every task to the right experts. Works with Claude Code and VS Code Copilot. Uses companion skills from this list as its knowledge base.

---

## MCP Servers

MCP (Model Context Protocol) servers give AI agents access to external tools and data sources.

| Server | Description |
|--------|-------------|
| [XcodeBuildMCP](https://github.com/nicklama/xcode-build-mcp) | Build, run, and test Xcode projects from AI agents. Required by the iOS Debugger Agent skill. |
| [Sosumi MCP](https://github.com/kanaa257/sosumi.ai) | Access Apple developer documentation from AI agents. |
| [awesome-copilot MCP](https://github.com/github/awesome-copilot) | Search and install agents, skills, and instructions from GitHub's curated collection. |

---

## Notable Authors

These developers maintain the most impactful iOS AI skills:

### [Antoine van der Lee](https://github.com/AvdLee) ([@twannl](https://x.com/twannl))

Author of [SwiftLee](https://www.avanderlee.com/) — one of the most widely-read Swift blogs. Maintains the top-installed Swift skills across SwiftUI, Concurrency, Testing, and Core Data. His skills are the gold standard for the ecosystem.

- [SwiftUI Expert Skill](https://github.com/AvdLee/SwiftUI-Agent-Skill) — 2.1K stars
- [Swift Concurrency Skill](https://github.com/AvdLee/Swift-Concurrency-Agent-Skill)
- [Swift Testing Skill](https://github.com/AvdLee/Swift-Testing-Agent-Skill)
- [Core Data Skill](https://github.com/AvdLee/Core-Data-Agent-Skill)

<details>
<summary><strong>Install all Antoine's skills</strong></summary>

```bash
npx skills add avdlee/swiftui-agent-skill --all
npx skills add avdlee/swift-concurrency-agent-skill --all
npx skills add avdlee/swift-testing-agent-skill --all
```

</details>

### [Thomas Ricouard](https://github.com/Dimillian) ([@dimillian](https://x.com/dimillian))

Creator of [IceCubes](https://github.com/Dimillian/IceCubeApp), one of the largest open-source SwiftUI apps. His [Skills repo](https://github.com/Dimillian/Skills) (2K stars) is the most comprehensive iOS-specific skills collection, covering performance, Liquid Glass, view patterns, concurrency, debugging, and workflow automation.

- [Dimillian/Skills](https://github.com/Dimillian/Skills) — 10 skills, 2K stars
- [Skills documentation site](https://dimillian.github.io/Skills/)

<details>
<summary><strong>Install all Thomas's skills (all 10 at once)</strong></summary>

```bash
npx skills add dimillian/skills --all
```

This single command installs: SwiftUI Performance Audit, SwiftUI Liquid Glass, SwiftUI View Refactor, SwiftUI UI Patterns, Swift Concurrency Expert, iOS Debugger Agent, App Store Changelog, GH Issue Fix Flow, macOS SwiftPM Packaging, and the GitHub CLI skill.

</details>

### [Paul Hudson](https://github.com/twostraws) ([@twostraws](https://x.com/twostraws))

Creator of [Hacking with Swift](https://www.hackingwithswift.com/) — the most popular Swift learning resource. His SwiftUI Pro skill brings his teaching expertise to AI agents with comprehensive reference docs covering APIs, accessibility, data flow, design, navigation, and performance.

- [SwiftUI Agent Skill](https://github.com/twostraws/swiftui-agent-skill)

<details>
<summary><strong>Install Paul's skills</strong></summary>

```bash
npx skills add twostraws/swiftui-agent-skill --all
```

</details>

---

## Resources

### Directories & Registries

- [skills.sh](https://skills.sh) — Searchable directory of all agent skills with install counts and security audits.
- [Agent Skills Specification](https://agentskills.io/specification) — The open standard for building skills.

### Guides

- [VS Code Copilot Customization](https://code.visualstudio.com/docs/copilot/copilot-customization) — Official guide for workspace instructions, agents, prompts, hooks, and skills.

---

## Contributing

Contributions welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a PR.

**Skill authors:** Submit your iOS and Swift skills. See the contributing guide for requirements.

**Agent team authors:** Built an agent team for Swift development? Add it to the Agent Teams section.

---

## Footnotes

Created by [Taylor Arndt](https://github.com/taylorarndt). Maintained by [Techopolis](https://github.com/techopolis-group).
