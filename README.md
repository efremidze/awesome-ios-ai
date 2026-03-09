# Awesome iOS AI [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> AI agent skills, agent teams, MCP servers, and tools that make AI coding assistants better at Swift and iOS development.

## Contents

- [Skills](#skills)
- [Agents](#agents)
- [MCP Servers](#mcp-servers)
- [Resources](#resources)

## Skills

[Agent Skills](https://agentskills.io/) are an open standard for giving AI coding agents specialized knowledge. A skill is a folder containing instructions, reference docs, and scripts that an agent loads on demand when it detects a relevant task. Skills work across GitHub Copilot, Claude Code, Cursor, Codex, and more.

Install any skill with the [skills CLI](https://skills.sh/docs/cli): `npx skills add <owner/repo@skill-name> -g -y`

### SwiftUI

- [SwiftUI Expert](https://skills.sh/avdlee/swiftui-agent-skill/swiftui-expert-skill) - State management, view composition, performance, iOS 26+ Liquid Glass. By Antoine van der Lee.
- [SwiftUI Pro](https://skills.sh/twostraws/swiftui-agent-skill/swiftui-pro) - Modern APIs, accessibility, data flow, navigation, and performance. By Paul Hudson.
- [SwiftUI Performance Audit](https://skills.sh/dimillian/skills/swiftui-performance-audit) - Diagnose slow rendering, janky scrolling, excessive view updates, and layout thrash. By Thomas Ricouard.
- [SwiftUI View Refactor](https://skills.sh/dimillian/skills/swiftui-view-refactor) - Consistent view structure, MV patterns, @Observable usage, dependency injection. By Thomas Ricouard.
- [SwiftUI UI Patterns](https://skills.sh/dimillian/skills/swiftui-ui-patterns) - Component references for TabView, NavigationStack, Sheets, and view composition. By Thomas Ricouard.
- [SwiftUI Liquid Glass](https://skills.sh/dimillian/skills/swiftui-liquid-glass) - iOS 26+ Liquid Glass API with `glassEffect`, `GlassEffectContainer`, and availability fallbacks. By Thomas Ricouard.

### Swift Concurrency

- [Swift Concurrency](https://skills.sh/avdlee/swift-concurrency-agent-skill/swift-concurrency) - Async/await, actors, Sendable, and strict concurrency. By Antoine van der Lee.
- [Swift Concurrency Expert](https://skills.sh/dimillian/skills/swift-concurrency-expert) - Swift 6.2+ focused. Actor isolation, data-race safety, minimal-change fixes for compiler errors. By Thomas Ricouard.

### Testing

- [Swift Testing Expert](https://skills.sh/avdlee/swift-testing-agent-skill/swift-testing-expert) - Modern Swift Testing framework with `#expect`, `#require`, traits, tags, parameterized tests, and XCTest migration. By Antoine van der Lee.

### Debugging

- [iOS Debugger Agent](https://skills.sh/dimillian/skills/ios-debugger-agent) - Build, run, and debug iOS apps on simulators via XcodeBuildMCP. By Thomas Ricouard.

### Design and Platform

- [iOS HIG](https://skills.sh/johnrogers/claude-swift-engineering/ios-hig) - Apple Human Interface Guidelines compliance. By johnrogers.
- [iOS 26 Platform](https://skills.sh/johnrogers/claude-swift-engineering/ios-26-platform) - Platform APIs and patterns for iOS 26. By johnrogers.
- [Mobile iOS Design](https://skills.sh/wshobson/agents/mobile-ios-design) - iOS design patterns and architecture. By wshobson.

### Workflow and Automation

- [App Store Changelog](https://github.com/Dimillian/Skills/tree/main/app-store-changelog) - Generate App Store release notes from Git history. By Thomas Ricouard.
- [GH Issue Fix Flow](https://github.com/Dimillian/Skills/tree/main/github) - End-to-end GitHub issue resolution with read, fix, build, test, and push. By Thomas Ricouard.
- [macOS SwiftPM Packaging](https://github.com/Dimillian/Skills/tree/main/macos-spm-app-packaging) - Scaffold, build, and package SwiftPM macOS apps without Xcode. By Thomas Ricouard.
- [Swift MCP Server Generator](https://skills.sh/github/awesome-copilot/swift-mcp-server-generator) - Generate MCP servers in Swift. By GitHub.

### Accessibility

- [iOS Accessibility](https://skills.sh/dpearson2699/swift-ios-skills/ios-accessibility) - Accessibility patterns and VoiceOver support for iOS. By dpearson2699.
- [Swift Accessibility](https://skills.sh/madebyecho/agent-skills/swift-accessibility) - Accessibility guidance for Swift apps. By madebyecho.

## Agents

- [Swift Agents](https://github.com/Techopolis/swift-agents) - 16 orchestrated specialists covering concurrency, SwiftUI, accessibility, security, testing, StoreKit, SwiftData, visionOS, Core ML, MLX, and Foundation Models. Works with Claude Code and VS Code Copilot.

## MCP Servers

- [XcodeBuildMCP](https://github.com/nicklama/xcode-build-mcp) - Build, run, and test Xcode projects from AI agents.
- [Sosumi MCP](https://github.com/kanaa257/sosumi.ai) - Access Apple developer documentation from AI agents.
- [awesome-copilot MCP](https://github.com/github/awesome-copilot) - Search and install agents, skills, and instructions from GitHub.

## Resources

- [skills.sh](https://skills.sh) - Searchable directory of all agent skills with install counts and security audits.
- [Agent Skills Specification](https://agentskills.io/specification) - The open standard for building skills.
- [VS Code Copilot Customization](https://code.visualstudio.com/docs/copilot/copilot-customization) - Official guide for workspace instructions, agents, prompts, hooks, and skills.

## Contributing

Contributions welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a PR.
