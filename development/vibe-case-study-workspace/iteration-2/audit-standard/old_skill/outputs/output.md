# Direction and evidence decision

Recommended archetype: Workflow / System  
Confidence: High  
Story thesis: I turned a fragmented HMI review handoff into a local workspace that helps designers move from a running Test APK to a curated audit record, while keeping the evidence decision in human hands.  
Selected length: Standard — 500–600 words. The evidence supports a clear before state, a meaningful product evolution, one consequential automation boundary, facilitated trial behavior, and feedback-led scope expansion.  
Observed evidence: No repository, product, or receipt was independently inspected for this response.  
Author-reported evidence: The confirmed before flow; the personal utility’s evolution into a local web workspace; more than ten designers in facilitated trials; some returning with later builds; requests to upload design files to the in-car system; candidate detection followed by designer review and selection.  
Missing evidence: A real input/output audit record; public workspace captures; anonymized receipts for trial participation, return behavior, and upload requests; packaging and access details; ownership across the author, AI, and collaborators.  
Relevant source patterns: MX-04 Repeated friction becomes a workflow; MX-02 Feedback visibly changes the next version; MX-11 Second-order use is stronger than raw reach.  
Adapted candidate statements: The disconnected review sequence became one workspace organized around the audit task (Author-reported). Upload requests expanded the product beyond fidelity checks (Author-reported). Designer-to-designer invitation would be a future signal of second-order adoption (Hypothesis).  
Claims to avoid or qualify: Self-serve adoption, independent reuse, invitation behavior, measured time savings, autonomous auditing, organization-wide rollout, implemented design-file upload, and AI-building capability growth.

# Public case-study draft

# Audit Studio: From Capture Utility to HMI Review Workspace

I built Audit Studio after seeing one HMI review repeatedly stretch across disconnected tools. What began as a screenshot utility for my own work became a local web workspace where designers could inspect a build, collect visual evidence, and decide what belonged in an audit record.

## At a Glance

**What:** A local workspace for reviewing Test APKs and organizing visual audit evidence.  
**How:** It connects capture and review while leaving evidence selection to the designer.  
**Context:** Developed from a personal utility and introduced to other designers through facilitated trials.

> **More than ten designers joined facilitated trials, and some returned with later builds.**  
> This is evidence of repeated trial behavior, not self-serve adoption.

## The audit lived between five tools

The confirmed workflow started with a Test APK. A designer opened it through QtScrcpy, captured a screenshot or video, found the exported media in Finder, then moved it into Figma or Excel. Each tool did its job, but the review depended on the designer carrying context across every handoff.

My first response was narrow: a utility that made screenshots easier. Using it showed me that capture was not the complete problem. The useful outcome was a traceable path from a running build to evidence a designer could review and use.

## Reframing a shortcut as a workspace

I expanded the utility into a local web workspace organized around that path. Instead of ending at an exported image, Audit Studio brought build inspection, capture, review, and record-making into one product model.

This reframing made the workflow usable by people other than me. A designer could bring in a build, move through its states, and collect potential evidence without inheriting my personal file-management habits. The workspace did not eliminate every underlying tool; it connected their roles around the audit task.

## Detection supports judgment; it does not replace it

Screenshot Flow introduced the most important product boundary. It detects candidate visual changes, but it does not automatically declare those changes audit findings. The designer reviews the candidates, removes irrelevant or duplicate states, and selects what enters the record.

That division of labor is deliberate. A visual difference may be expected, insignificant, or meaningful only in context. Automating detection widens the search; designer curation turns a candidate into defensible evidence. The product therefore reduces repetitive looking while preserving responsibility for what the audit claims.

## Facilitated use changed what came next

More than ten designers joined facilitated trials. Some later returned with newer builds, showing that the workflow remained useful as their work changed. Because I was present in this trial context, I treat their return as repeated trial behavior rather than independent reuse or adoption.

The strongest influence signal was a new request: designers wanted to upload design files to the in-car system. That request expanded the opportunity beyond checking whether implementation matched a design. It pointed toward a broader workspace for evaluating design material in its intended environment.

This did not prove that the upload capability was delivered or adopted. It changed the product direction. Audit Studio taught me to look past the utility that starts a project and identify the workflow people are actually trying to complete—and to automate discovery without automating the final judgment.

# Production notes

## Proof-statement specification

- Type: Adoption
- Statement: More than ten designers joined facilitated trials, and some returned with later builds.
- Optional qualifier: This is repeated trial behavior, not self-serve adoption.
- Evidence status: Author-reported
- Evidence ID: AS-TRIAL-01
- Intended placement: After At a Glance
- Originating source pattern: MX-11, qualified

## Visual receipts required

1. A reconstructed before-flow diagram labeled `Test APK → QtScrcpy → screenshot or video → Finder → Figma or Excel`.
2. A real Screenshot Flow sequence showing candidate detection, designer review, deselection, and the selected audit record.
3. The local workspace with an approved demo build, showing how inspection, capture, and evidence handling connect.
4. An anonymized trial receipt supporting the participant count and at least one dated or versioned later-build return.
5. An anonymized upload request paired with the resulting product direction or implemented change.

## Claim verification and boundaries

- Keep the trial count and return behavior attributed until receipts are available.
- Call the current evidence facilitated trial, not self-serve adoption, independent reuse, or team-wide rollout.
- Do not claim that returning designers invited others. Treat invitation only as a future success signal.
- Describe design-file upload as a scope-expanding request unless implementation and target-environment use are verified.
- Do not claim time savings, audit correctness, or full replacement of the existing toolchain without evidence.
- Keep Screenshot Flow’s human boundary explicit: the system detects candidates; the designer decides what enters the record.
- Omit an AI-building craft section until a concrete constraint, changed agent-working method, and verified result can support it.

## Confidentiality guidance

Use approved demo content where possible. Redact participant names, unreleased HMI screens, project and build identifiers, device details, internal paths, and request metadata. Preserve dates or version relationships only where needed to substantiate return behavior.
