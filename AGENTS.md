# AGENTS.md

This repository contains configuration files and resources for enhancing AI coding agents in Cursor IDE. The goal is to provide a curated collection of rules, MCP servers, and skills that improve the agentic coding experience.

## Repository Structure

```
cursor/
├── mcp/          # Model Context Protocol server configurations
├── rules/        # Cursor rule files (.mdc)
└── skills/       # Agent skills documentation and setup
```

## Components

### Rules (`cursor/rules/`)

Rule files (`.mdc`) provide persistent instructions to the AI agent. These are applied based on context or can be set to always apply.

| File | Purpose | Always Applied |
|------|---------|----------------|
| `react.mdc` | React/TypeScript best practices, code style, Shadcn UI patterns | ✅ |
| `next.mdc` | Next.js App Router conventions, testing, and MCP integration | ✅ |

**Installation:** Copy `.mdc` files to your project's `.cursor/rules/` directory.

### MCP Servers (`cursor/mcp/`)

MCP (Model Context Protocol) servers extend agent capabilities with external tools and context.

| Server | Description |
|--------|-------------|
| `shadcn` | Provides Shadcn UI component generation and management |
| `next-devtools` | Next.js development tools and documentation context |

**Installation:** Merge the `mcp.json` configuration into your Cursor MCP settings.

### Skills (`cursor/skills/`)

Skills are reusable knowledge bases that agents can reference. See the [skills README](cursor/skills/README.md) for installation instructions.

**Recommended Skills:**
- `vercel-react-best-practices` - React patterns from Vercel Labs
- `web-design-guidelines` - Design system guidance

## Usage

### Quick Setup

1. **Clone this repository**
   ```bash
   git clone https://github.com/yourusername/ai-coding-tools.git
   ```

2. **Copy rules to your project**
   ```bash
   cp -r ai-coding-tools/cursor/rules/*.mdc your-project/.cursor/rules/
   ```

3. **Add MCP servers to Cursor**
   - Open Cursor Settings → MCP
   - Add the server configurations from `cursor/mcp/mcp.json`

4. **Install skills (optional)**
   ```bash
   npx add-skill vercel-labs/agent-skills
   ```

## Agent Behavior

With these configurations, the AI agent will:

- Follow TypeScript and functional programming best practices
- Use Shadcn UI and Tailwind CSS for styling
- Run `npm run lint` after code changes
- Consult skills knowledge for React/Next.js patterns
- Initialize Next.js devtools context at session start

## Contributing

To add new configurations:

1. **Rules:** Add `.mdc` files to `cursor/rules/` with appropriate frontmatter
2. **MCP Servers:** Update `cursor/mcp/mcp.json` with new server definitions
3. **Skills:** Document installation in `cursor/skills/README.md`

## License

AGPL-3.0 license - See [LICENSE](LICENSE) for details.
