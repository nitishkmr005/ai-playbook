# Analysis & Strategy — Prompts 11–20

---

## 11 · The SWOT Analyzer

```
Perform a comprehensive SWOT analysis of [COMPANY/PRODUCT/STRATEGY].

For each quadrant (Strengths, Weaknesses, Opportunities, Threats):
- List 5 specific items (not generic — tied to THIS specific situation)
- For each item: one sentence explaining WHY it belongs in this quadrant
- Rate each item's impact: High / Medium / Low

Then provide:
- The #1 strategic priority based on this analysis (one sentence)
- The biggest risk if this priority is ignored (one sentence)
- The first action to take this week (one specific, actionable step)
```

**Variables:** `[COMPANY/PRODUCT/STRATEGY]`

---

## 12 · The Decision Matrix

```
I need to decide between these options: [LIST 2-4 OPTIONS]

Context: [RELEVANT BACKGROUND — budget, timeline, team, goals]

Build a decision matrix:
1. Identify the 5 most important criteria for this decision (ask me if unsure)
2. Weight each criterion by importance (must total 100%)
3. Score each option against each criterion (1-10)
4. Calculate weighted scores
5. Present as a formatted table

Then write a 2-paragraph recommendation that:
- Clearly states which option to choose and why
- Acknowledges the strongest argument for the runner-up
- Identifies the one condition that would change the recommendation
```

**Variables:** `[OPTIONS]`, `[CONTEXT]`

---

## 13 · The Root Cause Analyzer

```
Here is a problem I am facing: [DESCRIBE THE PROBLEM AND ITS SYMPTOMS]

Perform a root cause analysis:
1. Ask "Why?" 5 times in sequence (the 5 Whys technique), going deeper each time
2. For each level, identify whether this is a symptom or a root cause
3. At the deepest level, identify the TRUE root cause
4. Propose 3 solutions — one for the surface symptom, one for the mid-level cause, and one for the root cause
5. Recommend which solution to implement and why

Do not accept my initial framing of the problem at face value. The real problem is often not the one I described.
```

**Variables:** `[PROBLEM AND SYMPTOMS]`

---

## 14 · The Market Opportunity Scanner

```
Analyze the market opportunity for [PRODUCT/SERVICE IDEA].

Evaluate:
1. DEMAND: Who wants this? How many of them are there? How do you know they want it?
2. COMPETITION: Who else does this? What do they charge? Where are they weak?
3. TIMING: Why now? What changed that makes this viable today when it was not before?
4. MOAT: What would prevent competitors from copying this in 6 months?
5. UNIT ECONOMICS: What would this cost to deliver per customer vs. what could you charge?

For each section: be specific, use numbers where possible, and flag anything you are uncertain about.

End with a GO / CAUTIOUS GO / NO GO recommendation with your confidence level (high/medium/low).
```

**Variables:** `[PRODUCT/SERVICE IDEA]`

---

## 15 · The Meeting Strategist

```
I have a meeting about [TOPIC] with [WHO — their role, relationship, what they care about].

My goal for this meeting: [WHAT YOU WANT TO ACHIEVE]

Prepare:
1. Opening statement (2 sentences — sets the right frame for the conversation)
2. 3 key points I must communicate (in priority order)
3. 3 questions I should ask (ordered from most to least important)
4. 3 likely objections and how to respond to each
5. My ideal closing statement (summarizes agreement and next steps)
6. Walk-away point: what is the minimum acceptable outcome?
```

**Variables:** `[TOPIC]`, `[WHO]`, `[YOUR GOAL]`

---

## 16 · The Pricing Strategist

```
Help me price [PRODUCT/SERVICE].

Context:
- What it does: [DESCRIPTION]
- Who it is for: [TARGET CUSTOMER]
- What it costs me to deliver: [YOUR COSTS]
- Competitor pricing: [WHAT ALTERNATIVES CHARGE, if known]
- Value delivered: [WHAT THE CUSTOMER GETS — time saved, money earned, problems solved]

Design a pricing structure:
1. Three tiers (entry, core, premium) with names that reflect value, not size
2. What is included in each tier and WHY each boundary exists
3. The psychology behind each price point
4. Which tier most customers should land on and how to guide them there
5. One-time vs. recurring analysis — which model fits better and why

Show the pricing in a formatted comparison table.
```

**Variables:** `[PRODUCT/SERVICE]`, `[DESCRIPTION]`, `[TARGET CUSTOMER]`, `[YOUR COSTS]`, `[COMPETITOR PRICING]`, `[VALUE DELIVERED]`

---

## 17 · The Competitive Teardown

```
Perform a competitive teardown of [COMPETITOR NAME/URL].

Analyze:
1. POSITIONING: What is their core message? Who are they targeting? What emotion are they selling?
2. PRODUCT: What do they actually offer? What is the core feature vs. nice-to-haves?
3. PRICING: How do they charge? What does each tier include? Where is the profit margin?
4. CONTENT: What topics do they publish about? How often? What format performs best?
5. WEAKNESS: Where are they vulnerable? What do their customers complain about? What are they not doing?

End with: "If I were competing directly with [COMPETITOR], the 3 things I would do differently are..."
```

**Variables:** `[COMPETITOR NAME/URL]`

---

## 18 · The OKR Builder

```
Help me create OKRs for [TEAM/INDIVIDUAL/COMPANY] for [TIME PERIOD].

Context: [CURRENT SITUATION — where we are, where we want to go, what resources we have]

For each Objective (suggest 3):
- The Objective: ambitious but achievable, qualitative, inspiring
- 3-4 Key Results: specific, measurable, time-bound
- For each Key Result: the current baseline, the target, and how you would measure it
- A confidence level (1-10) that this Key Result is achievable in the timeframe

Flag any Key Results that might conflict with each other.
```

**Variables:** `[TEAM/INDIVIDUAL/COMPANY]`, `[TIME PERIOD]`, `[CONTEXT]`

---

## 19 · The Risk Assessor

```
I am about to [DESCRIBE THE INITIATIVE/DECISION/PROJECT].

Perform a risk assessment:
1. List the 7 most likely risks (things that could go wrong)
2. For each risk:
   - Probability: High / Medium / Low
   - Impact if it occurs: High / Medium / Low
   - Early warning sign (how would I detect this risk materializing?)
   - Mitigation strategy (what would I do to prevent it?)
   - Contingency plan (what would I do if it happens anyway?)
3. Plot all risks on a 2x2 matrix (probability vs. impact)
4. Identify the top 3 risks I should actively monitor

Be pessimistic. I want to hear about risks I have not considered, not reassurance that everything will be fine.
```

**Variables:** `[INITIATIVE/DECISION/PROJECT]`

---

## 20 · The Retrospective Facilitator

```
Facilitate a retrospective for this project/period: [DESCRIBE WHAT HAPPENED]

Structure:
1. WHAT WENT WELL (identify 5 specific things that worked, with evidence)
2. WHAT WENT WRONG (identify 5 specific things that did not work, with root causes)
3. WHAT WE LEARNED (3 lessons that will change how we work going forward)
4. WHAT WE WILL DO DIFFERENTLY (3 specific, actionable changes — not vague intentions)
5. WHAT WE WILL STOP DOING (2 things we should deliberately stop)

Rules:
- Be specific. "Communication was bad" is useless. "The product team was not informed about the pricing change until 2 days before launch, causing a scramble to update marketing materials" is useful.
- For every problem identified, include a specific preventive action.
```

**Variables:** `[WHAT HAPPENED]`
