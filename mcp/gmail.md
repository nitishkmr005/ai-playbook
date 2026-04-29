# Gmail MCP

**Provider:** claude.ai  
**Status:** △ needs authentication  
**Type:** Email

## Overview

Gmail MCP allows Claude to read, search, compose, and send emails through your Gmail account. Requires OAuth authentication before first use.

## Authentication

```
Step 1: Run authenticate tool → opens Google OAuth consent screen
Step 2: Complete sign-in in browser
Step 3: Run complete_authentication tool → confirms connection
```

## Available Tools (post-auth)

| Tool | Description |
|------|-------------|
| `authenticate` | Initiate Google OAuth flow for Gmail access |
| `complete_authentication` | Finalize the OAuth handshake |

Once authenticated, Claude gains access to Gmail operations including:
- Reading and searching messages
- Composing and sending emails
- Managing labels and threads
- Accessing drafts

## Usage Examples

```
Summarize my unread emails from the last 24 hours

Search for emails from team@company.com about the Q1 report

Draft a reply to the last email from John and send it

Label all emails about "invoices" as Finance
```

## Notes

- Requires a Google account with Gmail
- OAuth scopes are requested by claude.ai — review before approving
- Re-authentication may be needed if the token expires
