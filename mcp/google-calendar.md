# Google Calendar MCP

**Provider:** claude.ai  
**Status:** △ needs authentication  
**Type:** Calendar / Scheduling

## Overview

Google Calendar MCP lets Claude read, create, update, and delete calendar events across your Google Calendars. Requires OAuth authentication before first use.

## Authentication

```
Step 1: Run authenticate tool → opens Google OAuth consent screen
Step 2: Complete sign-in in browser
Step 3: Run complete_authentication tool → confirms connection
```

## Available Tools (post-auth)

| Tool | Description |
|------|-------------|
| `authenticate` | Initiate Google OAuth flow for Calendar access |
| `complete_authentication` | Finalize the OAuth handshake |

Once authenticated, Claude gains access to Calendar operations including:
- Listing and searching events
- Creating new events with attendees, location, description
- Updating or cancelling existing events
- Checking free/busy slots across calendars

## Usage Examples

```
What meetings do I have tomorrow?

Schedule a 1-hour team standup every Monday at 9am starting next week

Find a free 30-minute slot this week for a call with Alice

Cancel my 3pm meeting on Friday and send cancellation notices
```

## Notes

- Requires a Google account with Calendar enabled
- Can access multiple calendars (primary, shared, work, personal)
- OAuth token may expire; re-run authenticate if access is denied
