# Computer Use MCP

**Provider:** Built-in (always available)  
**Status:** ◯ disabled  
**Type:** Desktop Automation / GUI Control

## Overview

Computer Use is a built-in MCP that gives Claude direct control over your computer — mouse, keyboard, screen capture, and application interaction. It is disabled by default due to its broad system access and must be explicitly enabled.

## How to Enable

In Claude Code settings or `settings.json`:
```json
{
  "mcpServers": {
    "computer-use": {
      "enabled": true
    }
  }
}
```

Or toggle via `/mcp` → Computer Use → Enable.

## Capabilities (when enabled)

| Capability | Description |
|------------|-------------|
| Screen capture | Take screenshots to observe current UI state |
| Mouse control | Move cursor, click, double-click, right-click, drag |
| Keyboard input | Type text, send key combinations (Ctrl+C, Cmd+Tab, etc.) |
| Application launch | Open apps, files, and URLs |
| Scrolling | Scroll windows and web pages |
| Clipboard | Read from and write to the clipboard |

## Usage Examples

```
Open my terminal and run `git status` in the ~/projects/my-app folder

Take a screenshot and tell me what application is currently in focus

Fill in the login form on the page with my credentials and click Submit

Drag the file from my Downloads folder to the Documents folder

Open System Preferences and navigate to Display settings
```

## Safety Notes

- **Enabled with caution**: Computer Use can perform irreversible actions (delete files, send messages, make purchases)
- Claude will describe each action before executing and ask for confirmation on destructive operations
- Recommended to use in sandboxed or VM environments for automated workflows
- Disable when not in use to prevent accidental system interactions
- Works best on macOS and Linux; Windows support may vary
