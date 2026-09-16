# Direction and evidence decision

Recommended format: Workflow / System

Confidence: High. The project begins with a concrete multi-tool workflow, became a reusable local workspace, was used by more than ten designers in facilitated trials, and changed scope in response to participant requests.

Alternative format: Product Utility, if the story is narrowed to the personal screenshot tool and its immediate fidelity-checking value. This would underplay the stronger evidence that the workflow traveled beyond its creator and evolved through use.

Story Thesis: I turned a fragmented capture-to-audit workflow into a local web workspace that helps designers move from a running Test APK to a reviewed audit record, while keeping the final evidence decision in human hands.

Observed evidence: None supplied as independently inspectable artifacts in this task.

Author-reported evidence:

- Confirmed before flow: Test APK → QtScrcpy → screenshot or video → Finder → Figma or Excel.
- Audit Studio evolved from a personal screenshot utility into a local web workspace.
- More than ten designers joined facilitated trials.
- Some designers returned with later builds.
- Requests to upload design files to the in-car system expanded the product beyond fidelity checks.
- Screenshot Flow detects candidate visual changes; a designer reviews and selects what enters the audit record.
- Designer-to-designer invitations are hypothetical, not observed.

Missing context:

- Inspectable before/after artifacts and a real audit record.
- How Audit Studio was packaged, launched, or shared with trial participants.
- Which parts the author, AI, and collaborators each defined or implemented.
- A concrete AI-building failure or correction that changed the build method.
- Whether later-build use happened independently or through another facilitated session.
- Public or anonymizable receipts for trial participation, return use, and upload requests.

Recommended length: Standard — 800–1,100 words.

Length rationale: The evidence supports a meaningful evolution, three consequential product decisions, a human–automation boundary, facilitated trial behavior, and a scope-changing request. It does not yet support the additional phases or deeper distribution evidence needed for Extended.

Length options for user selection:

- Compact — 450–650: best if the case should focus only on the old workflow and Screenshot Flow’s review boundary.
- Standard — 800–1,100: selected because it can carry the personal-tool-to-shared-workspace evolution, trial evidence, and product-scope change without padding.
- Extended — 1,300–1,800: worthwhile only with version history, detailed distribution constraints, richer adoption receipts, and a concrete AI-building episode.

Adoption level: Facilitated trial, with a return-use signal from designers who brought later builds. Do not claim self-serve reuse, contribution, second-order adoption, or organization-wide rollout.

Selected narrative modules: Before Workflow; System Model; Workflow Walkthrough; Adoption Loop; Failure / Boundary.

Candidate proof blocks: the confirmed five-step before flow; 10+ designers in facilitated trials; automatic detection with designer selection; upload requests expanding scope beyond fidelity checks.

Visual Evidence Plan: a before-workflow diagram; a real Screenshot Flow input/review/output sequence; the local workspace surface; an anonymized facilitated-trial receipt; a later-build return receipt; and the design-upload request paired with the resulting product change.

Claims to avoid or soften: time saved; full replacement of every old tool; autonomous visual auditing; correctness without designer review; self-serve adoption; designer-to-designer invitation; organization-wide use; target-system compatibility; and AI-building capability growth without a concrete episode.

---

# Audit Studio: Turning a fragmented audit handoff into a shared workspace

I turned a personal screenshot utility into Audit Studio, a local web workspace for reviewing in-car interface builds. It brought a fragmented capture-to-documentation workflow into one working surface, then grew through facilitated use by other designers.

The aim was not to automate design judgment. It was to remove enough operational friction that designers could spend that judgment on the evidence that mattered.

## At a glance

**What:** A local workspace for capturing, reviewing, and organizing visual audit evidence from Test APKs.

**How:** Screenshot Flow detects candidate visual changes, then asks a designer to decide which ones belong in the audit record.

**Why it matters:** More than ten designers joined facilitated trials. Some returned with later builds, and their requests began to move the product beyond fidelity checks.

> **Constraint**
> **Test APK → QtScrcpy → screenshot or video → Finder → Figma or Excel**
> The confirmed before flow moved evidence across five distinct stages before it became part of an audit.

## The audit was scattered across the handoff

The starting point was a practical sequence. A designer opened a Test APK through QtScrcpy, captured a screenshot or video, found the exported file in Finder, and moved it into Figma or Excel to continue the audit.

Each tool performed a legitimate job, but the audit itself lived between them. Capturing evidence and turning it into a usable record were separate activities. The designer had to carry context across the running build, exported media, and a documentation surface.

I first responded to my own part of that friction with a screenshot utility. That solved a narrow capture problem, but it also revealed a larger opportunity: the useful unit was not the screenshot. It was the path from a running build to reviewed, traceable audit evidence.

## From a personal utility to a local workspace

I expanded the utility into Audit Studio, a local web workspace. This changed the product’s center of gravity. Instead of treating capture as the finish line, the workspace could support the sequence around it: bringing evidence together, reviewing it, and deciding what should enter the audit record.

Keeping the workspace local made it suited to the working context in which I was building it. More importantly, turning the utility into a workspace made the workflow legible to someone other than me. A designer could work through the audit in a shared product model instead of inheriting my personal file-handling habits.

