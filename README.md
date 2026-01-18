# AI Coding Tools

A curated collection of Cursor IDE configurations for enhanced AI-assisted development. Includes rules, MCP servers, and skills for productive vibe coding.

## What's Included

| Component | Description |
|-----------|-------------|
| **Rules** | `.mdc` files with coding standards for React, Next.js, TypeScript |
| **MCP Servers** | Shadcn UI and Next.js devtools integrations |
| **Skills** | Vercel Labs best practices and design guidelines |

## Quick Start

```bash
# Clone the repo
git clone https://github.com/yourusername/ai-coding-tools.git

# Copy rules to your project
cp -r ai-coding-tools/cursor/rules/*.mdc your-project/.cursor/rules/

# Install skills
npx add-skill vercel-labs/agent-skills
```

For MCP servers, add the configurations from `cursor/mcp/mcp.json` to your Cursor MCP settings.

## Documentation

See [AGENTS.md](AGENTS.md) for detailed setup instructions and configuration options.

## Structure

```
cursor/
├── mcp/mcp.json       # MCP server configurations
├── rules/
│   ├── next.mdc       # Next.js conventions
│   └── react.mdc      # React/TypeScript standards
└── skills/README.md   # Skills installation guide
```

## License

[AGPL-3.0 license](LICENSE)
