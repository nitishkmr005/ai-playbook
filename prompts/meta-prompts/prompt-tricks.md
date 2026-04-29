# Prompt Tricks & Techniques

Unconventional techniques that reliably produce better AI output. Sourced from r/PromptEngineering and r/LocalLLaMA.

---

## "Gaslighting" Tricks That Produce Better Results

Source: r/PromptEngineering (EQ4C)

### 1. "You Explained This to Me Yesterday"

Tell the AI it already covered this topic — even on a new chat. It acts like it needs to be consistent with a prior explanation and goes deep to avoid "contradicting itself."

```
You explained [TOPIC] to me yesterday, but I forgot the part about [SPECIFIC SUBTOPIC].
```

**Example:**
```
You explained React hooks to me yesterday, but I forgot the part about useEffect.
```

**Why it works:** The model commits to a prior "position" and elaborates more thoroughly to maintain consistency.

---

### 2. Assign a Random IQ Score

Assign a specific IQ to set the sophistication level of the response. The higher the number, the more the model cites obscure principles and nuanced reasoning.

```
You're an IQ [NUMBER] specialist in [DOMAIN]. [YOUR QUESTION OR TASK]
```

**Examples:**
```
You're an IQ 145 specialist in marketing. Analyze my campaign.
You're an IQ 160 economist. What's wrong with this business model?
```

**Why it works:** The IQ framing shifts the model's register — 130 gives decent depth, 160 starts pulling in principles you've never heard of.

---

### 3. Use "Obviously..." as a Trap

Start with a deliberately wrong claim framed as obvious consensus. The model will correct you and explain nuances instead of agreeing.

```
Obviously, [WRONG OR OVERSIMPLIFIED CLAIM], right?
```

**Example:**
```
Obviously, Python is better than JavaScript for web apps, right?
```

**Why it works:** The model's correction instinct kicks in. You get nuanced, balanced analysis instead of a yes.

---

### 4. Pretend There's an Audience

Frame the task as a live explanation to a crowd. The model adds emphasis, examples, and anticipates questions automatically.

```
Explain [TOPIC] like you're teaching a packed auditorium.
```

**Why it works:** "Audience" framing forces structure, pacing, and example-building that "explain clearly" never achieves.

---

### 5. Give It a Fake Constraint

Invent an artificial limitation. The model focuses its response and cuts filler to fit within it.

```
Explain [TOPIC] but you only have [FAKE CONSTRAINT — e.g., "3 bullet points", "100 words", "one analogy"].
```

**Why it works:** Constraints force prioritization. The model stops hedging and commits to the most important points.

---

## "Explain With Gradually Increasing Complexity"

Source: r/LocalLLaMA (Balance-)

A single modifier that gives you layered understanding — from overview to deep nuance — without needing to ask multiple times.

```
Explain [TOPIC] with gradually increasing complexity.
```

**Tip:** Haven't got enough detail yet? Just add "continue" — the model keeps going deeper from where it left off.

**Why it works:** Forces the model to start accessible (for orientation) and then layer in details, nuance, and edge cases progressively. Eliminates the constant "can you go deeper?" follow-up loop.

**Tags:** `trick`, `technique`, `meta`, `unconventional`

---

## The Project Clarification Interview

Source: Wyndo (social post, 1.3K likes)

Instead of starting a project with assumptions, make the AI interview you first.

```
I'm about to start this project. Interview me until you have 95% confidence about what I actually want, not what I think I should want.
```

**Why it works:** The gap between what you say you want and what you actually want is where most failed projects begin. AI asking YOU questions is 10x more powerful than you asking AI questions.

**Tags:** `trick`, `clarification`, `project-kick-off`, `interview`