This is also where the project became a system rather than a collection of shortcuts. The system had an input—a build and its visual states; an automated action—finding candidate changes; a decision point—designer review; and an output—a selected audit record.

## Detection narrows the field; the designer makes the claim

Screenshot Flow detects candidate visual changes. That detection is deliberately not the final audit decision. A designer reviews the candidates and selects what should be recorded.

That boundary matters because a visual difference is not automatically a design issue. A detected change may be expected, irrelevant, duplicated, or meaningful only in context. If Audit Studio wrote every candidate directly into the audit record, it would make the output look more certain while reducing its usefulness.

The workflow therefore uses automation for breadth and human review for meaning:

1. The system detects candidate visual changes.
2. The designer reviews those candidates in context.
3. The designer selects the evidence that enters the audit record.

> **Insight**
> **Detect automatically; curate deliberately.**
> Audit Studio accelerates evidence discovery without outsourcing the audit decision.

This division of labor became the core product principle. Automation should reduce the cost of looking, not erase accountability for what the audit says.

## Facilitated trials showed that the workflow could travel

More than ten designers joined facilitated trials of Audit Studio. This was not self-serve adoption: I was present in the trial context, so the evidence supports a claim about guided use rather than independent rollout.

Still, the trials moved the project beyond personal utility. Other designers could bring their own work into the workflow and evaluate whether the workspace helped them audit it. Some later returned with newer builds, a stronger signal than first-session interest because they saw enough value to apply the workflow again as their product changed.

> **Adoption**
> **10+ designers joined facilitated trials.**
> Some returned with later builds; independent self-serve reuse remains unverified.

The boundary is as useful as the signal. I can say that designers tried the workflow and that some returned. I cannot say that they adopted it without support, rolled it out across an organization, or invited other designers. That last behavior remains a hypothesis to test, not a portfolio outcome.

## Use expanded the product beyond fidelity checks

The most consequential feedback did not ask for a faster version of the same audit. Designers requested the ability to upload design files to the in-car system. That pushed Audit Studio beyond comparing implementation fidelity and toward a broader design-validation workflow.

The request changed the product question. Audit Studio was no longer only about documenting whether a build matched an intended design. It could begin to support getting design material into the environment where designers needed to evaluate it.

> **Influence**
> **Upload requests expanded the product’s scope.**
> Facilitated use revealed a need beyond fidelity checks: moving design files toward the in-car system.

This is the clearest evidence of influence in the project. The trials did not merely confirm the original concept; they exposed an adjacent job and redirected what the workspace could become.

## What Audit Studio proves—and what it does not

Audit Studio shows how a repeated handoff can become a reusable capability when the workflow, decision boundary, and output are made explicit. It also shows why a system does not need to automate the final judgment to create leverage. In this case, preserving designer selection is part of the product’s integrity.

The current evidence supports facilitated trial, return behavior, and product influence. It does not yet prove self-serve distribution or second-order adoption. Those are the next validation boundaries: can a designer start the workflow without me, use it on another build, and help another designer do the same?

The lesson I would carry forward is narrow but durable: automate the search space, then design the moment where a person turns detected information into a defensible decision.

---

# Production notes

## Evidence and capture requests

1. Capture the old flow with real, anonymized screens from Test APK, QtScrcpy, Finder, and the final Figma or Excel record. Present it as a workflow diagram, not a tool collage.
2. Record one real Screenshot Flow run showing the source state, detected candidates, designer review, selections, and resulting audit record.
3. Capture the local workspace’s launch or access surface to show how the workflow was packaged and shared.
4. Add an anonymized receipt for the 10+ facilitated-trial count, such as a session log or participant list with identifying details removed.
5. Pair one later-build return with dated or versioned evidence. Confirm whether it was independently initiated or part of another facilitated session.
6. Pair an upload request with the resulting interface or version change. If the feature was not implemented, describe it only as a scope-changing request or future direction.

## Claim verification

- Keep “facilitated trials” in every public claim about the 10+ designers.
- Describe later builds as return behavior until independent reuse is verified.
- Do not publish the hypothetical claim that returning designers invited others.
- Do not claim time savings without a consistent before/after task and measurement basis.
- Do not imply Screenshot Flow produces correct audit findings automatically; selection remains a designer decision.
- Verify what “uploading design files to the in-car system” technically means before implying compatibility, deployment, or successful use in the target environment.

## Ownership and AI-building gap

The author’s ownership of the utility-to-workspace evolution is clear from the supplied account. Before publication, document who defined the product decisions, who implemented the system, what AI executed, and what collaborators contributed. No AI-building craft section appears in the public draft because the current evidence contains no concrete constraint → changed agent method → better result episode.

## Confidentiality guidance

Blur product names, unreleased vehicle UI, participant identities, build identifiers, file paths, and internal issue content. Preserve dates or version relationships where they are needed to prove return behavior, but replace sensitive labels consistently.

## Editorial pattern used

The outline uses two compatible source-library patterns: “Repeated friction becomes a workflow” for the before-to-system progression, and “Feedback visibly changes v2” for the upload-request expansion. The final reflection follows “One artifact becomes a broader belief,” bounded to the demonstrated human–automation decision rather than a general claim about AI.
