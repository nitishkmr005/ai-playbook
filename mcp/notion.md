# Notion MCP

**Provider:** claude.ai  
**Status:** △ needs authentication  
**Type:** Notes / Knowledge Base / Project Management

## Overview

Notion MCP enables Claude to read, create, and update pages, databases, and blocks in your Notion workspace. Requires OAuth authentication before first use.

## Authentication

```
Step 1: Run authenticate tool → opens Notion OAuth consent screen
Step 2: Select the workspace and pages to grant access to
Step 3: Run complete_authentication tool → confirms connection
```

## Available Tools (post-auth)

| Tool | Description |
|------|-------------|
| `authenticate` | Initiate Notion OAuth flow |
| `complete_authentication` | Finalize the OAuth handshake |

Once authenticated, Claude gains access to Notion operations including:
- Reading and searching pages and databases
- Creating new pages with rich content (headings, bullets, code, tables)
- Updating existing page content and properties
- Querying database views with filters and sorts
- Managing database entries (create, update, delete rows)

## Usage Examples

```
Summarize all pages tagged "In Progress" in my Projects database

Create a new meeting notes page in my Work space for today's standup

Add a new row to my Book Tracker database: "Atomic Habits" by James Clear, Status: Reading

Search my Notion for everything related to "API design"
```

## Notes

- Notion OAuth requires explicitly granting access to specific pages/databases — Claude only sees what you share
- Rich text formatting (callouts, toggles, synced blocks) is supported
- Large pages with many nested blocks may be read in chunks
- Re-authenticate if your Notion token expires
