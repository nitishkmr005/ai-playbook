# Google Drive MCP

**Provider:** claude.ai  
**Status:** △ needs authentication  
**Type:** File Storage / Documents

## Overview

Google Drive MCP enables Claude to browse, read, create, and manage files and folders in your Google Drive, including Google Docs, Sheets, and Slides. Requires OAuth authentication before first use.

## Authentication

```
Step 1: Run authenticate tool → opens Google OAuth consent screen
Step 2: Complete sign-in in browser
Step 3: Run complete_authentication tool → confirms connection
```

## Available Tools (post-auth)

| Tool | Description |
|------|-------------|
| `authenticate` | Initiate Google OAuth flow for Drive access |
| `complete_authentication` | Finalize the OAuth handshake |

Once authenticated, Claude gains access to Drive operations including:
- Listing and searching files/folders
- Reading file contents (Docs, Sheets, plain text, PDFs)
- Creating and editing Google Docs or Sheets
- Moving, copying, renaming, and deleting files
- Managing sharing permissions

## Usage Examples

```
Find all spreadsheets shared with me in the last week

Summarize the document "Q2 Product Roadmap" in my Drive

Create a new Google Doc with a meeting agenda template

Move all files in my Downloads folder to the Archive folder
```

## Notes

- Requires a Google account with Drive access
- Large binary files (images, videos) may not be readable as text
- Editing Google Docs/Sheets happens via Drive API — formatting may differ from native editor
- OAuth token may expire; re-run authenticate if access is denied
