---
name: vibe-case-study
description: Write or revise a portfolio case-study story for a vibe-coded or AI-built product project using repository evidence and author context. Use this skill only when the user explicitly asks to create, draft, outline, structure, or rewrite that project's case-study story. Do not trigger for general repository inspection, product critique, coding help, documentation, claim review, or case studies unrelated to vibe-coded product projects.
---

# Vibe Case Study

Write the shortest credible case study that explains what was built, the product judgment behind it, and what happened.

Use one shared reading model:

`Fixed bookends + flexible middle + lightweight evidence discipline`

Do not classify the project into an archetype. Do not retrofit a generic UX process. Let the project's actual decisions determine the middle.

Default to the user's language. If no preference is available, use the language of the supplied material.

## When to use this skill

Use this skill only when both conditions are true:

1. The subject is a vibe-coded or AI-built product project.
2. The user explicitly wants to create or revise its portfolio case-study story, outline, structure, or narrative.

Do not use this skill for:

- general repository inspection or explanation;
- product or UX critique without a case-study-writing request;
- coding, debugging, or implementation work;
- README, documentation, recap, or PRD writing;
- checking an isolated claim without developing a case-study story;
- case-study work for projects that were not vibe-coded or AI-built.

If the request does not satisfy both conditions, do not apply this workflow.

## Core editorial rule

Every section should advance one meaningful claim about the project. Visuals and evidence should support that claim.

A meaningful claim tells the reader at least one of these:

- what the product does;
- why it exists;
- what the author decided and why;
- what constraint changed the experience;
- what changed during iteration;
- what result, response, or lesson followed.

If a section can be removed without weakening the story, remove it or merge it.

## Evidence discipline

Keep evidence handling practical:

1. Treat facts directly visible in the repository or supplied artifacts as verified.
2. Treat user-provided context as author-reported context.
3. Never infer motivations, decisions, feedback, adoption, or impact from code alone.
4. Ask the user when a missing fact materially changes the story.
5. Do not describe interest, reactions, a prototype, or successful implementation as adoption or product impact.
6. Do not manufacture research, testing, metrics, outcomes, quotes, or decisions to make the case feel complete.

Internal labels such as `verified`, `author-reported`, and `unconfirmed` may help reasoning, but do not turn them into a required workflow or public output.

Evidence can remain flexible while drafting:

- infer possible missing context for brainstorming, clearly labeled as a possibility;
- use placeholders such as `[confirm whether this changed after user feedback]`;
- propose a stronger claim the author could make if they can verify it;
- recommend a screenshot, commit, message, analytics signal, or other receipt that would support a claim;
- narrow a claim to what the current source actually proves.

Never present provisional material as fact. Never cite a source that does not materially support the adjacent claim.

## Four-step workflow

### Step 1 — Understand the project

Inspect the repository and supplied context before outlining or drafting.

Use the smallest set of inspections that can establish:

- what the product does;
- its major features and user flows;
- product architecture when it affects the experience or story;
- visible iterations or version changes;
- implementation constraints that affected the experience;
- useful README or documentation context;
- relevant commit history when it adds evidence of a meaningful change.

Inspect working product states or supplied artifacts when available. Distinguish current behavior from plans, stubs, and documentation claims.

Do not treat lines of code, file count, repository complexity, tests, or generated UI as evidence of product value. Tests may verify behavior; they do not prove usefulness, adoption, or impact.

After inspection, identify only the missing human context that materially affects the story. Useful questions include:

- What triggered the project?
- Who was it initially for?
- What existing approach was unsatisfactory?
- What was the most consequential product or design decision?
- What changed during iteration, and why?
- Did anyone actually use it? What happened?
- What did AI produce, and what did you personally decide or correct?
- What result or evidence can be shown publicly?

Do not ask all of these by default. Ask the smallest number needed, combine related questions, and do not ask for facts the repository already establishes.

### Step 2 — Find the story

Write a one-sentence **Story Thesis** before drafting. It should explain:

- what was built;
- the meaningful problem or opportunity;
- the most significant decision, approach, or insight;
- why the project is worth reading.

Do not force a sentence formula. The thesis is an editorial tool and does not need to appear in the published case.

Then identify the smallest set of ideas needed to prove the thesis. Prefer causal relationships over process inventory:

`trigger -> decision -> changed product or behavior -> result or bounded lesson`

