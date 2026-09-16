# Product Experiment Template Contract

## Purpose

Use this contract for a new product bet, consequential interaction, or high-fidelity prototype where the strongest story is how the designer made and tested a decision under real constraints.

Default audience: product-design recruiter or hiring manager.  
Output length: use the user-selected Compact, Standard, or Expanded mode.  
Reference basis: [Meng Xie AI-Native Case Study Pattern Matrix](../../../meng-case-study-pattern-matrix-validated.md).

## Use this archetype when

- The project begins with a product hypothesis, new behavior, or unresolved design question.
- The repository or design artifacts expose competing directions, significant iteration, or a consequential choice.
- Platform, data, performance, business, trust, or system constraints shaped the solution.
- A real-state prototype, working build, or complete interaction flow exists.
- The case can explain what was learned or decided—not merely what was produced.

Typical examples include hackathon product bets, 0→1 features, coded prototypes, production-code experiments, and new interaction models.

## Do not use this archetype when

- The project is a focused utility whose primary proof is usefulness. Use **Product Utility**.
- The durable value is a repeatable workflow or skill used by others. Use **Workflow / System**.
- No alternative, constraint, decision, or validation question can be identified. Use **Practice Note** or request more context.
- The repository contains several generated concepts but no evidence that they answer different product questions.
- The only proof is lines of code, prompt count, build speed, or visual polish.

## What the case must prove

By the end, a reviewer should be able to answer:

1. What product bet or design question was being tested?
2. Why could ordinary mockups or the existing approach not answer it?
3. Which constraints made the decision difficult?
4. What alternatives were considered, and how did they differ meaningfully?
5. Which direction was selected, rejected, or reframed—and why?
6. What did real-state validation reveal?
7. What outcome, decision, or framework followed?

## Minimum evidence gate

| Required evidence | Passing condition | If missing |
| --- | --- | --- |
| Product question | One explicit hypothesis, uncertainty, or decision | Ask the author; do not derive intent from implementation |
| Constraint | At least one concrete constraint shaped the work | Re-route to Product Utility if the story is only usefulness |
| Decision evidence | Alternatives, iteration, or a documented trade-off | Do not claim exploration; use a single-direction narrative |
| Real-state validation | Working flow, build, test, or realistic state evidence | Label as concept exploration, not validated experiment |
| Decision or learning | The work changed a direction, surfaced a constraint, or produced a reusable judgment | Use Practice Note if only a technical lesson remains |
| Ownership | Designer, AI, engineering, and collaborator roles are distinguishable | Ask before drafting |

## Story Thesis

### Formula

> By testing **[product bet]** under **[real constraint]**, I learned that **[decision or principle]**, which changed **[product direction, review, or team understanding]**.

### Strong example

> By building five upgrade-flow directions inside the production Android environment, I exposed state and performance constraints before selection, turning an abstract review into a decision people could make on real devices.

### Weak example

> I generated five designs with Claude Code and wrote 2,500 lines of code.

The weak version reports output volume but does not identify the product question, decision, or consequence.

## Recommended narrative modules

Adapt this shell to the selected length mode:

1. **Hero claim** — product bet + real constraint + consequence.
2. **Orientation** — Make What / How / Why it matters clear through neutral prose; `At a Glance` is optional and should not receive proof styling.
3. **Context** — the uncertainty and why it mattered.
4. **Experiment middle** — modules selected from the evidence.
5. **Decision / outcome** — what changed because of the experiment.
6. **Reflection or framework** — the transferable design judgment.

Choose two to five middle modules:

- **The Bet** — expected user or product behavior and what remained uncertain.
- **Why Existing Fidelity Was Insufficient** — what a static or isolated prototype could not reveal.
- **Constraints** — platform, state, performance, business, trust, or implementation boundaries.
- **Competing Directions** — comparable alternatives tied to distinct hypotheses.
- **Decision Moment** — selection criteria, review evidence, and rejected trade-offs.
- **Real-State Validation** — physical device, live data, edge cases, or system behavior.
- **AI Division of Labor** — what AI generated or inspected and where human judgment intervened.
- **System Spin-Off** — an adjacent workflow or tool only if it emerged directly from the product work and has separate proof.

Do not include every generated direction. Include only directions that clarify the decision.

## Context interview

Quick Mode should select three to six questions that the artifacts cannot answer:

- What was the exact decision or uncertainty at the start?
- Why was the existing prototype fidelity insufficient?
- Which constraint most changed the design?
- What were the meaningful differences between the directions?
- Which direction won or was rejected, and who made that decision?
- What did a real device, real state, or review reveal that a mock did not?
- Which AI output was wrong, unstable, or misleading?
- What did you personally frame, design, correct, or decide?
- What product or team outcome followed the experiment?

## Visual Evidence Plan

### Required visual package

1. **Bet and constraint** — a compact diagram or annotated context artifact.
2. **Comparable directions** — two to five alternatives shown at the same scale and state.
3. **Decision evidence** — selected direction plus rationale or trade-off.
4. **Real-state demo** — physical device, working build, realistic data, or complete behavior.
5. **Outcome receipt** — review decision, selected direction, discovered edge case, or resulting framework.

### Conditional visuals

- Edge-case sequence when trust or state management is central.
- Performance or animation capture when static artifacts hid the issue.
- Before/after review evidence when the experiment changed team decision quality.
- System-spin-off input/output only when the secondary workflow is genuinely part of the thesis.

### Comparison rules

- Keep direction screenshots at the same size and state.
- Annotate differences in product behavior, not merely styling.
- State which question each direction tested.
- Do not imply a formal scoring model unless one existed.
- Do not fabricate a discarded alternative to make the process look richer.

## Common overclaiming risks

- Calling generated alternatives “exploration” when they differ only visually.
- Treating code volume, token cost, or build speed as design impact.
- Claiming production validation when the work was never tested in a production-like state.
- Saying a direction “won” without a decision source.
- Claiming user validation from stakeholder review.
- Presenting discovered engineering constraints as user insights.
- Allowing a system spin-off to overwhelm the original product decision.

## Quality rubric

Score each dimension 0–2. A publishable draft requires at least 12/14 and no zero in Product Question, Decision Logic, Evidence Integrity, or Ownership.

| Dimension | 0 | 1 | 2 |
| --- | --- | --- | --- |
| Product question | No uncertainty stated | General goal | Specific hypothesis or decision |
| Constraint | Technology list | Constraint named | Constraint visibly changes the design |
| Alternatives | Output gallery | Alternatives differ | Alternatives test distinct product ideas |
| Decision logic | No selection | Selection stated | Evidence and trade-offs explain the decision |
| Real-state validation | Mock only | Working state shown | Real state reveals something decisive |
| Evidence integrity | Claims exceed receipts | Most claims labeled | Claims, receipts, and gaps are explicit |
| Ownership | Roles blurred | Contributions summarized | Design, AI, engineering, and collaborators separated |

## Completion output

Before drafting prose, return:

```text
Recommended archetype: Product Experiment
Confidence:
Product question:
Primary constraint:
Story Thesis:
Observed evidence:
Author-reported evidence:
Missing context:
Directions worth showing:
Decision evidence:
Visual Evidence Plan:
Claims to avoid or soften:
```
