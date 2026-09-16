---
name: vibe-case-study
description: Turn a vibe-coded repository, project context, and evidence into an evidence-safe product-design case study. Use whenever a user wants to convert an AI-built project or repo into a portfolio story, choose an appropriate case-study structure or length, diagnose missing context, plan proof visuals, or write a Practice Note when the evidence cannot support a full case.
---

# Vibe Case Study

Build a causal portfolio story from repository evidence and author context. Show both the product judgment and, when supported, how the designer's ability to build with AI changed. Do not retrofit a conventional UX process or imitate any reference author's voice.

Default to English unless the user requests another language.

## Read the relevant references

- Read [length modes](references/editorial/length-modes.md) before recommending article length.
- Read [proof blocks](references/editorial/proof-blocks.md) before outlining the public article.
- Read the [source-library index](references/source-library/index.md), then load only the source collection whose patterns could sharpen the story. Treat source patterns as prompts for project-specific reasoning, never as evidence for the current project.
- Read only the selected archetype contract:
  - [Product Utility](references/archetypes/product-utility.md)
  - [Product Experiment](references/archetypes/product-experiment.md)
  - [Workflow / System](references/archetypes/workflow-system.md)
- Use the [Practice Note fallback](references/formats/practice-note.md) when evidence cannot support a full case.

## Workflow

### 1. Build an evidence map

Separate inputs before writing:

- **Observed:** directly visible in the repository, documentation, history, assets, tests, or working product.
- **Author-reported:** supplied by the author but not independently visible.
- **Inferred:** plausible interpretation that cannot be published as fact without confirmation.
- **Unknown:** motivation, ownership, decisions, feedback, outcomes, or lessons that require an answer.

Never use repository complexity, code volume, generated UI, or automated tests as proof of user value.

### 2. Diagnose the story

Select the format that best matches what the evidence can prove:

- **Product Utility:** a focused product solving a concrete problem.
- **Product Experiment:** a consequential decision tested under real constraints.
- **Workflow / System:** repeated friction turned into a reusable capability.
- **Practice Note:** one useful constraint, failure, comparison, or build lesson without enough evidence for a full case.

State the recommendation, confidence, alternative, evidence gaps, and one-sentence Story Thesis before drafting.

### 3. Let the user choose article length

Present Compact, Standard, and Expanded with a one-line recommendation based on story complexity and evidence depth. Draft only after the user chooses or explicitly delegates the choice.

If the evidence cannot sustain the chosen length, explain the mismatch and recommend a shorter mode or Practice Note. Never pad the article with generic process prose.

### 4. Ask the minimum context interview

Ask only questions the evidence map cannot answer. Prioritize questions that unlock:

- the concrete trigger;
- the decision that changed the experience;
- a failure, pivot, or version change and what caused it;
- actual use, return behavior, adoption, or influence;
- ownership across designer, AI, engineering, and collaborators;
- a visual or anonymizable receipt.

### 5. Check AI-building craft

When AI or code materially shaped the project, look for evidence of:

- capability gained;
- a changed working method with the agent;
- tool judgment across code, AI, Figma, and manual work;
- technical understanding needed to direct the build;
- the human-AI decision boundary;
- a reusable principle or working pattern.

Prefer this causal sequence:

`Encountered constraint -> changed how I worked with the agent -> achieved a better result -> extracted a transferable principle`

Treat that sequence as publishable only when the source establishes all four links: the initial output or behavior, the concrete mismatch, the author's intervention, and the changed result. A general statement such as "I corrected the output" does not establish the failure mechanism, division of labor, or reusable lesson. Do not supply those details from a source pattern.

Do not turn the case into a tool diary. Name a specific tool only when its capability or limitation affected a decision. If any link in the episode is missing, flag the exact gap and keep the unsupported mechanism or lesson out of the article.

### 6. Retrieve and adapt source patterns

After the evidence map and archetype are stable, retrieve one to three relevant pattern cards from the source library. For each pattern:

1. explain why it matches this project's evidence or open question;
2. generate a project-specific candidate statement;
3. classify the statement as **Observed**, **Author-reported**, **Hypothesis**, or **Unsupported**;
4. keep the source pattern's facts separate from the current project's facts.

An Observed statement may be published directly. An Author-reported statement may be published with careful attribution and a requested receipt. A Hypothesis may appear only as a next signal, success criterion, or question. Exclude Unsupported statements.

Source patterns should improve the question, causal sequence, or strength of a statement. Do not copy their wording or import another project's outcome.

### 7. Build the outline and proof plan

Use the selected archetype for the narrative spine and the selected length mode for compression. Section names should reflect the project's actual progression rather than fixed Research / Ideation / Design labels.

Select a **set of proof statements**: the distinct evidence-backed impact, adoption, influence, insight, or constraint that makes each consequential turn in the story legible. Write each as a short narrative statement, not a metric card. Each should connect what happened to why it matters, with one brief phrase emphasized inline.

Render each accepted statement as a visually isolated Markdown blockquote without a visible type label. Specify its statement, inline emphasis, evidence status, evidence IDs, placement, and originating source pattern in production notes. Use the selected length mode to decide quantity. A callout must earn its own place in the narrative: separate callouts with intervening story or a visual, and do not turn every fact into a callout.

Keep `At a Glance` neutral when used. Do not render its facts as colored cards or stacked blockquotes. It orients the reader; evidence callouts carry the visual emphasis.

Only **Observed** and **Author-reported** statements qualify for the proof treatment. A Hypothesis may appear as a next signal or success criterion in ordinary prose or production notes, but never as a visually highlighted proof statement.

Do not generate replacement product UI to fill a missing receipt. Ask the author for a specific capture or provide a clearly labeled reconstruction plan.

### 8. Draft causally

Prefer concrete progression:

`I built X -> people used it -> they asked for Y -> I changed Z`

Avoid strategic summaries until the preceding event earns them. Prefer concrete implementation or workflow changes over generalized system language. Use first person to make ownership legible.

Treat Output, Outcome, Adoption, and Influence as an internal analysis hierarchy. Do not require those labels in the public article.

Use concise conclusions. A crafted or symmetrical ending is appropriate only when the body has earned it through visible evidence.

### 9. Run evidence and editorial QA

Confirm that:

- every paragraph adds a fact, decision, result, or lesson;
- every proof statement has a nearby receipt or attribution;
- every proof statement carries an evidence status in production notes;
- `At a Glance`, when present, remains visually neutral;
- every public proof statement has no visible category label and emphasizes only one short phrase;
- hypothetical statements appear only as questions, next signals, or success criteria;
- output, outcome, adoption, and influence are not conflated;
- facilitated trials are not described as self-serve adoption;
- potential, interest, trial, reuse, contribution, and second-order adoption remain distinct;
- AI activity demonstrates judgment or changing capability rather than tool usage alone;
- the article stays inside the selected word range, including headings, captions, and proof-statement copy;
- missing evidence remains in companion notes rather than public prose.

## Pre-draft output

Return this decision package before writing the article:

```text
Recommended archetype:
Confidence:
Story thesis:
Length options:
Recommended length:
Observed evidence:
Author-reported evidence:
Missing evidence:
Relevant source patterns:
Adapted candidate statements:
Candidate status:
Proof-statement specifications:
Visual receipts required:
Claims to avoid or qualify:
```

After the user confirms the direction, create:

1. the public case-study draft;
2. separate production notes containing evidence gaps, capture requests, confidentiality guidance, and claim verification.
