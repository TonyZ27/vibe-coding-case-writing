# Case-study diagnosis

**Recommended format:** Practice Note fallback, not a full case study  
**Confidence:** High  
**Recommended archetype:** None yet. Practice Note is a fallback format, not a fourth archetype.  
**Alternative:** Product Utility, but only if the script becomes a working, intentionally scoped tool and gains a concrete product decision plus a real-use receipt.  
**Selected variant:** Build lesson, provisionally. This variant is only viable if one specific failure, change, or implementation insight can be demonstrated.

## Why a full case study is not supported

The available evidence describes an unfinished command-line script used twice by its creator. Those two runs are personal use, not adoption. There are no external users, feedback-led changes, packaged release, considered alternatives, or documented product decision. That leaves no defensible causal arc from problem to decision to validated outcome, and no basis for presenting the script as a reusable workflow or product success.

A Practice Note is the strongest honest direction, but it is not ready to draft yet. Even that shorter format needs one concrete trigger, an inspectable contrast, and a lesson that came from a choice the author actually made. If no such episode exists, keep this as private project documentation rather than publishing a generic reflection.

## Provisional story thesis

> An unfinished screenshot-renaming script can document an emerging personal workflow, but two creator-run uses prove only that the script was tried—not that it is reliable, reusable, or valuable to others.

This is a framing boundary, not yet a publishable thesis. A final thesis must name the specific naming problem, what failed or changed, and the bounded lesson supported by that event.

## Length options

- **Compact — 400–500 words:** Recommended if a concrete build lesson and one before/after receipt can be supplied. It is the shortest mode that can carry a trigger, change, evidence, and limitation without padding.

- **Standard — 500–600 words:** Suitable only if there are two or three consequential decisions or visible iterations with receipts. The current evidence does not support it.

- **Expanded — 700–800 words:** Worthwhile only for a multi-phase project with alternatives, validation, adoption, and several strong visuals. The current project does not support it.

**Recommended length:** Compact Practice Note, pending your choice. No draft should be written until you select a length or explicitly delegate that choice.

## Evidence map

### Observed evidence

- None independently inspected or supplied as a repository artifact in this request.

### Author-reported evidence

- The artifact is an unfinished command-line script.
- It renames exported screenshots.
- The creator used it twice.
- It has no external users or feedback.
- It has no packaged release.
- No alternatives were evaluated.
- No product decision was documented.

### Inferred — not publishable as fact

- Screenshot renaming was repetitive or costly enough to motivate automation.
- The two runs succeeded or saved time.
- The script improved filename consistency.
- AI materially changed the creator's working method.
- The script could be useful to other designers.

### Missing evidence

- The concrete trigger: what happened during screenshot export that prompted the script.
- A real input/output example from one of the two runs.
- What failed, remained uncertain, or changed during the build.
- The author's actual judgment or lesson from that event.
- The author's role versus any AI tool's role.
- A transfer boundary: when this method is useful and when it is not.
- Basic reliability evidence, such as handling one representative batch correctly.
- External use, feedback, packaging, and distribution evidence needed for a full case study.

## Relevant source patterns

### MX-01 — Personal constraint sharpens scope

**Why it matches:** This is a creator-built utility, so a narrow personal trigger could explain its scope without inventing a market need. The required trigger and working-task receipt are still missing.

**Adapted candidate statement:** “Because [specific screenshot-export situation], I limited the first version to [essential renaming behavior] rather than [unnecessary scope].”  
**Candidate status:** Unsupported until the trigger, scope decision, and real output are confirmed.

### MX-05 — Packaging separates reuse from the creator

**Why it matches:** The absence of packaging is a meaningful boundary. It explains why the project cannot yet be described as a reusable workflow.

**Adapted candidate statement:** “The script remained an unfinished, creator-operated command-line tool; nobody else has used it independently.”  
**Candidate status:** Author-reported. Suitable for limitations, not as an adoption or impact claim.

### MX-12 — One artifact earns a broader belief

**Why it matches:** A Practice Note needs one bounded lesson, but that lesson must follow from a specific event rather than be generated from the existence of code.

**Adapted candidate statement:** “This project showed me that [bounded lesson] when [specific condition].”  
**Candidate status:** Unsupported until a failure, decision, and result form a causal chain.

## Proof-block specifications

### Proof block 1

**Type:** Constraint  
**Statement:** Unfinished CLI, used in two creator-run sessions  
**Optional qualifier:** Personal use only; no external validation  
**Evidence status:** Author-reported  
**Evidence ID:** AR-01  
**Intended placement:** Orientation  
**Originating source pattern:** none

### Proof block 2

**Type:** Next signal  
**Statement:** Can another person rename one screenshot batch without the creator's help?  
**Optional qualifier:** Requires packaging and an independent-use receipt  
**Evidence status:** Hypothesis  
**Evidence ID:** H-01  
**Intended placement:** Limitations or next experiment  
**Originating source pattern:** MX-05

No Impact, Adoption, or Influence block is supportable.

## Visual Evidence Plan

1. **Trigger evidence:** A real pre-script folder listing showing the original exported filenames. Do not reconstruct it unless clearly labeled.
2. **Method and result:** One terminal capture showing the command and the resulting filenames from the same real batch.
3. **Contrast:** A side-by-side before/after from one of the two actual runs. Do not claim time savings without a recorded baseline.
4. **Failure or change:** The actual error, edge case, or earlier output that caused a code or workflow change. If none exists, omit this module rather than inventing iteration.
5. **Ownership:** If AI-building craft is included, preserve the prompt, diff, or note that shows what AI executed and what the author reviewed or corrected.

## Claims to avoid or soften

- Do not call two creator-run sessions “adoption,” “user validation,” or “repeat usage.”
- Do not call the script a product, reusable system, or released tool without packaging and independent use.
- Do not claim that it saves time, reduces errors, or improves consistency without a known comparison.
- Do not imply a feedback-led iteration, evaluated alternative, or product decision when none is documented.
- Do not turn code volume, technical complexity, or an automated test into evidence of user value.
- Do not add an AI-collaboration lesson unless a concrete failure, intervention, and verified improvement can be shown.

## What would upgrade this to a full case study

- A working, packaged version that another person can run without the creator.
- A documented scope or interaction decision and the constraint behind it.
- A real-use receipt from someone other than the creator.
- Feedback that visibly changes a later version.
- A before/after task demonstration with a known measurement basis.

## First question

Which length should I use after the missing context is supplied: **Compact (recommended, 400–500 words)**, **Standard (500–600)**, or **Expanded (700–800)**?

I will not draft the Practice Note until you choose a length or explicitly delegate the choice.
