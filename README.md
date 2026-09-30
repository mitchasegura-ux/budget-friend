# budget-friend

An AI agent skill that helps with **personal budgeting and self-employed finances**:

- **Personal**: track spending and income, sort spending into needs, obligations and wants, build a week-by-week cash flow budget (including for irregular pay), set SMART goals, grow an emergency fund, and pay down debt.
- **Self-employed / freelance / gig / sole proprietor**: keep business and personal money separate, size owner's draws, forecast cash runway, estimate quarterly taxes, check deductions (gear, mileage, home office), and pay subcontractors correctly.

It follows the open [Agent Skills](https://github.com/agentskills/agentskills) format (`SKILL.md` + on-demand chapter files), so it works in **Claude Code, OpenAI Codex, OpenCode, GitHub Copilot CLI, Amp** and other compatible tools.

> **Education, not advice.** Built from public CFPB, FTC, IRS, SBA and OpenStax material (see [sources.md](sources.md)). Not tax, legal or investment advice. Tax numbers are 2025/2026 US federal values; check them again every year.

## Install

**Any tool, one command** (uses the [`skills` CLI](https://skills.sh)), after this folder is published to a git repo:

```bash
npx skills add <your-github-user>/budget-friend
```

**From this folder** (macOS/Linux). Links the skill and the slash commands into every supported tool:

```bash
./install.sh
```

**Manual**: copy or link this folder to the skills directory your tool uses:

| Tool | Skill folder | Slash-command folder |
|---|---|---|
| Claude Code | `~/.claude/skills/budget-friend` | `~/.claude/commands/` |
| OpenAI Codex | `~/.agents/skills/budget-friend` | `~/.codex/prompts/` |
| OpenCode | `~/.agents/skills/budget-friend` (also reads `~/.claude/skills`) | `~/.config/opencode/commands/` |
| GitHub Copilot CLI / Amp | `~/.agents/skills/budget-friend` | — |
| Project-only (any tool) | `.claude/skills/` or `.agents/skills/` in the repo | — |

Restart your agent session after installing.

## Use

| Command | What it does |
|---|---|
| /bf-init | Initializes your finance folder, interviews you for missing info, and sets up your profile |
| /bf-budget | Builds a monthly budget plus a week-by-week cash flow budget |
| /bf-spending | Sorts pasted or exported transactions into categories and finds spending leaks |
| /bf-debt | Builds a debt log, calculates debt-to-income, and plans payoff order |
| /bf-runway | Self-employed: calculates burn rate, runway, Stability Fund gap, and a safe draw |
| /bf-quarterly | Self-employed: calculates the quarterly estimated-tax amount and the next due date |
| /bf-deductible | Self-employed: checks whether an expense can be written off |

In Codex, prompts run as `/prompts:bf-budget`. In tools without slash commands, just ask ("use budget-friend to build my budget").

**Privacy:** never paste account numbers, SSNs, or passwords. Redact them before pasting statements.

## What's inside

```
SKILL.md        core frameworks + chapter & topic index (loaded first)
chapters/       18 on-demand chapters (ch01–13 self-employed, ch14–18 personal)
glossary.md     key terms
patterns.md     step-by-step techniques
cheatsheet.md   decision rules, thresholds, tax calendar
sources.md      every source URL
commands/       the six /bf-* slash commands
install.sh      links everything into Claude Code, Codex, OpenCode, Copilot, Amp
```

## Uninstall

```bash
rm ~/.agents/skills/budget-friend ~/.claude/skills/budget-friend ~/.claude/commands/bf-*.md ~/.codex/prompts/bf-*.md ~/.config/opencode/commands/bf-*.md
```

## License & attribution

Content is synthesized from US government works (public domain) and OpenStax *Entrepreneurship* (© Rice University, CC BY-NC-SA 4.0), so derived material is shared under **CC BY-NC-SA 4.0**. Generated with [book-to-skill](https://github.com/virgilio94/book-to-skill).
