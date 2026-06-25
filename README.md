# SF Compute Agent Skills and Plugin

Skills and plugin for AI agents working with SF Compute

## Install

### npx skills

```bash
# See what this repo contains
npx skills add sfcompute/skills --list

# Install all SF Compute skills globally (recommended)
npx skills add sfcompute/skills --global

# Install a specific SF Compute skill globally
npx skills add sfcompute/skills --global --skill sf-cli
```

Project-level installs are also supported. Omit `--global` if you want the skills scoped to the current repository instead of user-level.

### Claude Code

With Claude CLI:

```bash
claude plugin marketplace add sfcompute/skills
claude plugin install sfcompute@sfcompute-skills
```

Inside Claude CLI:

```bash
/plugin marketplace add sfcompute/skills
/plugin install sfcompute@sfcompute-skills
```

### Claude Desktop

1. Go to Customize
1. Hit the `+` button to add a personal plugin.
1. Select **Create plugin** and then **Add marketplace**. Select **Add from repository**.
1. Input `sfcompute/skills` and hit **Sync**.
1. When the UI refreshes, install the SF Compute plugin with the `+` b

After installation, try a task that should trigger one of the skills:

- "Install the SF Compute CLI and log me in."
- "List my SF Compute instances as JSON."
- "Check current GPU availability and pricing."
- "Buy compute for a training run this weekend."
- "Create an order to sell my idle capacity."
- Invoke using `/sf-cli`

## Features

Use this skill when you need to:

- install, upgrade, or authenticate the SF Compute CLI
- run CRUD operations on instances, orders, capacities, images and other resources
- check availability, billing, events, and limits
- buy or sell GPU compute from the terminal

Example prompts:

- "Install the SF Compute CLI on macOS."
- "Log into SF Compute and show my account."
- "Show GPU availability and create a buy order."
