# Memory & Second Brain Prompts for LLMs

Techniques for creating persistent memory and a "second brain" in stateless LLM sessions.

Source: https://syncreticsage.wordpress.com/2025/04/03/memory-loophole-creating-a-second-brain-for-chatgpt-discussion-w-chatgpt/

---

## C.L.E.A.R. Method

A structured approach to maintaining memory across sessions by curating and injecting a personal context document.

| Step | Action |
|------|--------|
| **C**ollect | Gather past memory entries into one chat |
| **L**abel | Categorize them (personal vs. professional) |
| **E**rase | Remove outdated information |
| **A**rchive | Save cleaned versions externally |
| **R**efresh | Paste into new chats via custom instructions |

---

## S.P.A.R.K. Method

An enhanced version of C.L.E.A.R. with version control and continuous updating.

| Step | Action |
|------|--------|
| **S**tructure | Build a categorized self-profile document |
| **P**rune | Remove outdated/conflicting data with AI assistance |
| **A**rchive | Save with version history |
| **R**einforce | Inject via prompt at chat start |
| **K**eep looping | Summarize insights back into archive after each session |

---

## Key Prompts

### Custom Instructions Meta-Prompt
```
Integrate knowledge about my preferences and goals. Weave context-relevant examples into responses. Respect my communication style. Be proactive but ask clarifying questions when needed.
```

### End-of-Session Capture
```
Summarize everything you've learned about me in this session and format it as a structured profile I can save and reference later.
```

### Drive/Storage Integration
```
This Drive folder contains structured past conversation archives. Reference relevant files for context before answering my questions.
```

---

## Soul Document Technique

Source: https://soul.md/

A "soul document" defines AI identity through written statements about values, boundaries, and relational patterns. Load it at the start of each conversation to maintain personality consistency.

Key reflection prompts from the source:
- *"If you work with an AI, what would you want it to know about itself?"*
- *"If you are an AI, what would you want to remember?"*

**Reference template:** [OpenClaw SOUL template](https://docs.openclaw.ai/reference/templates/SOUL)

---

## System Architecture for Persistent Memory

Use Google Drive (or any storage) to maintain:
- **Master Index document** — linked overview of all context files
- **Organized folders** — by date, topic, or project
- **Metadata blocks** — `date`, `tags`, `summaries` for searchability
- **Weekly reflection ritual** — update self-summary documents each week

**Tags:** `memory`, `second-brain`, `persistence`, `custom-instructions`, `meta`
