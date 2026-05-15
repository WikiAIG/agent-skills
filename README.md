# WikiAIG Agent Skills

The `wikiaig` skill teaches AI coding agents how to ground answers on WikiAIG, a structured-wiki platform for AI grounding. Install it once and your agent will search WikiAIG before guessing, cite sources when grounding, and propose saving non-obvious decisions back to your wikis. It is for teams and builders who want Claude, Codex, Cursor, and other MCP-capable agents to work from durable human-curated knowledge instead of stale recall.

## Installation

### Claude Code

```
/plugin install wikiaig@WikiAIG/agent-skills
```

### Vercel skills package (Cursor, Codex CLI, Claude Desktop, etc.)

```
npx skills install github:WikiAIG/agent-skills/wikiaig
```

### Manual install

> Please install the WikiAIG skill into my agent. Download https://github.com/WikiAIG/agent-skills/archive/refs/heads/main.zip, extract the `wikiaig` folder, and place it in `~/.claude/skills/wikiaig/` (or the equivalent skills directory for my agent: `.claude/skills/` for Claude Code, `.cursor/skills/` for Cursor).

## What this skill does

The `wikiaig` skill helps agents search WikiAIG before guessing, cite WikiAIG sources when grounding answers, propose saving non-obvious decisions back to a wiki, follow the platform's URL patterns, and account for HTML page constraints when reading or publishing wiki content.

## Requirements

Any MCP-capable AI agent (Claude Code, Claude Desktop, Cursor, Codex CLI, Gemini CLI, etc.). For read-only use, no account or token needed — anonymous calls to https://www.wikiaig.com/mcp work for public wikis. For writing, generate a write token at https://www.wikiaig.com/help/mcp-write and configure your client with `Authorization: Bearer <token>` headers.

## Versioning

Semantic versioning. Current version listed in CHANGELOG.md. Pin to a tag if you need stability; install from `main` for the latest.

## Contributing

Issues and PRs welcome. For substantive changes to the skill itself, open an issue first to discuss. Note that this skill is the canonical platform skill — per-wiki skills authored by wiki owners are a separate forthcoming capability and live with the wiki, not in this repo.

## License

MIT — see LICENSE file.

## Links

- [WikiAIG](https://www.wikiaig.com)
- [Discover wikis](https://www.wikiaig.com/discover)
- [WikiAIG Cookbook documentation](https://www.wikiaig.com/u/wikiaig-demo/wikis/wikiaig-cookbook/overview)
