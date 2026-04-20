# drmike-swe-plugin

A custom Claude Code plugin for software engineering workflows.

## Structure

- **agents/** — Custom agents with specialized system prompts and tool configurations
- **commands/** — Slash commands available in Claude Code sessions
  - `/greeting` — Greets the user and identifies the plugin as the source
- **hooks/** — Lifecycle event hooks
  - `SessionStart.sh` — Displays a friendly welcome message at the start of every session
- **skills/** — Reusable skill definitions loaded into Claude's context

## Usage

Install this plugin via your Claude Code settings to activate the custom commands, hooks, and skills in your sessions.
