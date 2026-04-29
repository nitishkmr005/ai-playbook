# Technical & Development — Prompts 21–28

---

## 21 · The Architecture Advisor

```
I want to build [DESCRIBE THE SYSTEM].

Requirements:
- [REQUIREMENT 1]
- [REQUIREMENT 2]
- [REQUIREMENT 3]
- Expected scale: [USERS/DATA VOLUME]
- Budget constraints: [ANY LIMITATIONS]

Propose 2 architectural approaches. For each:
1. Component diagram (described in text — list every service/module and how they connect)
2. Technology choices with reasoning for each
3. Pros and cons (be honest about tradeoffs)
4. Estimated complexity: Simple / Moderate / Complex
5. The #1 thing that could go wrong with this approach

Recommend one approach. Explain why. Then give me the first 5 implementation steps in order.
```

**Variables:** `[SYSTEM DESCRIPTION]`, `[REQUIREMENTS]`, `[SCALE]`, `[BUDGET CONSTRAINTS]`

---

## 22 · The Code Reviewer

```
Review this code:

<code>
[PASTE CODE]
</code>

Check for:
1. SECURITY: Injection vulnerabilities, exposed secrets, XSS, insecure data handling
2. LOGIC: Edge cases not handled, incorrect conditional logic, off-by-one errors
3. PERFORMANCE: N+1 queries, unnecessary computations, missing caching opportunities
4. READABILITY: Unclear naming, missing comments on complex logic, overly nested code
5. BEST PRACTICES: Violations of language conventions, missing error handling, unused imports

For each issue found:
- Severity: Critical / High / Medium / Low
- Exact location (line or function name)
- Why it is a problem (not just what is wrong, but what could happen)
- The fix (show corrected code)

If the code is clean, say so. Do not invent issues to seem thorough.
```

**Variables:** `[CODE]`

---

## 23 · The Debug Diagnostician

```
I am getting this error: [PASTE COMPLETE ERROR MESSAGE AND STACK TRACE]

Context: [WHAT THE CODE IS SUPPOSED TO DO]

1. Do NOT jump to a fix immediately
2. First: explain what this error message means in plain English
3. Second: list the 3 most likely root causes in order of probability
4. Third: for each potential cause, explain what evidence would confirm it
5. Fourth: once the root cause is identified, show the fix
6. Fifth: explain what would prevent this type of bug in the future

[PASTE RELEVANT CODE]
```

**Variables:** `[ERROR MESSAGE + STACK TRACE]`, `[CONTEXT]`, `[RELEVANT CODE]`

---

## 24 · The API Designer

```
Design a REST API for [DESCRIBE THE SYSTEM/FEATURE].

For each endpoint:
- Method and path (following REST conventions)
- Request body schema (with required/optional fields)
- Response schema (success and error cases)
- Authentication requirements
- Rate limiting recommendation

Also include:
- Error response format (consistent across all endpoints)
- Pagination approach for list endpoints
- Versioning strategy
- 3 potential security concerns and how to address each

Present as a formatted API reference document.
```

**Variables:** `[SYSTEM/FEATURE DESCRIPTION]`

---

## 25 · The Database Schema Designer

```
Design a database schema for [DESCRIBE THE APPLICATION].

Requirements:
- [LIST KEY ENTITIES AND RELATIONSHIPS]
- Expected scale: [DATA VOLUME AND GROWTH RATE]

For each table:
- Columns with types, constraints, and descriptions
- Primary key and indexes
- Foreign key relationships

Also provide:
- An entity relationship description (how tables connect)
- 3 common queries this schema must support efficiently
- Index recommendations for those queries
- One potential scaling concern and how to address it
- Migration strategy if requirements change later
```

**Variables:** `[APPLICATION DESCRIPTION]`, `[ENTITIES AND RELATIONSHIPS]`, `[SCALE]`

---

## 26 · The Test Case Generator

```
Generate comprehensive test cases for this function/feature:

<code_or_description>
[PASTE CODE OR DESCRIBE THE FEATURE]
</code_or_description>

Test categories:
1. HAPPY PATH: 3 tests for normal, expected usage
2. EDGE CASES: 5 tests for boundary conditions, empty inputs, maximum values
3. ERROR CASES: 3 tests for invalid inputs, missing data, system failures
4. SECURITY: 2 tests for injection attempts, unauthorized access
5. PERFORMANCE: 1 test for behavior under load or with large datasets

For each test:
- Test name (descriptive)
- Input
- Expected output
- Why this test matters
```

**Variables:** `[CODE OR FEATURE DESCRIPTION]`

---

## 27 · The Documentation Writer

```
Write developer documentation for this code/API/system:

<code_or_spec>
[PASTE CODE OR SPECIFICATION]
</code_or_spec>

Include:
1. Overview (what this does and why it exists — 2-3 sentences)
2. Quick Start (get up and running in under 5 minutes)
3. Core Concepts (explain the mental model, not just the API surface)
4. API Reference (every public function/endpoint with parameters, return values, and examples)
5. Common Patterns (3 typical usage patterns with code examples)
6. Troubleshooting (5 common issues and their solutions)

Write for a developer who is smart but has never seen this codebase before.
```

**Variables:** `[CODE OR SPECIFICATION]`

---

## 28 · The Refactoring Planner

```
This code needs refactoring:

<code>
[PASTE CODE]
</code>

Analyze:
1. What are the top 3 code quality issues? (duplicated logic, mixed responsibilities, unnecessary complexity)
2. For each issue: explain WHY it is a problem, not just that it exists
3. Propose a refactoring plan with specific steps in order
4. For each step: show the before and after code
5. Verify that the refactored code maintains identical external behavior
6. Estimate the impact: how much does this improve maintainability, readability, and testability?

Do NOT change external behavior. Internal improvement only.
```

**Variables:** `[CODE]`
