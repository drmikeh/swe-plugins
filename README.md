# drmike-plugins

A monorepo containing custom Claude Code plugins by Dr. Mike Hopper.

## Plugins

### `swe/` — drmike-swe-plugin

Skills, agents, commands, and hooks for software engineering workflows.

#### Structure

- **agents/** — Custom agents with specialized system prompts and tool configurations
    - `test-ci-runner` — Runs the project's unit test suite in CI mode and reports results
    - `code-improvement-advisor` — Reviews code for readability, performance, and best practices
    - `git-committer` — Performs git commits using the git-commit skill and conventional commits
- **commands/** — Slash commands available in Claude Code sessions
    - `/aloha` — Greets the user and identifies the plugin as the source
- **hooks/** — Lifecycle event hooks
    - `SessionStart.sh` — Displays a friendly welcome message at the start of every session
- **skills/** — Reusable skill definitions loaded into Claude's context
    - `greeting` — Greets the user with a friendly message
    - `git-commit` — Executes git commits using the Conventional Commits specification
    - `explain-code` — Explains code with visual diagrams and analogies
    - `test-ci-runner` — Runs the unit test suite in CI mode and reports results

---

### `design/` — drmike-design-plugin

Skills for UX design workflows, including user research, wireframing, prototyping, and design best practices.

#### Structure

- **skills/** — Reusable skill definitions loaded into Claude's context
    - `greeting` — Greets the user with a friendly message (design plugin variant)

## Usage

Install each plugin directory (`swe/` or `design/`) individually via your Claude Code settings to activate the custom commands, hooks, and skills for that plugin in your sessions.