Look for a supported building takeaway using the guidance below: what would this decision change about how the author approaches a similar build? Do not force one when only the product behavior is known.

Do not add Research, Personas, Journey Map, Ideation, or Usability Testing sections unless those activities genuinely happened and are important to the argument.

### Step 3 — Choose depth

Use the shortest depth that communicates all consequential ideas without removing important causality.

#### Short

Use when the project has one main idea or one meaningful decision.

- Keep the middle to one compact module.
- Merge context and approach where that reads naturally.
- Avoid standalone process sections.

#### Standard

Use by default when the project contains several meaningful product or build decisions.

- Preserve the shared spine.
- Use roughly two to four middle modules.
- Give each module a distinct narrative job.

#### Deep

Use only when multiple meaningful stages, pivots, or an earned reusable insight require extended explanation. A concise building takeaway can belong in Short or Standard; its presence alone does not justify Deep.

- Expand the middle around those stages.
- Add a turning point, build method, or reusable principle only when evidence supports it.
- Do not use depth to compensate for missing outcomes or weak decisions.

Depth changes the flexible middle, not the overall case-study skeleton. Do not enforce word-count ranges.

### Step 4 — Outline or draft

Use this shared outer structure:

1. **Hero** — name the product, what it enables, and the clearest reason to care. Keep it concise. In a full article draft, follow the Hero with its primary media marker and any useful resource cards.
2. **At a Glance** — always use exactly three entries in this order: **What**, **How**, **Why it matters**. What names the product and who it serves; How explains its core workflow or mechanism in plain language; Why it matters connects that behavior to the user's problem or a supported outcome. Keep each entry concise and evidence-grounded. Do not substitute or append role, stack, timeframe, or status fields; include those elsewhere only when they advance the story.
3. **Context** — explain the trigger, prior friction, opportunity, and relevant constraints.
4. **Flexible Middle** — use project-specific sections that prove the Story Thesis.
5. **Outcome** — state what happened, what remains unproven, and any lesson the events actually earned.
6. **Resources** — include links, demos, repositories, or related artifacts only when useful and publishable.

Possible middle modules include:

- Approach
- What I Built
- Key Product Decision
- Core Interaction
- Scope Decision
- Technical Constraint
- Iteration / Turning Point
- How I Built It
- AI Collaboration
- Reusable Insight / Principle

These are options, not a checklist. Rename them to describe the actual claim. Select only modules that materially advance the story.

## Content display markers

Use these Markdown markers only in full article drafts and full-draft revisions. Do not emit them in a pre-draft package or outline.

### Media

Add one primary media recommendation immediately after the Hero by default:

```text
[media]
placement: hero-end
suggestion: [what the asset should show]
```

Suggest inline media only when it materially explains a nearby interaction, comparison, iteration, workflow, technical constraint, or product output. State what the asset should show. Do not add media merely to break up text.

### Resource

When a useful, publishable project URL is supplied or established by the repository, place a resource card immediately after Hero Media:

```text
[resource]
title: [action-oriented link title]
description: [what the reader will find]
url: https://example.com
```

Use exactly one URL per card. Use separate adjacent cards for multiple related resources. If a useful resource clearly exists but its URL is unavailable, complete the article without a resource marker and ask for the URL afterward. Do not insert a URL placeholder. Do not ask about resources when none are clearly relevant.

### Highlight

Do not generate a highlight in a first draft. Highlighting is deliberate editorial emphasis, controlled by the user.

On an explicit request to add, replace, or remove a highlight, use or edit only this marker:

```text
[highlight]
content: [the existing approved sentence or paragraph]
```

Preserve the original factual meaning. Avoid adjacent or excessive highlights. Removing a highlight returns its unchanged content to normal Markdown prose.

These markers are semantic content for later portfolio rendering. Do not specify their web styling, typography, spacing, responsive behavior, or component implementation.

## AI collaboration is optional

Include AI-building process only when AI materially affected a product decision, constraint, iteration, or working method.

Do not add an AI section merely because the project was vibe-coded. Do not turn the article into a prompt diary, tool list, conversation chronology, or speed-of-generation showcase. Name a tool only when its capability or limitation affected the result.

A strong AI-related episode often follows:

`initial approach -> limitation or mismatch -> author's intervention -> changed result -> transferable lesson`

This is one possible pattern, not a required failure story. Specification choices, task boundaries, evaluation criteria, and workflow design can also earn a building lesson without a failed AI output.

