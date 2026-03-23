<div align="center">
  <h1>Squidward3n</h1>
  <p>Desktop command center for orchestrating multiple AI coding agents working in parallel on Azure DevOps tickets and pull requests.</p>
</div>

## Overview

Squidward3n manages the full lifecycle of AI-assisted development — from assigning Azure DevOps work items to Claude Code agents, through code review and PR creation. Run multiple agents in parallel, each in their own cloned repo, with full visibility and control from a single dashboard.

## Features

### Agent Pools
- Create pools from a git clone URL — agents are cloned and configured automatically
- Auto-scaling maintains a minimum number of idle agents ready for work
- Agents get themed names (Star Wars, Ninja Turtles, Jungle Book)

### Ticket Workflow
- Browse Azure DevOps tickets and assign them to available agents
- Agents create branches, write code, self-review, and submit for human review
- Configurable acceptance scripts per project (e.g. `yarn test && yarn build`)
- Interactive permission approval — Allow or Deny tool usage in real-time
- Model and permission mode selection per task

### PR Review Assistant
- View pull requests assigned to you across multiple projects
- Spawn an agent to analyse any PR with structured findings:
  - Key changes and risk assessment
  - Issues detected (bugs, security, breaking changes)
  - Test coverage gaps
  - Suggested review order
- Ask follow-up questions with an inline chat

### Dashboard
- Live overview: In Progress, Awaiting Review, Needs Input, Review Assist, Idle
- Desktop notifications for permission requests and review submissions
- Click any card to jump to detail or review panel
- Unified activity feed with collapsible working sections between agent messages

## Screenshots

*Coming soon*

## Requirements

- **Claude Code CLI** — `npm install -g @anthropic-ai/claude-code`
- **Anthropic API key** configured in Claude Code
- **Azure DevOps** account with a Personal Access Token
- **Git** installed and available on PATH

## Coming soon 

Squidward3n currently supports Azure DevOps and Claude Code. We're working on making it platform-agnostic so you can use it with your existing tools.

**DevOps Platforms**
- GitHub (Issues, Projects, Pull Requests)
- GitLab (Issues, Merge Requests)
- Jira + Bitbucket

**AI Agents**
- OpenAI Codex
- Google Gemini
- Amazon Q Developer
- Locally run models

**Code Editors**
- VS Code (current)
- JetBrains IDEs
- Cursor
- Windsurf

Have a platform you'd like to see supported? Open an issue and let us know.

## Installation

Download the latest release for your platform from the [Releases](https://github.com/RobertScholey98/Squidward3n/releases) page:

| Platform | Format |
|----------|--------|
| macOS (Apple Silicon + Intel) | `.dmg` |
| Windows | `.exe` (NSIS installer) |
| Linux | `.AppImage` |

## License

Copyright (c) 2026 Rob Scholey. All rights reserved.

This software is proprietary. Unauthorized copying, modification, or distribution is prohibited.
