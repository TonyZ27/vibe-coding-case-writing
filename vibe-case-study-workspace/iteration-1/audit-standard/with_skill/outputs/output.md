# Audit Studio — Decision Package

Recommended archetype: Workflow / System  
Confidence: High  
Story thesis: I turned a fragmented Android HMI review process into a local web workspace that connects build review and evidence capture while keeping the designer responsible for what enters the audit record.  
Selected length: Standard — 500–600 words. The evidence supports a clear before state, product evolution, a consequential automation boundary, facilitated trials, and feedback-led scope expansion.  
Observed evidence: No product or repository evidence was independently verified for this response.  
Author-reported evidence: The confirmed before flow; the evolution from personal screenshot utility to local web workspace; facilitated trials with more than ten designers; some designers returning with later builds; requests to upload design files to the in-car system; Screenshot Flow's candidate detection and designer-controlled selection.  
Missing evidence: Publishable screenshots of the workspace and Screenshot Flow; anonymized trial, return-use, and feature-request receipts; one real input/output audit record; confirmation of which capabilities work end to end.  
Relevant source patterns: MX-04 Repeated friction becomes a workflow; MX-02 Feedback visibly changes the next version; MX-11 Second-order use is stronger than raw reach.  
Adapted candidate statements: The disconnected review sequence became one workspace organized around the audit task (Author-reported). Requests to validate design files in-car expanded the product beyond fidelity checks (Author-reported). Returning designers inviting others would indicate second-order adoption (Hypothesis).  
Claims to avoid or qualify: Do not call facilitated trials self-serve adoption. Do not claim time savings, production readiness, independent reuse, or designer-to-designer invitations without receipts.

# Public Case-Study Draft

# From a Screenshot Shortcut to a Shared HMI Review Workspace

I built Audit Studio after noticing that a routine Android HMI review was spread across a chain of tools. What began as a personal screenshot utility became a local web workspace, shaped by facilitated trials with more than ten designers and by requests that pushed the product beyond implementation-fidelity checks.

> **Impact**
> **A fragmented review flow became one workspace**
> Build review, capture, and evidence handling were organized around one designer task.

## One review, six handoffs

The original workflow was consistent but fragmented: receive a test APK, open it through QtScrcpy, capture screenshots or video, find and organize the files in Finder, then move the evidence into Figma or Excel.

Each tool handled its part. The friction came from the handoffs between them. The designer had to keep the review state, the captured media, and the eventual audit record connected manually.

I first addressed the part I felt most directly: taking screenshots. That utility solved a personal inconvenience, but it did not yet reorganize the full review.

## Turning utilities into a review workflow

I moved the utility into a local web workspace and structured it around what a designer was trying to accomplish: open a build, inspect the in-car experience, capture relevant states, and carry selected evidence into an audit record.

This reframing mattered more than adding another capture control. Audit Studio connected previously separate actions into one sequence, so the product model followed the review rather than the underlying technical tools.

The key design decision appeared in Screenshot Flow. As a designer moves through the interface, the system detects candidate visual changes. It does not decide that every changed frame deserves to become evidence. The designer reviews the candidates and selects what enters the audit record.

> **Insight**
> **Detect changes automatically; curate evidence deliberately**
> The system handles repetitive detection while the designer retains editorial judgment.

That boundary made the automation useful without pretending that visual difference and design significance are the same thing. Detection is mechanical. Relevance depends on the review question, context, and the designer's judgment.

## Trials changed the product's scope

I introduced the workspace through facilitated sessions. More than ten designers joined the trials, and some returned with later builds to review. Because I was still present, I treat this as repeated trial behavior—not proof of self-serve adoption.

> **Adoption**
> **10+ designers joined facilitated trials**
> Some returned with later builds, showing repeated demand while the workflow still depended on facilitation.

The more consequential signal was what participants asked for next. Some wanted to upload design files to the in-car system and review them in context before implementation. Their request expanded the problem from checking whether a build matched a design to supporting broader in-car design validation.

That changed my understanding of the product. Audit Studio was no longer just a faster path to screenshots. It was becoming a workspace where designers could bring different review inputs to the same physical context, observe the result, and decide what evidence mattered.

## What this case changed for me

Audit Studio taught me that the product opportunity was not a new capture technology. It was the orchestration of existing capabilities around a designer's actual review sequence—and a clear boundary between what the system can notice and what a designer must decide.

# Production Notes

## Evidence and capture requests

1. **Before workflow** — Create a reconstructed diagram labeled: `Test APK → QtScrcpy → screenshot/video → Finder → Figma or Excel`. Do not add time or efficiency estimates.
2. **Workspace overview** — Capture the local web workspace with a real or approved demo build visible. This supports the shift from personal utility to shared workflow.
3. **Screenshot Flow** — Record a 10–15 second sequence showing candidate detection, review, deselection, and saving. Keep both automatic and human actions visible.
4. **Real input/output pair** — Show one source build state beside the selected evidence in an audit record. Redact product names, device identifiers, internal paths, and confidential HMI content.
5. **Trial receipt** — Provide anonymized evidence that more than ten designers participated and that some returned with later builds.
6. **Influence receipt** — Pair an anonymized request to upload design files to the in-car system with the resulting product direction or implemented change. Until implementation is shown, describe this as scope expansion, not delivered capability.

## Proof-block specifications

| Type | Statement | Qualifier | Evidence status | Evidence ID | Placement | Source pattern |
| --- | --- | --- | --- | --- | --- | --- |
| Impact | A fragmented review flow became one workspace | Build review, capture, and evidence handling were organized around one designer task. | Author-reported | AS-WORKFLOW-01 | After hero | MX-04 |
| Insight | Detect changes automatically; curate evidence deliberately | The system handles repetitive detection while the designer retains editorial judgment. | Author-reported | AS-BOUNDARY-01 | Screenshot Flow section | none |
| Adoption | 10+ designers joined facilitated trials | Some returned with later builds; the creator still facilitated use. | Author-reported | AS-TRIAL-01 | Trials section | MX-11, qualified |

## Claim verification and boundaries

- Verify every product capability shown in the public draft with a fresh end-to-end capture before publication.
- Keep “more than ten” and return behavior attributed until anonymized receipts are available.
- Call the current evidence **facilitated trial**, not self-serve adoption, reuse, or team-wide rollout.
- Do not claim that returning designers invited others. That is a **hypothesis** and may appear only as a future success signal: “Do returning designers bring other designers into the workflow without creator facilitation?”
- Do not claim reduced review time without a consistent before/after measurement.
- Do not imply that requests to upload design files prove the capability was implemented.
- Do not use tests, interface screenshots, or code complexity as evidence of user value.
- No AI-building craft section is included because no concrete failure, correction, or changed agent-working method was supplied.

## Confidentiality guidance

Use only approved HMI content. Redact designer names, project names, build identifiers, device details, internal paths, and chat metadata. If a real product screen cannot be published, capture an approved demo rather than generating replacement product UI and presenting it as evidence.
