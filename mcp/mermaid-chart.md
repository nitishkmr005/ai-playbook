# Mermaid Chart MCP

**Provider:** claude.ai  
**Status:** ✔ connected  
**Type:** Diagramming / Code-based Charts

## Overview

Mermaid Chart MCP lets Claude generate, validate, and render Mermaid diagrams — flowcharts, sequence diagrams, ER diagrams, Gantt charts, and more. No authentication required.

## Available Tools

| Tool | Description |
|------|-------------|
| `list_tools` | List all available MCP tools and their capabilities |
| `get_diagram_title` | Extract the title from an existing Mermaid diagram |
| `get_diagram_summary` | Generate a human-readable summary of what a diagram shows |
| `get_mermaid_syntax_document` | Retrieve Mermaid syntax reference for a specific diagram type |
| `search_mermaid_icons` | Search the icon library for use in diagrams |
| `validate_and_render_mermaid_diagram` | Validate Mermaid syntax and render to image |

## Supported Diagram Types

- Flowchart (`graph TD / LR`)
- Sequence diagram
- Class diagram
- State diagram
- Entity-Relationship (ER)
- Gantt chart
- Pie chart
- Quadrant chart
- Git graph
- Mindmap
- Timeline

## Usage Examples

```
Draw a sequence diagram of a user login flow with JWT tokens

Validate this Mermaid code and render it as an image:
  graph TD; A-->B; B-->C

Generate an ER diagram for a blog database with users, posts, comments

Show me the syntax for a Gantt chart

Search for cloud icons to use in my architecture diagram
```

## Notes

- Use `get_mermaid_syntax_document` before writing complex diagrams to avoid syntax errors
- `validate_and_render_mermaid_diagram` catches errors before they reach the UI
- Rendered output is typically a PNG/SVG image link
