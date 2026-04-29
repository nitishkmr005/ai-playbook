# AI Playbook

A personal collection of prompts, skills, agents, commands, and MCP configurations for working effectively with AI tools — primarily Claude Code and the Anthropic API.

---

## Quick Reference — What to Use When

> **For agents:** Match the user's query to a row below, then read the linked file.

| If the user asks about... | Go to |
|---------------------------|-------|
| Writing an article, thread, email, or repurposing content | `prompts/expert-40/01-writing-and-content.md` |
| SWOT, decision matrix, OKRs, pricing, competitive teardown | `prompts/expert-40/02-analysis-and-strategy.md` |
| Architecture, code review, debugging, API design, DB schema | `prompts/expert-40/03-technical-and-development.md` |
| Weekly planning, learning plans, negotiation, habits | `prompts/expert-40/04-productivity-and-personal.md` |
| Analyzing data, surveys, or synthesizing research | `prompts/expert-40/05-data-and-research.md` |
| Difficult conversations, feedback, presentations, pitches | `prompts/expert-40/06-communication.md` |
| Extracting insights beyond summarizing | `prompts/analysis-and-strategy/information-processing.md` |
| Resume writing, ATS optimization, job search | `prompts/career/resume-and-job-search.md` |
| Executive workflows — meeting prep, time audits, project status | `prompts/productivity-and-personal/executive-workflows.md` |
| Root cause analysis, critical thinking, assumption checking | `prompts/reasoning/critical-thinking.md` |
| 80/20 rule, fear-setting, minimum effective dose | `prompts/reasoning/productivity-frameworks.md` |
| Multi-expert debate, tree-of-thought reasoning | `prompts/reasoning/tree-of-thought.md` |
| Generating images — 3D, illustrations, characters | `prompts/image-generation/3d-illustrations.md` |
| Infographic or process flow image | `prompts/image-generation/infographics.md` |
| Artistic style (charcoal, blueprint, Pixar, clay) | `prompts/image-generation/artistic-styles.md` |
| Logo or brand identity image | `prompts/image-generation/logos-branding.md` |
| SaaS homepage or dashboard UI mockup | `prompts/ui-design/saas-dashboards.md` |
| Evaluating or scoring a prompt | `prompts/meta-prompts/prompt-evaluator.md` |
| Building a prompt from scratch | `prompts/meta-prompts/prompt-architect.md` |
| Prompt tricks that improve output quality | `prompts/meta-prompts/prompt-tricks.md` |
| Conversational image prompt builder | `prompts/meta-prompts/adaptive-image-creator.md` |
| Persistent memory / second brain for AI | `prompts/meta-prompts/memory-second-brain.md` |
| Converting content to a podcast script | `prompts/content-creation/podcast-script.md` |
| Simplifying or refactoring code automatically | `agents/code-simplifier/agents/code-simplifier.md` |
| Running a structured code review | `commands/code-review/commands/code-review.md` |
| Committing, pushing, or opening a PR | `commands/commit-commands/` |
| Setting up automated hooks / behavior guards | `plugins/hookify/README.md` |
| Running iterative agent loops | `plugins/ralph-loop/README.md` |
| Connecting Claude to Notion, Gmail, Calendar, Drive | `mcp/` — see MCP section below |
| Drawing diagrams (Excalidraw, Mermaid) | `mcp/excalidraw.md` or `mcp/mermaid-chart.md` |
| Deploying to Vercel | `mcp/vercel.md` |
| Looking up library/framework documentation | `mcp/context7.md` |
| Building or calling the Claude/Anthropic API | `skills/claude-api/SKILL.md` |
| RAG, vector search, embeddings | `skills/llamaindex/SKILL.md`, `skills/chroma/SKILL.md`, `skills/qdrant-vector-search/SKILL.md` |
| Fine-tuning a model (LoRA, QLoRA) | `skills/peft-fine-tuning/SKILL.md` |
| Distributed / large-scale model training | `skills/deepspeed/SKILL.md`, `skills/pytorch-fsdp/SKILL.md`, `skills/training-llms-megatron/SKILL.md` |
| Running LLMs locally (CPU/GPU) | `skills/llama-cpp/SKILL.md`, `skills/gguf-quantization/SKILL.md` |
| React / Next.js performance | `skills/vercel-react-best-practices/SKILL.md` |
| Building or improving frontend UI | `skills/frontend-design/SKILL.md` |
| Working with PDF, PPTX, or XLSX files | `skills/pdf/SKILL.md`, `skills/pptx/SKILL.md`, `skills/xlsx/SKILL.md` |
| Setting up a CLAUDE.md for a project | `claude-md/CLAUDE.md` |

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
| `prompts/expert-40/` | 40 production-ready prompts tested on Claude, ChatGPT, and Gemini — writing, strategy, technical, productivity, data, communication |
| `prompts/analysis-and-strategy/` | Information processing: 8 prompts beyond summarizing (insights, action plans, leverage points) |
| `prompts/career/` | Resume rebuild, ATS optimization, job-specific tailoring, recruiter mind-reader |
| `prompts/productivity-and-personal/` | Executive workflows — meeting prep, time audits, project status, deadline checks |
| `prompts/reasoning/` | Critical thinking (Socratic method, assumption detector, devil's advocate), productivity frameworks (80/20, fear-setting, MED), tree-of-thought |
| `prompts/meta-prompts/` | Prompt architect system prompt, ultrathink coding prompt, prompt evaluator (24 metrics), prompt tricks, adaptive image creator, memory/second-brain |
| `prompts/image-generation/` | 3D illustrations, artistic styles (charcoal, blueprint, Pixar), infographics, logos & branding |
| `prompts/ui-design/` | SaaS dashboards, dark-themed homepages, fintech UI mockups |
| `prompts/content-creation/` | Podcast-style conversational script generator |
| `prompts/references/` | External system prompt repos and resources |

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

| Agent | Description | Use when |
|-------|-------------|----------|
| `code-simplifier` | Simplifies and refines code for clarity and maintainability | After writing or editing code — removes duplication, improves naming, preserves behavior |

---

## Commands

Slash commands for Claude Code workflows.

| Command | Description | Use when |
|---------|-------------|----------|
| `commit-commands` | Commit, push, open PRs, clean gone branches | Finishing a feature or fix — run `/commit`, `/commit-push-pr`, or `/clean_gone` |
| `code-review` | Structured multi-agent PR review | Before merging — runs parallel agents checking CLAUDE.md compliance, bugs, and git history |

---

## MCP Server Configurations

Setup guides for Model Context Protocol (MCP) servers — connect Claude to external tools and services.

| Integration | File | Use when |
|-------------|------|----------|
| Notion | `mcp/notion.md` | Reading or writing Notion pages and databases |
| Gmail | `mcp/gmail.md` | Sending, reading, or drafting emails |
| Google Calendar | `mcp/google-calendar.md` | Scheduling, checking, or creating calendar events |
| Google Drive | `mcp/google-drive.md` | Accessing or storing files in Drive |
| Mermaid Chart | `mcp/mermaid-chart.md` | Creating flowcharts, sequence diagrams, ER diagrams |
| Excalidraw | `mcp/excalidraw.md` | Freeform whiteboard-style diagrams and sketches |
| Vercel | `mcp/vercel.md` | Deploying projects or managing Vercel resources |
| Hugging Face | `mcp/hugging-face.md` | Browsing models, datasets, or Spaces on HF Hub |
| Context7 | `mcp/context7.md` | Looking up live documentation for libraries and frameworks |
| Computer Use | `mcp/computer-use.md` | Controlling the desktop — mouse, keyboard, screenshots |

---

## Claude.md Templates

`claude-md/` contains CLAUDE.md templates — project-level instructions that guide Claude's behavior within a codebase.

---

## Plugins

| Plugin | Description | Use when |
|--------|-------------|----------|
| `hookify` | Rule-based hooks that intercept tool calls and warn or block on pattern matches | Preventing Claude from doing something dangerous or undesirable (e.g., blocking `rm -rf`, enforcing test requirements) |
| `ralph-loop` | Stop-hook that feeds Claude a prompt file in a continuous loop until done | Long autonomous tasks where Claude should keep iterating until the goal is complete |

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
