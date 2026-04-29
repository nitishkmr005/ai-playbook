# Tree of Thought Prompts

Structured multi-perspective reasoning frameworks.

---

## Three Expert Consultants (Business Challenge)

Forces the model to explore multiple solution paths, debate disagreements, and converge on a recommendation.

```
Act as 3 expert business consultants evaluating this challenge: [INSERT BUSINESS CHALLENGE]

Each consultant will:
1. Identify 3 possible approaches
2. For each approach, explore 2-3 potential outcomes
3. Evaluate pros/cons of each path
4. Recommend the optimal solution with reasoning

Consultants should debate any disagreements before final recommendation. Think step by step while performing this task.
```

**Usage:** Replace `[INSERT BUSINESS CHALLENGE]` with your specific problem.
**Tags:** `tree-of-thought`, `reasoning`, `business`, `debate`, `multi-perspective`

---

## Notes

- Tree of Thought works best for complex, open-ended problems with no single obvious answer.
- The "debate disagreements" instruction forces the model to surface genuine trade-offs rather than converging prematurely.
- Can be adapted by changing the number of consultants, the domain (e.g., engineers, scientists, product managers), or the depth of exploration per branch.
