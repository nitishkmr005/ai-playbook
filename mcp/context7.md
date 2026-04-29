# Context7 MCP

**Provider:** Upstash (via claude.ai plugins)  
**Status:** install from claude.com/plugins/context7  
**Type:** Documentation Lookup / Up-to-date Library Docs

## Overview

Context7 solves the problem of LLMs hallucinating outdated APIs. It pulls current, version-specific documentation and code examples directly from source repositories into the prompt — so Claude uses real, live docs instead of stale training data.

## Available Tools

| Tool | Description |
|------|-------------|
| `resolve-library-id` | Match a library name to its Context7-compatible identifier (e.g. `"react"` → `/facebook/react`) |
| `query-docs` | Fetch up-to-date documentation and code examples for a specific library and version |

## How to Use

Add **`use context7`** anywhere in your prompt — Claude will automatically resolve the library and pull current docs before responding.

```
Create a Next.js middleware that checks for a valid JWT in cookies. use context7

Set up a Prisma schema with PostgreSQL and run migrations. use context7

Configure Cloudflare Workers KV storage with TypeScript. use context7

Show me how to use useQuery in TanStack Query v5. use context7
```

You can also target a specific library explicitly:

```
use library /supabase/supabase for the auth API
use library /vercel/next.js@14 for App Router docs
```

## Installation

1. Go to [claude.com/plugins/context7](https://claude.com/plugins/context7)
2. Click **Install** — no authentication required
3. Once connected, add `use context7` to any prompt

## Notes

- No API key or authentication needed — Context7 is free to use
- Works best for popular open-source libraries with active documentation
- Version targeting prevents mixing docs from different major versions
- Pairs well with the `mcp-builder` skill when building new MCP servers that need current SDK docs
