Opinionated tools and skills for AI agents -- turning them into disciplined, autonomous engineering assistants.

## Claude Settings

| Repository | Description |
|---|---|
| [.claude](https://github.com/ai-awesome/.claude) | Global configuration that makes Claude Code act as a planner/coordinator with thinking discipline, TTS hooks, and a dedicated worker agent for implementation tasks. |

## SKILLs

| Repository | Skill | Description |
|---|---|---|
| [skill-submit-pr](https://github.com/ai-awesome/skill-submit-pr) | `/submit-pr` | Automates branching, building, testing, committing, pushing, PR creation, and CI monitoring in a single command. |
| [skill-publish](https://github.com/ai-awesome/skill-publish) | `/publish` | Automates version bumping, release tagging, and pushing to trigger CI-based publishing. |
| [skill-audit-project](https://github.com/ai-awesome/skill-audit-project) | `/audit-project` | Performs a structured six-phase project audit evaluating goal alignment, dependency health, code quality, and produces a prioritized improvement roadmap. |
| [skill-create-slides](https://github.com/ai-awesome/skill-create-slides) | `/create-slides` | Creates Reveal.js + Markdown presentations using the slides.johnsonlee.io framework, with four built-in presentation styles and GitHub Pages deployment. |
| [skill-always-hungry](https://github.com/ai-awesome/skill-always-hungry) | `/always-hungry` | Scouts the open-source community for improvements to any project, evaluates candidates with automated auditing, and applies what works. |

## Getting Started

### Quick install

```sh
bash <(curl -fsSL https://raw.githubusercontent.com/ai-awesome/.claude/main/scripts/install.sh)
```

The install script handles both fresh installs and existing `~/.claude` directories. If conflicting files are detected, it will prompt you to back them up before proceeding.

### Manual install

Clone directly if you don't have `~/.claude` yet:

```sh
git clone git@github.com:ai-awesome/.claude.git ~/.claude
```

If `~/.claude` already exists, run the install script locally:

```sh
curl -fsSL https://raw.githubusercontent.com/ai-awesome/.claude/main/scripts/install.sh | bash
```

## Contributing

1. Fork the relevant repository and create a feature branch.
2. Make your changes and ensure they are consistent with the existing style.
3. Submit a pull request with a clear description of what you changed and why.
