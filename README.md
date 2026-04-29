# AI Playbook

A personal collection of prompts, skills, agents, commands, and MCP configurations for working effectively with AI tools — primarily Claude Code and the Anthropic API.

---

## What's Inside

```
ai-playbook/
├── prompts/          # Reusable prompt library organized by use case
├── skills/           # Claude Code skills (plug-in capabilities)
├── agents/           # Custom Claude agent definitions
├── commands/         # Slash commands for Claude Code
├── mcp/              # MCP server setup guides
├── claude-md/        # CLAUDE.md templates for projects
└── plugins/          # Claude Code plugin configs
```

---

## Prompts

Organized prompt library covering a wide range of use cases.

| Folder | Description |
|--------|-------------|
| `prompts/image-generation/` | 3D illustrations, artistic styles, infographics, logos & branding |
| `prompts/ui-design/` | SaaS dashboards, dark-themed homepages, product UI mockups |
| `prompts/meta-prompts/` | Prompt evaluator, adaptive image creator, second-brain / memory system |
| `prompts/reasoning/` | Tree-of-thought, multi-expert debate frameworks |
| `prompts/content-creation/` | Podcast-style script generator, article writing |
| `prompts/references/` | External system prompt repos, tools, and resources |

---

## Skills

Claude Code skills that add domain-specific capabilities. Drop these into `~/.claude/skills/` to make them available globally.

| Skill | Description |
|-------|-------------|
| `claude-api` | Build and optimize Claude API / Anthropic SDK apps with prompt caching |
| `chroma` | Chroma vector database for embeddings and RAG |
| `qdrant-vector-search` | Qdrant high-performance vector search |
| `faiss` | FAISS similarity search and dense vector clustering |
| `llamaindex` | LlamaIndex RAG framework with 300+ data connectors |
| `peft-fine-tuning` | LoRA, QLoRA, and 25+ PEFT methods for LLM fine-tuning |
| `deepspeed` | DeepSpeed ZeRO optimization and distributed training |
| `pytorch-fsdp` | Fully Sharded Data Parallel training with PyTorch |
| `pytorch-lightning` | High-level PyTorch training with Trainer and callbacks |
| `huggingface-accelerate` | Minimal distributed training API for PyTorch |
| `training-llms-megatron` | Megatron-Core for large-scale LLM training (2B–462B params) |
| `moe-training` | Mixture of Experts model training with DeepSpeed / HuggingFace |
| `knowledge-distillation` | Teacher-to-student model compression |
| `model-pruning` | Wanda and SparseGPT pruning for LLM inference |
| `model-merging` | Merge fine-tuned models with mergekit |
| `speculative-decoding` | Speculative decoding, Medusa, and lookahead for faster inference |
| `llama-cpp` | llama.cpp inference on CPU, Apple Silicon, and consumer GPUs |
| `gguf-quantization` | GGUF format and llama.cpp quantization |
| `long-context` | RoPE, YaRN, ALiBi context window extension |
| `nanogpt` | Educational GPT-2 reproduction (~300 lines) |
| `nemo-curator` | GPU-accelerated data curation for LLM pre-training |
| `sentence-transformers` | Sentence and text embeddings with 5000+ pre-trained models |
| `scientific-schematics` | Publication-quality scientific diagrams |
| `frontend-design` | Production-grade frontend UI design |
| `vercel-react-best-practices` | React and Next.js performance from Vercel Engineering |
| `web-design-guidelines` | UI code review for web interface guidelines |
| `claude-md-improver` | Audit and improve CLAUDE.md files |
| `skill-creator` | Create and refine new Claude Code skills |

---

## Agents

Custom Claude agent definitions for specialized tasks.

| Agent | Description |
|-------|-------------|
| `code-simplifier` | Simplifies and refines code for clarity and maintainability |

---

## Commands

Slash commands for Claude Code workflows.

| Command | Description |
|---------|-------------|
| `commit-commands` | Commit, push, and open PRs — with language-specific templates |
| `code-review` | Structured code review slash command |

---

## MCP Server Configurations

Setup guides for Model Context Protocol (MCP) servers — connect Claude to external tools and services.

| Integration | File |
|-------------|------|
| Notion | `mcp/notion.md` |
| Gmail | `mcp/gmail.md` |
| Google Calendar | `mcp/google-calendar.md` |
| Google Drive | `mcp/google-drive.md` |
| Mermaid Chart | `mcp/mermaid-chart.md` |
| Excalidraw | `mcp/excalidraw.md` |
| Vercel | `mcp/vercel.md` |
| Hugging Face | `mcp/hugging-face.md` |
| Context7 | `mcp/context7.md` |
| Computer Use | `mcp/computer-use.md` |

---

## Claude.md Templates

`claude-md/` contains CLAUDE.md templates — project-level instructions that guide Claude's behavior within a codebase.

---

## Plugins

| Plugin | Description |
|--------|-------------|
| `hookify` | Claude Code hook configurations |
| `ralph-loop` | Loop-based automation plugin |

---

## Getting Started

### Use a Skill
Copy the skill folder into your Claude skills directory:
```bash
cp -r skills/claude-api ~/.claude/skills/
```

### Use a Command
Copy commands into your Claude commands directory:
```bash
cp -r commands/commit-commands ~/.claude/commands/
```

### Use a CLAUDE.md Template
Copy the template into your project root and customize:
```bash
cp claude-md/CLAUDE.md ./CLAUDE.md
```

---

## Related Resources

- [Claude Code Docs](https://docs.anthropic.com/claude-code)
- [MCP Server Directory](https://github.com/modelcontextprotocol/servers)
- [Awesome MCP Servers](https://github.com/punkpeye/awesome-mcp-servers)
