# ai-awesome

Opinionated tools and skills for [Claude Code](https://docs.anthropic.com/en/docs/claude-code) -- turning it into a disciplined, autonomous engineering assistant.

## Repositories

| Repository | Description |
|---|---|
| [claude-global-settings](https://github.com/ai-awesome/claude-global-settings) | Global configuration that makes Claude Code act as a planner/coordinator with thinking discipline, TTS hooks, and a dedicated worker agent for implementation tasks. |
| [skill-submit-pr](https://github.com/ai-awesome/skill-submit-pr) | `/submit-pr` skill -- automates branching, building, testing, committing, pushing, PR creation, and CI monitoring in a single command. |
| [skill-publish](https://github.com/ai-awesome/skill-publish) | `/publish` skill -- automates version bumping, release tagging, and pushing to trigger CI-based publishing. |
| [skill-project-audit](https://github.com/ai-awesome/skill-project-audit) | `/project-audit` skill -- performs a structured six-phase project audit evaluating goal alignment, dependency health, code quality, and produces a prioritized improvement roadmap. |

## Getting Started

Install the global settings to configure Claude Code as a planner/coordinator:

```sh
git clone https://github.com/ai-awesome/claude-global-settings.git
ln -sf "$(pwd)/claude-global-settings/CLAUDE.md" ~/.claude/CLAUDE.md
ln -sf "$(pwd)/claude-global-settings/settings.json" ~/.claude/settings.json
ln -sf "$(pwd)/claude-global-settings/agents" ~/.claude/agents
```

Install skills individually as needed:

```sh
claude mcp add-skill https://github.com/ai-awesome/skill-submit-pr
claude mcp add-skill https://github.com/ai-awesome/skill-publish
claude mcp add-skill https://github.com/ai-awesome/skill-project-audit
```

## Contributing

1. Fork the relevant repository and create a feature branch.
2. Make your changes and ensure they are consistent with the existing style.
3. Submit a pull request with a clear description of what you changed and why.