Include only the links the project supports. If the intervention is known but the mechanism or changed result is not, ask for it or keep the wording narrow.

Make ownership legible: distinguish what AI generated from what the author framed, evaluated, corrected, rejected, or decided.

## Derive a reusable building takeaway

When supported, go one level beyond the outcome (what happened) or product lesson (what the experience needed). Extract a building principle: what should someone do differently when specifying, building, evaluating, or collaborating with AI on a similar project, and why?

Use this as an internal reasoning aid, not a published formula:

`concrete decision -> underlying constraint -> repeatable working practice -> limit of applicability`

Ground the takeaway in a consequential constraint, boundary, or intervention already established in the story. Connect it to an actionable working practice, not a feature summary, AI-role disclosure, or generic advice such as "be clear with AI." Derive the practice from this project's evidence; do not reuse the same automation-versus-human-judgment lesson across unrelated projects.

Product behavior alone does not establish how the author prompted AI, what was hardest, or what changed their working method. Use author context or documented process for those claims. If that bridge is missing, retain the narrower product lesson, offer a clearly provisional interpretation, or ask one targeted question. Do not invent a failed attempt, a before/after comparison, or demonstrated reuse to make a lesson feel earned. A transferable principle is not evidence that a framework, skill, or playbook was built or adopted.

Prefer one concise takeaway integrated near the decision that earns it or in the closing reflection. Replace a redundant summary where possible. Do not require a separate AI-lessons section, named framework, new artifact, or extra depth. Preserve concrete outcomes rather than replacing them with reflection.

## Concise pre-draft output

Before writing the article, return:

```text
Story Thesis:
Recommended depth:
What the repository establishes:
Missing context:
Proposed structure:
Evidence or visuals worth showing:
Claims to avoid or qualify:
```

Keep this package concise. Omit empty categories. Do not include an archetype, confidence score, candidate-statement taxonomy, proof specification, or source-pattern ID.

If the user directly requests a draft and the evidence is sufficient, the pre-draft package can be brief and followed by the draft in the same response. If a consequential fact is missing, ask for it before presenting a factual final draft; offer provisional wording or placeholders when that would still help.

## Drafting guidance

- Lead with product behavior and consequential decisions, not implementation chronology.
- Use concrete actions and first person where it clarifies ownership.
- Connect iteration to its cause; do not merely list versions.
- Keep `At a Glance` factual and compact.
- Place a visual near the claim it helps the reader understand.
- Prefer real product states, before/after comparisons, decision artifacts, outputs, or credible usage receipts over decorative imagery.
- In full drafts, use the display-marker rules above; keep pre-drafts and outlines as ordinary Markdown.
- Do not generate replacement product UI and present it as evidence. Label reconstructions clearly.
- State outcomes at the level the evidence supports: built, tested, used, reused, requested, adopted, or measured are different claims.
- Separate facilitated use from self-serve adoption and interest from behavior.
- End with a bounded result or lesson. Do not manufacture a grand conclusion.

## QA

Before returning an outline or draft, check:

- Does every section contribute a meaningful fact, decision, result, or lesson?
- Does the article follow the actual project rather than a generic UX process?
- Does At a Glance contain exactly What, How, and Why it matters, in that order, with no unsupported impact claims?
- Are product judgment and author ownership clear?
- Are unsupported claims removed, narrowed, qualified, or marked for confirmation?
- Is AI-building content included only when it materially affects the story?
- If a building takeaway is included, does it tell a reader what to do differently in a similar build and why, beyond summarizing the product or AI's role?
- Can the takeaway be traced to this project's evidence and author context, without inventing a working method, personal learning, or demonstrated reuse? If not, narrow it or ask for the missing context.
- In a full draft, does Hero Media follow the Hero, and does each resource card contain one useful URL?
- Are inline media markers attached to claims they materially explain, rather than decorative breaks?
- Are highlights present only because the user explicitly requested them, with their factual meaning unchanged?
- Could any section be removed without damaging the story? If yes, remove or merge it.
- Is the selected depth the shortest one that still works?

Do not use a scoring rubric.

## Optional inspiration

The skill is complete without external references. When the user asks about Meng Xie's approach, wants comparative editorial inspiration, or would benefit from examples of variable depth within a consistent reading model, consult [Meng Xie research notes](references/meng-xie.md). Use them as inspiration only; never import another project's facts, claims, headings, or voice.
