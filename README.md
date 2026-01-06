# Agent 37 Skills Collection

A collection of Claude Code plugins for enhanced AI assistance.

## Available Plugins

### yc-advisor (Skill)

Provides access to Y Combinator's complete library of 434 curated startup resources including essays by Paul Graham, founder interviews, and startup school lectures.

**Automatically used when:**
- Asking questions about startups, founding decisions, co-founders
- Seeking advice on fundraising, product development, growth, hiring
- Looking for entrepreneurial guidance backed by YC's expertise

### local-review (Command)

Code review for uncommitted local changes. Reviews staged and unstaged changes for bugs, security vulnerabilities, CLAUDE.md compliance, and TypeScript issues.

**Invoke with:** `/local-review:local-review`

**Features:**
- Scans for bugs, logic errors, and edge cases
- Checks for security vulnerabilities (OWASP top 10)
- Validates compliance with your project's CLAUDE.md guidelines
- Filters out false positives with confidence scoring
- Groups issues by severity (Critical / Warning)

## Installation

1. Add the marketplace:
   ```bash
   /plugin marketplace add Agent-3-7/agent37-skills-collection
   ```

2. Install a plugin:
   ```bash
   # Install yc-advisor skill
   /plugin install yc-advisor@agent37-skills

   # Install local-review command
   /plugin install local-review@agent37-skills
   ```

## Skills vs Commands

- **Skills** are automatically triggered by Claude based on context (e.g., yc-advisor activates when you ask about startups)
- **Commands** are explicitly invoked with `/plugin-name:command-name` (e.g., `/local-review:local-review`)

## License

MIT License - see [LICENSE](LICENSE) for details.
