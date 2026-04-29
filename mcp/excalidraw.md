# Excalidraw MCP

**Provider:** claude.ai  
**Status:** ✔ connected  
**Type:** Diagramming / Whiteboard

## Overview

Excalidraw MCP lets Claude create, edit, and export hand-drawn-style diagrams and whiteboard sketches directly inside Claude Code. No authentication required — works out of the box.

## Available Tools

| Tool | Description |
|------|-------------|
| `create_view` | Create a new Excalidraw canvas/view |
| `export_to_excalidraw` | Export current diagram to Excalidraw format (.excalidraw JSON) |
| `read_checkpoint` | Read a previously saved diagram checkpoint |
| `read_me` | Read the MCP's own documentation/capabilities |
| `save_checkpoint` | Save the current diagram state as a checkpoint |

## Usage Examples

```
Draw a system architecture diagram with a frontend, API gateway, and database
→ Uses create_view + export_to_excalidraw

Save my diagram progress so I can resume it later
→ Uses save_checkpoint

Load my saved architecture diagram
→ Uses read_checkpoint
```

## Notes

- Produces `.excalidraw` JSON files compatible with excalidraw.com
- Diagrams have a hand-drawn aesthetic by default
- Checkpoints allow iterative refinement across sessions
