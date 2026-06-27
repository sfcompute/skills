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

Invoke using `/sf-cli` on Claude.

### Codex CLI

```bash
codex plugin marketplace add sfcompute/skills
codex plugin install sfcompute@sfcompute-skills
```

### Codex Desktop

1. Click on Plugins in the left side bar
2. Hit the drop-down `next to the +` button and select 'Add Marketplace'
3. Input `sfcompute/skills` and click `Add marketplace`
4. Install `SF Compute` plugin

Use `@sfcompute` to invoke the plugin explicitly.

### Cursor

1. Go to `Settings` > `Plugins` in the desktop app
2. Paste `https://github.com/sfcompute/skills` in the text box with placeholder text that says "Search or Paste Link"
3. Click on the `SF Compute` plugin that appears and hit `Add to Cursor`

## Example prompts

- "Install the SF Compute CLI on macOS."
- "Log into SF Compute and show my account."
- "Show GPU availability and create a buy order."
- "Create a new capacity named golden-gate."
- "Buy compute for a training run this weekend."
