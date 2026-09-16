# Practice Note Fallback Contract

## Purpose

Use this format when a repository contains a useful constraint, failure, tool evaluation, technical lesson, or personal workflow but cannot support a full product case study without inventing users, decisions, iteration, or outcomes.

Practice Note is an evidence-preserving fallback, not a lesser case study and not a fourth archetype. It should make one useful judgment clearly and stop before the evidence runs out.

Default audience: product-design recruiter, hiring manager, or peer practitioner.  
Default output: a focused note readable in two to three minutes.  
Reference basis: [Meng Xie AI-Native Case Study Pattern Matrix](../../../meng-case-study-pattern-matrix-validated.md).

## Route here when

- The repository documents one hard constraint and how it was resolved.
- A pure-AI or initial approach failed and a hybrid method worked.
- The strongest artifact is a tool evaluation or landscape comparison.
- The project produced a useful technical or design-working lesson but little user evidence.
- The workflow has not been packaged or adopted beyond the creator.
- The product is incomplete, private, or too weakly evidenced for a full case study.
- The author wants to share a method honestly without retrofitting a conventional UX process.

## Do not use this format when

- A specific user problem, working utility, and use evidence support **Product Utility**.
- A meaningful product question, constraint, decision, and real-state validation support **Product Experiment**.
- A repeatable system, real output, packaging, and adoption support **Workflow / System**.
- The material synthesizes several completed cases into a capability model. That is a **Portfolio Thesis**, which is outside the Repo-to-Case-Study flow.
- There is no evidence-backed lesson at all. Recommend documenting the project privately rather than publishing a note.

## What the note must prove

By the end, a reader should be able to answer:

1. What specific question, constraint, or failure occurred?
2. Why did the obvious or first approach fail?
3. What method, comparison, or handoff worked better?
4. What concrete evidence supports that judgment?
5. When should another practitioner apply or avoid the lesson?

## Minimum evidence gate

| Required evidence | Passing condition | If missing |
| --- | --- | --- |
| Specific trigger | A concrete constraint, question, or failed approach | Do not publish a generic AI reflection |
| Evidence-backed contrast | Before/after, option comparison, test, output, or observed failure | State the note as a question still being explored |
| Author judgment | The author made a choice, handoff, or recommendation | Ask what was learned; do not infer it from the code |
| Transfer boundary | The note says when the lesson applies and where it may not | Add an explicit limitation section |
| Ownership | AI, tools, collaborators, and author roles are distinguishable | Ask before drafting |

No user research, adoption, or business outcome is required. If those do not exist, do not add substitutes.

## Recommended variants

### Constraint and handoff

Use for a hard limit, failed automation, or hybrid AI/manual solution.

`Constraint → Failed route → Handoff strategy → Result → Reusable lesson`

### Tool evaluation

Use for a comparative trial or recommendation.

`Decision context → Evaluation lens → Options → Trade-offs → Recommendation → Limits`

### Build lesson

Use for a repository that surfaced one useful design or implementation insight.

`What I tried → What broke → What changed → Evidence → What I would do next`

Select one variant. Do not combine unrelated lessons into a broad “what I learned about AI” article.

## Story Thesis

### Constraint-and-handoff formula

> When **[approach]** failed under **[specific constraint]**, splitting the work between **[AI/tool role]** and **[human role]** produced **[evidenced result]**, revealing **[bounded lesson]**.

### Tool-evaluation formula

> Comparing **[options]** against **[decision context]** showed that **[tool/method]** is best for **[specific use]**, but not for **[explicit limitation]**.

### Strong example

> When automated SVG simplification kept breaking the asset or exceeding the pipeline limit, using AI for diagnosis and validation while handling two complex paths manually reduced the file from 18K to 8K characters and passed the pipeline.

### Weak example

> AI is powerful, but humans are still important.

The weak version is generic, unbounded, and unsupported by a concrete event.

## Recommended structure

1. **Title as judgment** — name the constraint or conclusion, not the tool alone.
2. **Orientation** — Make Question / Method / Takeaway clear through neutral prose; `At a Glance` is optional and should not receive proof styling.
3. **Context** — enough detail to understand why the issue mattered.
4. **What happened** — the failure, comparison, or observed behavior.
5. **What worked** — method and evidence.
6. **Where this applies** — recommendation and boundaries.

Optional modules:

- **Decision matrix** for tool evaluation.
- **AI / human handoff** for hybrid workflows.
- **Before / after** for measurable technical or workflow change.
- **Honest limitations** when the preferred method has clear unsuitable uses.
- **Next experiment** when the result is promising but incomplete.

## Context interview

Quick Mode should select two to five questions:

- What exactly failed or remained uncertain?
- What constraint made the obvious approach inadequate?
- What alternatives did you actually try?
- What evidence changed your judgment?
- What did AI do, and where did you intervene?
- What result can be demonstrated or measured?
- When would you not recommend this method?
- What remains unverified?

## Visual Evidence Plan

### Required visual package

1. **Trigger evidence** — limit, error, old workflow, or decision context.
2. **Contrast** — failed vs. successful output or side-by-side options.
3. **Method** — compact handoff flow or evaluation matrix.
4. **Result** — final artifact, passing state, or inspectable output.

### Rules

- Do not fabricate a before state.
- Do not create a formal score if the author did not use one.
- Label reconstructed workflows.
- Keep screenshots large enough to inspect.
- Use numbers only when the measurement basis is known.
- A generated diagram may explain a verified relationship, but it must not invent research, users, metrics, or product UI.

## Common overclaiming risks

- Expanding one failure into a universal principle.
- Calling a personal workaround a reusable system.
- Presenting a tool trial as product research.
- Claiming performance improvement without a consistent baseline.
- Adding imagined users or business value to make the note feel larger.
- Hiding the manual step that made the result work.
- Treating a clean final output as proof that the method is reliable across cases.

## Quality rubric

Score each dimension 0–2. A publishable note requires at least 8/10 and no zero in Specificity or Evidence Integrity.

| Dimension | 0 | 1 | 2 |
| --- | --- | --- | --- |
| Specificity | Generic topic | Event or constraint named | Exact trigger and stakes are concrete |
| Contrast | One final output | Before/after stated | Failure and success are inspectable |
| Judgment | Tool activity only | Lesson stated | Evidence clearly supports a bounded recommendation |
| Evidence integrity | Unsupported generalization | Gaps labeled | Claims stay within demonstrated evidence |
| Transfer boundary | Universal claim | Limitation mentioned | Suitable and unsuitable contexts are explicit |

## Completion output

Before drafting, return:

```text
Recommended format: Practice Note
Confidence:
Reason a full case study is not supported:
Selected variant:
Story Thesis:
Observed evidence:
Author-reported evidence:
Missing context:
Visual Evidence Plan:
Claims to avoid or soften:
What evidence would upgrade this to a full case study:
```
