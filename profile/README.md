# ai-awesome

Opinionated tools and skills for [Claude Code](https://docs.anthropic.com/en/docs/claude-code) -- turning it into a disciplined, autonomous engineering assistant.

## Repositories

| Repository | Description |
|---|---|
| [claude-global-settings](https://github.com/ai-awesome/claude-global-settings) | Global configuration that makes Claude Code act as a planner/coordinator with thinking discipline, TTS hooks, and a dedicated worker agent for implementation tasks. |
| [skill-submit-pr](https://github.com/ai-awesome/skill-submit-pr) | `/submit-pr` skill -- automates branching, building, testing, committing, pushing, PR creation, and CI monitoring in a single command. |
| [skill-publish](https://github.com/ai-awesome/skill-publish) | `/publish` skill -- automates version bumping, release tagging, and pushing to trigger CI-based publishing. |
| [skill-audit-project](https://github.com/ai-awesome/skill-audit-project) | `/audit-project` skill -- performs a structured six-phase project audit evaluating goal alignment, dependency health, code quality, and produces a prioritized improvement roadmap. |
| [skill-create-slides](https://github.com/ai-awesome/skill-create-slides) | `/create-slides` skill -- creates Reveal.js + Markdown presentations using the slides.johnsonlee.io framework, with four built-in presentation styles and GitHub Pages deployment. |

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
# Clone and install skills
git clone https://github.com/ai-awesome/skill-submit-pr.git
mkdir -p ~/.claude/skills/submit-pr
ln -sf "$(pwd)/skill-submit-pr/SKILL.md" ~/.claude/skills/submit-pr/SKILL.md

git clone https://github.com/ai-awesome/skill-publish.git
mkdir -p ~/.claude/skills/publish
ln -sf "$(pwd)/skill-publish/SKILL.md" ~/.claude/skills/publish/SKILL.md

git clone https://github.com/ai-awesome/skill-audit-project.git
mkdir -p ~/.claude/skills/audit-project
ln -sf "$(pwd)/skill-audit-project/SKILL.md" ~/.claude/skills/audit-project/SKILL.md

git clone https://github.com/ai-awesome/skill-create-slides.git
mkdir -p ~/.claude/skills/create-slides
ln -sf "$(pwd)/skill-create-slides/SKILL.md" ~/.claude/skills/create-slides/SKILL.md
```

Or add them as submodules in your dotfiles:

```sh
git submodule add https://github.com/ai-awesome/skill-submit-pr.git ~/.claude/skills/submit-pr
git submodule add https://github.com/ai-awesome/skill-publish.git ~/.claude/skills/publish
git submodule add https://github.com/ai-awesome/skill-audit-project.git ~/.claude/skills/audit-project
git submodule add https://github.com/ai-awesome/skill-create-slides.git ~/.claude/skills/create-slides
```

## Contributing

1. Fork the relevant repository and create a feature branch.
2. Make your changes and ensure they are consistent with the existing style.
3. Submit a pull request with a clear description of what you changed and why.
