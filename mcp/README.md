# MCP Servers

Model Context Protocol (MCP) servers extend Claude Code with external integrations.

## Status

| MCP | Provider | Status | File |
|-----|----------|--------|------|
| Excalidraw | claude.ai | ✔ connected | [excalidraw.md](excalidraw.md) |
| Mermaid Chart | claude.ai | ✔ connected | [mermaid-chart.md](mermaid-chart.md) |
| Context7 | Upstash | install needed | [context7.md](context7.md) |
| Gmail | claude.ai | △ needs auth | [gmail.md](gmail.md) |
| Google Calendar | claude.ai | △ needs auth | [google-calendar.md](google-calendar.md) |
| Google Drive | claude.ai | △ needs auth | [google-drive.md](google-drive.md) |
| Hugging Face | claude.ai | △ needs auth | [hugging-face.md](hugging-face.md) |
| Notion | claude.ai | △ needs auth | [notion.md](notion.md) |
| Vercel | claude.ai | △ needs auth | [vercel.md](vercel.md) |
| Computer Use | Built-in | ◯ disabled | [computer-use.md](computer-use.md) |

## Authentication

MCPs marked **△ needs auth** require a one-time OAuth or token setup:
1. In Claude Code, run `/mcp`
2. Select the MCP and follow the authentication steps
3. Status changes to ✔ connected

## Adding More MCPs

Install new MCPs from `claude.com/plugins` or configure custom servers in `~/.claude/settings.json` under `mcpServers`.
