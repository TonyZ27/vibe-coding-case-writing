# Meng Xie AI-Native Case Study Pattern Matrix

> Research snapshot: 2026-08-24  
> Corpus: The 17 project pages currently listed on the [Meng Xie AI-Native Design Portfolio](https://mengxie.me/).  
> Purpose: Extract a reusable narrative system and validate story archetypes for a Repo-to-Case-Study Agent. This is not an attempt to imitate the author's voice or independently verify internal business data.

## Executive conclusion

The three candidate archetypes are valid, but they should not be treated as three fixed page layouts:

| Repo-led archetype | Count | What it primarily proves | Representative cases |
| --- | ---: | --- | --- |
| **Product Utility** | 4 | Finding a specific problem, controlling scope, and shipping a useful tool quickly | Little Color World, Passport Photo Generator, Parental Leave Calculator, Bloom |
| **Product Experiment** | 3 | Making a consequential product decision under real constraints and testing it through an experience people can use | Group Order, Production Codebase Prototyping, Status Scheduling |
| **Workflow / System** | 7 | Turning repeated friction into a reusable workflow, skill, tool, or learning system | Production Audit, Learning Hub, Vibe Designing, Playbook, Dogfooding, Figma SoTs, Deck Creation |

The remaining three pages establish necessary exit routes:

- **Practice Note (2):** Human–AI Collaborative Design and Pencil.dev Evaluation. These are better suited to a method, failure, or tool judgment than a full product case study.
- **Portfolio Thesis (1):** The AI Product Studio detail page synthesizes capabilities across multiple projects. It cannot be generated responsibly from a single repository.

The future Agent should therefore not force every repository into one of three templates. It should:

> Determine what the project is best positioned to prove, then decide whether the available evidence can support a case study. If not, recommend a Practice Note.

## Research boundaries and evidence policy

- The homepage currently lists **17 AI Projects Shipped**; this matrix covers all 17.
- Sixteen detail pages were directly readable. The `Subs Dogfooding for All Employees` detail page failed during direct retrieval, but its full body was available through the search index, so its source status is noted separately.
- Usage numbers, internal feedback, organizational impact, and commercial figures are author-reported. This study analyzes how those claims are structured; it does not treat them as independently verified facts.
- `AI Product Studio` contains a public-content conflict: the homepage card describes an AI product-photography concept for WhatsApp businesses, while the current detail page is a cross-project Full-Stack Designer vision. The matrix classifies the structure of the detail page and preserves the conflict as a warning.

### Evidence-strength definitions

These ratings describe whether a page gives the reader enough receipts. They are not judgments about whether a project is real.

- **Strong:** A concrete artifact, a decision or version change, and outcome or adoption evidence form a credible loop.
- **Medium:** The artifact and point of view are clear, but outcomes rely mainly on reactions, self-reporting, or incomplete process evidence.
- **Weak:** The page is dominated by vision or value statements, making project evolution difficult to assess.
- **N/A:** The page is not a single-project case study.

## 17-project Pattern Matrix

| # | Project | Page type / best-fit archetype | Story thesis | How the middle unfolds | Strongest proof presented | Visual-evidence pattern | Evidence strength |
| ---: | --- | --- | --- | --- | --- | --- | --- |
| 1 | [AI-Powered Group Order for WhatsApp](https://mengxie.me/projects/group-buy.html) | Product Experiment | AI creates value by removing input friction from an established group-ordering behavior, not by inventing a new behavior | Cultural behavior → two-sided product bet → consumer/business scope → community response → principle | Top 10 / 200+, leadership presentation, two-sided business model | Photo/link input → AI item list → group order; consumer and business sides shown together | Medium |
| 2 | [WhatsApp Production Audit Platform](https://mengxie.me/projects/vibe-coding-beyond-diffs.html) | Workflow / System | A design deliverable can be a tool the team uses directly, not only a mock or specification | Deliverable gap → self-serve audit platform → build approach → cross-team sharing → redefined deliverable | Working internal tool, shared by design and engineering, cross-posted across groups | Old workflow friction → self-serve browsing UI → audit output; real tool screenshots | Medium |
| 3 | [Little Color World](https://mengxie.me/projects/little-color-world.html) | Product Utility | A highly specific personal situation can force product scope and interaction design to become unusually clear | Sixteen-hour flight → toddler constraints → product choices → observed use → creative point of view | Zero-install live site, real use by a child, explicit no-reading and large-target constraints | 8–12 second tap-to-color demo; annotations for large targets and no-failure states | Medium |
| 4 | [Passport Photo Generator](https://mengxie.me/projects/passport-photo.html) | Product Utility | A simple but sharply focused tool can be more valuable than bloated or expensive alternatives | Parent pain → minimum product → feature scope → user quote → community response | Working tool, specific user quote, 18 reactions / 2 shares | Upload → adjust → download sequence; result sample; user-feedback receipt | Medium |
| 5 | [Human–AI Collaborative Design](https://mengxie.me/projects/human-ai-collaborative-design.html) | Practice Note | The most effective AI workflow is not full automation; it is knowing when to return precision work to human judgment | Hard limit → pure-AI failure → four-tool handoff → quantified result → method tips | 18K → 8K, pipeline passed, two paths resolved manually | Before/after numbers; AI/manual handoff flow; failed-output comparison | Strong |
| 6 | [Parental Leave Calculator](https://mengxie.me/projects/leave-calculator.html) | Product Utility | The best vibe-coded utilities often address problems that are specific, rules-heavy, and emotionally costly | Rules-heavy pain → v1 → community feedback → v2 → use and distribution → belief | v1/v2 differences, feedback-led features, four-group distribution, user quote | Rules input → calendar output; v1/v2 comparison; feedback-to-change mapping | Strong |
| 7 | [Pencil.dev Evaluation](https://mengxie.me/projects/pencil-dev.html) | Practice Note | A useful tool evaluation explains which problem a tool fits, rather than declaring a universal winner | Market context → three-tool positioning → distinctive capabilities → team-decision impact → evaluation principle | Figma Make / Pencil / Cursor comparison, triggered TPA request | Three-tool spectrum; capability/use-case matrix; real trial screenshots | Medium |
| 8 | [AI Design Learning Hub](https://mengxie.me/projects/learning-hub.html) | Workflow / System | Information architecture is design: reducing discovery cost is what turns AI FOMO into action | Information overload → three-pillar system → design intent → value propositions → lessons | Three-pillar IA and roughly one-hour learning units; limited concrete adoption evidence | Content-noise before state → three-pillar hub; learning path and real pages | Weak–Medium |
| 9 | [Production Codebase Prototyping](https://mengxie.me/projects/production-codebase-prototyping.html) | Product Experiment | Production prototypes reveal constraints that static mocks cannot expose | High-risk surface → five directions → fidelity framework → build/device experience → lessons → organizational response | Five directions, debug APK, 2.5K lines, physical-device experience, VP newsletter | Five-direction overview; physical-device demo; fidelity spectrum; edge-case receipts | Strong |
| 10 | [Vibe Designing](https://mengxie.me/projects/vibe-designing.html) | Workflow / System | Design judgment can be encoded as a shared capability that narrows the gap between “works” and “feels right” | Capability gap → Double Diamond mapping → two skills → input/output → scaling claim | Two installable skills, ten lenses, explicit output formats | Framework map; input → output for each skill; real diagnosis sample | Medium |
| 11 | [AI-Native Prototyping Playbook](https://mengxie.me/projects/playbook.html) | Workflow / System | Documentation should change how people think, not merely list procedures | Scattered knowledge → progressive architecture → teaching design → impact → co-creator feedback | 20-page playbook, 11 reactions, 10 comments, 2 shares, co-creator quote | Four-stage learning path; forkable example; co-creation receipt | Strong |
| 12 | [Bloom Parenting Resource Hub](https://mengxie.me/projects/bloom.html) | Product Utility (community-build variation) | Vibe coding's larger value is not individual productivity but a lower barrier to collective product creation | Fragmented information → product scope → bilingual/UGC system → contributor model → community thesis | Live demo, 5+ contributors, explicit feature ownership, EN/CN | Product overview; contributor-to-feature map; contribution-to-discovery demo | Strong |
| 13 | [AI Product Studio](https://mengxie.me/projects/ai-product-studio.html) | Portfolio Thesis | Multiple projects accumulate into a capability model for the “full-stack designer” | Vision → full-stack definition → five-layer capability stack → future directions | Cross-project synthesis across 11 projects; no single-project process on the current page | Capability stack, project timeline, cross-case evidence index | N/A |
| 14 | [Subs Dogfooding for All Employees](https://mengxie.me/projects/subs-dogfooding-prototypes.html) | Workflow / System | Prototype builds are one-time artifacts; the transferable value is a repeatable way to audit gated features | Four access gates → dual-platform builds → internal validation → four-step workflow → distribution trade-offs → adoption | iOS + Android, Days → Mins, one AB prop, four-channel trade-off, cross-team reference | Gate map; four-step audit flow; distribution decision matrix; install-to-audit demo | Strong |
| 15 | [AI-Native Figma SoTs](https://mengxie.me/projects/figma-sot.html) | Workflow / System | Once a workflow becomes a skill, adoption no longer depends on its creator | Two repeated pains → reverse handoff → two workflows → outputs → skill packaging → community pull | Editable DS frames, logic-rich flowchart, Hrs → Mins, 21 reactions / 23 comments | Production + code → editable Figma; real frame/flowchart; community receipt | Strong |
| 16 | [AI-Native Deck Creation](https://mengxie.me/projects/ai-native-deck-creation.html) | Workflow / System (with Practice Note traits) | Tools are the final 20%; content judgment and a transferable workflow drive deck quality | Tool landscape → content thesis → tool change → four-step workflow → honest trade-offs → second-order adoption | 5+ approaches compared, explicit unsuitable use cases, attendee becoming a teacher | Tool decision matrix; four-step workflow; finished output; second-order adoption receipt | Strong |
| 17 | [Status Scheduling Subscriber UX](https://mengxie.me/projects/status-scheduling.html) | Product Experiment (with a system spin-off) | A 0→1 product project can solve a user-trust problem while exposing and fixing an organizational review bottleneck | Two user journeys → core interaction decisions → AI's BR role → review bottleneck → assistant → outcomes | iOS + Android flows, explicit rationale, 90/10 deck, org-wide assistant | Cross-platform walkthrough; annotated key interaction; BR input chain; assistant demo | Strong |

## Why the three archetypes hold

### A. Product Utility

**Recognition signals**

- The project begins with a specific person, situation, or recurring frustration rather than a broad market proposition.
- The product scope can be explained in three to six capabilities.
- The most convincing result is often that someone used, shared, or requested changes to the product—not necessarily a business KPI.

**Stable narrative spine**

`Specific situation → Friction → Minimum useful product → Real use / feedback → Iteration → Product belief`

**Minimum evidence threshold**

- A working state or complete task demo.
- A product judgment explaining why the scope was deliberately constrained.
- At least one receipt for real use, feedback, or a version change.

**Do not force**

- Do not retrofit personas, journey maps, or a large research phase.
- Do not present reaction counts as user outcomes.
- When commercial metrics do not exist, report task completion, repeat use, or evidence that use triggered iteration.

### B. Product Experiment

**Recognition signals**

- The project contains a new product bet, consequential interaction, or high-fidelity validation question.
- The repository or design files expose alternatives, real states, platform constraints, or selection history.
- The case is not primarily about making a product; it is about why one direction deserved to be chosen.

**Stable narrative spine**

`Product bet → Constraint → Competing directions → Key decision → Real-state validation → Outcome / framework`

**Minimum evidence threshold**

- A clearly stated hypothesis or design question.
- At least one consequential decision shaped by a constraint.
- Real-state evidence of the final experience.
- If the case claims iteration, it must show what changed and what evidence triggered the change.

**Do not force**

- Do not use lines of code as a substitute for design quality.
- Do not show multiple directions without explaining what was decided.
- Include AI-tool activity only when it reveals judgment, constraint, or correction.

### C. Workflow / System

**Recognition signals**

- The project begins with repeated team or organizational friction.
- The output includes repeatable steps, a skill, a tool, or a framework—not only a one-time artifact.
- Its value must be demonstrated by whether someone else can use it independently.

**Stable narrative spine**

`Repeated friction → Workflow model → Build / encode → Real output → Packaging → Adoption → Transferable pattern`

**Minimum evidence threshold**

- A before workflow with specific friction points.
- An executable workflow or system structure.
- At least one real output.
- One adoption receipt beyond the author.

**Do not force**

- “Reusable” cannot rely on the author's assertion alone. If nobody else has used it, describe it as a proposed system.
- Reactions to a launch post are not the same as workflow adoption.
- A tool list cannot replace the actors, inputs, decisions, and outputs inside a workflow.

## Two non-template formats

### Practice Note

Recommend a short Practice Note when the repository only supports a one-off solution, tool evaluation, or hybrid working method:

`Constraint / question → What failed → What worked → Evidence → Reusable lesson`

This is not a fourth case-study template. It is a fallback that prevents evidence inflation.

### Portfolio Thesis

Use a Portfolio Thesis only after several cases exist, to synthesize capabilities, methods, and direction across projects:

`Repeated project pattern → Capability model → Cross-case evidence → Point of view → Next frontier`

A single repository must not enter this route.

## Meng's fixed shell and variable middle

### Fixed shell

Nearly every complete detail page uses:

1. **Chapter / date / category:** Places the project inside a longer growth narrative.
2. **Hero claim:** Uses one or two sentences to state the artifact, key difference, and significance.
3. **Proof strip:** Presents three or four numbers, states, or adoption signals.
4. **At a Glance:** Consistently answers What / How / Why it matters.
5. **Context:** Establishes the specific friction, constraint, or opportunity.
6. **Project-specific middle:** Follows the available project evidence instead of a fixed process.
7. **Outcome / response / lesson:** Turns the local result into a transferable judgment.

`At a Glance` is the most reusable element because it forces a distinction between:

- **What:** The artifact that was delivered.
- **How:** The capability or working method used.
- **Why it matters:** What the project proves.

### Variable middle

| Available project evidence | Suitable middle module |
| --- | --- |
| v1/v2 or feedback-driven iteration | Version comparison + feedback source |
| Multiple design directions | Alternatives + constraint + decision |
| Reusable workflow | Before flow + workflow steps + generated output |
| Tool evaluation | Landscape + trade-offs + recommendation |
| Community co-creation | Contribution model + ownership + governance |
| Organizational adoption | Packaging + distribution + adoption receipts |
| One failure or hard constraint | Failure → handoff → result → lesson |

Future templates should fix the questions the reader must be able to answer, not the section names.

## Voice profile: patterns worth borrowing

### 1. Lead with the judgment, then explain the mechanism

The opening is not “I used Claude / Figma Make.” It states what changed and why it matters. Tools usually appear in `How` or in the build section.

### 2. Use short sentences and one idea per paragraph

A common rhythm is: one clear judgment → concrete examples or bullets → one broader conclusion. This makes the pages easy to scan and keeps technical content from overwhelming the narrative.

### 3. Use headings as claims or tasks, not generic process labels

Beyond `At a Glance` and `Context`, middle-section headings are project-specific: `The Spectrum of Design Fidelity`, `The Post-Scheduling Flow`, `Spotting the Bottleneck`, and `The Adoption Loop`. This exposes the character of the project more effectively than mechanically applying Research / Ideation / Design.

### 4. Use first person to mark ownership

`I built / I identified / I distilled / I shared` marks individual contribution. Co-created work switches to `we` and names contributors. The future Agent must confirm ownership from the repository and interview rather than infer it from tone.

### 5. Include technical detail only when it proves a constraint

Details such as an AB prop, Buck `select()`, real Android code, or an 800-character limit are used to prove a safety boundary, complexity, or design decision—not to display a technology stack.

### 6. End by turning the artifact into a belief

Typical transformations include:

- A parenting tool → specific problems are often the best targets for fast building.
- A production prototype → different fidelity levels answer different design questions.
- A workflow → packaging it as a skill separates adoption from the creator.
- A teaching session → second-order adoption begins when learners teach others.

### 7. Combine quantitative and qualitative evidence

The proof strip supplies numbers, while the body adds user quotes, physical-device experience, version changes, or organizational adoption. Reaction counts are weak in isolation; they become useful only when paired with concrete behavior.

## Patterns not to copy

Meng's cases provide strong structural references, but the future skill must be stricter than the source material:

1. **Do not upgrade self-reported impact into a verified result.** “Shared org-wide” and “repeatedly used by teams” are different evidence levels.
2. **Reconcile metric conflicts.** The homepage described Leave Calculator as used by hundreds, while the detail page said dozens. The Agent must ask or use the more conservative wording.
3. **Do not treat reactions as outcomes.** They can indicate interest, but not task improvement.
4. **Separate potential from actual results.** `$3.1B market opportunity` and `200M+ potential users` describe market scope, not project impact.
5. **Do not copy duplicate or loose sections.** The Production Codebase page repeats `Community Response`; template QA should consolidate repetition.
6. **Do not inherit grand claims automatically.** Terms such as “production-grade,” “org-wide,” and “first” require repository evidence, release history, or user confirmation.
7. **Use an evidence map when summaries and detail pages conflict.** The public `AI Product Studio` mismatch shows why the Agent cannot start writing after reading only a README or project summary.

## Visual Evidence Plan: images are receipts, not decoration

### General claim → evidence mapping

| Story claim | Preferred visual evidence | Fallback when evidence is missing |
| --- | --- | --- |
| The old process was cumbersome | Before workflow, old UI, or screenshots of actual steps | Use a verifiable text-based flow and label it reconstructed |
| One interaction reduced several steps | 8–12 second end-to-end demo | Use a three-frame input → state → output sequence |
| Real constraints shaped the solution | Physical device, error state, performance state, or edge case | Name the source of the constraint; do not generate fictional UI |
| v2 was driven by feedback | v1/v2 comparison plus the original feedback or issue | Without a feedback receipt, say “changed,” not “feedback-led” |
| A workflow is reusable | Workflow diagram plus one real generated output | If nobody else has used it, label it proposed |
| Adoption occurred | Installation, reuse, contribution, re-sharing, or real-use record | Label reactions only as an interest signal |
| AI and designer responsibilities were distinct | Input / AI action / human judgment / output | Confirm ownership in the interview; do not infer motivation from commit authorship |

### Minimum visual package by archetype

**Product Utility**

1. Final product overview.
2. One complete task demo.
3. One annotated scope or interaction decision.
4. If iteration is claimed, a v1/v2 comparison.
5. One real-use or feedback receipt.

**Product Experiment**

1. Product bet / constraint diagram.
2. Comparable views of two to five directions.
3. Selected direction and rationale.
4. Real-state or physical-device demo.
5. Edge-case, review, or decision outcome.

**Workflow / System**

1. Before workflow.
2. New workflow steps and decision points.
3. At least one real input/output pair.
4. A failure, boundary, or trade-off.
5. One receipt for adoption, reuse, or contribution by someone else.

The Agent must not generate product UI to fill evidence gaps. It should instead produce specific capture instructions:

```text
Section: Core interaction
Need: 01-core-demo.mp4
Capture: Complete flow from user input to final result
Length: 8–12 seconds
Must show: Input, processing state, final result
Avoid: Meaningless cursor movement, a full-product tour, unreadably small text
Caption claim: One interaction replaces the previous three-step flow.
```

## Routing rules for the future Repo Agent

### Step 1 — Evidence Map

Separate evidence into three layers before writing prose:

- **Observed:** Facts directly visible in the repository, README, code, routes, assets, commits, issues, or releases.
- **Inferred:** Plausible but unconfirmed users, motivations, decision rationales, or effects.
- **Unknown:** Context, ownership, feedback, outcome, and learning that only the author can provide.

### Step 2 — Story Diagnosis

Output:

```text
Recommended format: Workflow / System
Confidence: High
Primary reason: Repo contains a repeatable audit workflow and packaged command.
Alternative: Product Utility
Why not selected: End-user value is secondary to team reuse.
Evidence gaps: original trigger, who reused it, adoption receipt.
```

### Step 3 — Thesis Gate

Generate and validate the following before drafting:

```text
What I built: ______
What this case proves: ______
Supporting evidence: ______
Contradicting or missing evidence: ______
```

If the thesis is only “I used AI to build X,” it fails the gate.

### Step 4 — Minimum Interview

Quick Mode should ask only three to six high-value questions that the repository cannot answer:

- Why did you start the project? Who had what specific problem?
- Which decision changed the final experience most, and why?
- What failed, was removed, or changed? What evidence triggered that change?
- What did AI execute, and what did you personally judge or correct?
- Who actually used it? Is there a public or anonymizable receipt?
- If the reviewer remembers one learning, what should it be?

### Step 5 — Outline + Visual Evidence Plan

Deliver the outline, claim/evidence mapping, and missing-visual list first. Draft prose only after the author confirms them.

### Step 6 — Draft QA

Check every claim:

- Is this observed, author-reported, or inferred?
- Is proof located near the claim?
- Does the AI activity reveal actual design judgment?
- Has a traditional UX process been retroactively invented?
- Is the outcome a product result, adoption result, interest signal, or potential?
- Does each visual prove a local claim?

## Next-stage recommendation: define Template Contracts before writing a long prompt

The next stage should create three archetype references from this matrix. Each reference should use the same contract:

1. **Use / do-not-use conditions.**
2. **Questions the case must answer.**
3. **Minimum evidence threshold.**
4. **Optional middle modules.**
5. **Story Thesis formula.**
6. **Visual-evidence requirements.**
7. **Claims most likely to be overstated.**
8. **One positive and one negative example.**
9. **Quality rubric.**

Then evaluate the system with four different repositories:

- A small personal utility.
- A product prototype with competing directions.
- An Agent, skill, or internal workflow.
- A weak-evidence repository that should fall back to a Practice Note.

Write the top-level `SKILL.md` only after all four routing behaviors are stable.

## Primary Sources

- [AI-Native Design Portfolio — homepage](https://mengxie.me/)
- [AI-Powered Group Order for WhatsApp](https://mengxie.me/projects/group-buy.html)
- [WhatsApp Production Audit Platform](https://mengxie.me/projects/vibe-coding-beyond-diffs.html)
- [Little Color World](https://mengxie.me/projects/little-color-world.html)
- [Passport Photo Generator](https://mengxie.me/projects/passport-photo.html)
- [Human–AI Collaborative Design](https://mengxie.me/projects/human-ai-collaborative-design.html)
- [Parental Leave Calculator](https://mengxie.me/projects/leave-calculator.html)
- [Pencil.dev Evaluation](https://mengxie.me/projects/pencil-dev.html)
- [AI Design Learning Hub](https://mengxie.me/projects/learning-hub.html)
- [Production Codebase Prototyping](https://mengxie.me/projects/production-codebase-prototyping.html)
- [Vibe Designing](https://mengxie.me/projects/vibe-designing.html)
- [AI-Native Prototyping Playbook](https://mengxie.me/projects/playbook.html)
- [Bloom Parenting Resource Hub](https://mengxie.me/projects/bloom.html)
- [AI Product Studio](https://mengxie.me/projects/ai-product-studio.html)
- [Subs Dogfooding for All Employees](https://mengxie.me/projects/subs-dogfooding-prototypes.html)
- [AI-Native Figma SoTs](https://mengxie.me/projects/figma-sot.html)
- [AI-Native Deck Creation](https://mengxie.me/projects/ai-native-deck-creation.html)
- [Status Scheduling Subscriber UX](https://mengxie.me/projects/status-scheduling.html)
- [2026 presentation — cross-project narrative](https://mengxie.me/presentation/index.html)
