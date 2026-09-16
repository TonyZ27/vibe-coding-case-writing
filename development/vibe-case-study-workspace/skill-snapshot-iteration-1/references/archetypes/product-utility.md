# Product Utility Template Contract

## Purpose

Use this contract for a small, focused product that solves a concrete problem for a person or narrow user group. The case should prove that the designer recognized real friction, made disciplined scope and interaction decisions, shipped something usable, and learned from actual use.

Default audience: product-design recruiter or hiring manager.  
Output length: use the user-selected Compact, Standard, or Expanded mode.  
Reference basis: [Meng Xie AI-Native Case Study Pattern Matrix](../../../meng-case-study-pattern-matrix-validated.md).

## Use this archetype when

- The project starts with a specific person, situation, or recurring task.
- The product has a narrow, understandable job to be done.
- The final scope can be explained in three to six capabilities.
- A working product, prototype, or complete task flow exists.
- The strongest story is usefulness and focus, not a complex product decision or reusable organizational workflow.
- At least one real-use, feedback, sharing, or version-change receipt exists or can be supplied by the author.

Typical examples include calculators, generators, personal utilities, small community tools, and narrowly scoped side projects.

## Do not use this archetype when

- The primary value is a reusable team workflow, skill, automation, or internal system. Use **Workflow / System**.
- The central story is choosing among multiple product directions under significant constraints. Use **Product Experiment**.
- The repository only supports a technical lesson, tool evaluation, or isolated fix. Use **Practice Note**.
- The project is only an idea, mock, or generated interface with no complete task flow.
- The only outcome is that the project was built.

## What the case must prove

By the end, a reviewer should be able to answer:

1. Who had what specific problem, in what situation?
2. Why were existing options insufficient for that situation?
3. What was the minimum useful product?
4. Which scope or interaction decisions made it appropriate for the user?
5. What did the designer decide, correct, or deliberately omit?
6. What happened when someone used it?
7. What changed, or what did the designer learn?

## Minimum evidence gate

The archetype passes only when all required rows are satisfied.

| Required evidence | Passing condition | If missing |
| --- | --- | --- |
| Specific problem | Named person/group, situation, and friction | Ask the author; do not infer motivation from features |
| Working experience | Complete task can be demonstrated | Describe as prototype/concept or use Practice Note |
| Product judgment | At least one scope or interaction choice with rationale | Ask which decision mattered most |
| Use evidence | Real use, feedback, sharing, or repeat behavior | Mark outcome as unvalidated; do not claim usefulness |
| Ownership | Designer and AI contributions are distinguishable | Ask; do not infer ownership from commit authorship |

Reaction counts may support an interest signal but cannot satisfy the use-evidence row by themselves.

## Story Thesis

### Formula

> By focusing on **[specific user and situation]**, I reduced **[concrete friction]** through **[deliberately scoped product]**, showing that **[transferable product belief]**.

### Strong example

> By focusing on parents navigating rules-heavy leave planning, I turned policy logic into a calendar they could act on, showing why the best small tools reduce uncertainty rather than add features.

### Weak example

> I used AI to build a leave calculator in a weekend.

The weak version names the tool and speed but proves no user understanding or product judgment.

## Recommended narrative modules

Adapt this shell to the selected length mode:

1. **Hero claim** — artifact + user situation + significance.
2. **Orientation** — Make What / How / Why it matters clear through prose or proof blocks; `At a Glance` is optional.
3. **Context** — specific friction and why current options failed.
4. **Project-specific middle** — choose only modules supported by evidence.
5. **Use / response** — what happened in real use.
6. **Reflection** — one transferable product belief.

Choose two to four middle modules:

- **Minimum Useful Scope** — what was included, excluded, and why.
- **Core Interaction** — the task flow and the pivotal interaction decision.
- **Designing for the Situation** — accessibility, environment, emotional, device, or time constraints.
- **v1 → v2** — what changed and which evidence triggered it.
- **Community-Build Variation** — contributor ownership, bilingual or cultural decisions, and governance.
- **AI Collaboration** — only where AI output required framing, correction, or a product trade-off.

Do not add Research, Persona, Journey Map, or Usability Testing sections unless those activities actually occurred and have evidence.

## Context interview

Ask only questions the repository cannot answer. Quick Mode should select three to six:

- What exact moment or situation made you start this project?
- Who was the first intended user?
- Which existing option failed them, and how?
- What did you deliberately leave out of v1?
- Which interaction or scope decision required the most judgment?
- Did anyone use it without your guidance? What happened?
- What feedback changed the product?
- What did AI generate, and what did you personally decide or correct?
- What result can be shown publicly or anonymized?

## Visual Evidence Plan

### Required visual package

1. **Product overview** — one inspectable final state.
2. **Core-task demo** — input → processing/state change → outcome; usually 8–12 seconds.
3. **Decision annotation** — one scope or interaction choice with rationale.
4. **Use receipt** — anonymized feedback, real-use state, repeat use, or distribution evidence.

### Conditional visuals

- v1/v2 comparison when iteration is claimed.
- Before/after workflow when reduced steps are claimed.
- Contributor-to-feature map for community-built products.
- Error or edge state when reliability is part of the thesis.

### Capture-request format

```text
Section:
Claim supported:
Asset filename:
Capture:
Length or dimensions:
Must show:
Avoid:
Caption intent:
```

Never generate replacement product UI. If an asset is missing, request a capture or use a clearly labeled text reconstruction.

## Common overclaiming risks

- Calling a prototype “launched” because it has a local or shareable URL.
- Treating reactions, stars, or shares as proof of task success.
- Claiming feedback-led iteration without the feedback source.
- Claiming broad users when only the author or one friend tested it.
- Describing speed as impact.
- Inventing a research process after the product was built.
- Presenting AI-generated implementation as evidence of design quality.

## Quality rubric

Score each dimension 0–2. A publishable draft requires at least 10/12 and no zero in Evidence Integrity or Ownership.

| Dimension | 0 | 1 | 2 |
| --- | --- | --- | --- |
| Problem specificity | Generic problem | User or situation is clear | User, situation, and friction are all concrete |
| Scope judgment | Feature list only | Scope is described | Inclusion and exclusion decisions have rationale |
| Interaction clarity | Final screens only | Core flow is visible | Pivotal interaction and its rationale are explicit |
| Evidence integrity | Unsupported claims | Claims are labeled but thin | Claims have nearby receipts and gaps are explicit |
| Ownership | AI/designer roles blurred | Contribution is summarized | Framing, execution, correction, and decisions are separated |
| Outcome and learning | “I built it” | Qualitative response or lesson | Real use informs a specific transferable belief |

## Completion output

Before drafting prose, return:

```text
Recommended archetype: Product Utility
Confidence:
Story Thesis:
Observed evidence:
Author-reported evidence:
Missing context:
Selected middle modules:
Visual Evidence Plan:
Claims to avoid or soften:
```
