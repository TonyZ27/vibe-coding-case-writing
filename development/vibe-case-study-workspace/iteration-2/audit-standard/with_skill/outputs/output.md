# Audit Studio: Turning a Capture Shortcut into a Review Workspace

Audit Studio began as a utility I made for myself. It became a local web workspace where designers could inspect an in-car build, capture evidence, and assemble an audit record without stitching the process together across unrelated tools.

## The old workflow scattered the audit

Reviewing a build meant moving through a fixed chain: Test APK → QtScrcpy → screenshot or video → Finder → Figma or Excel. Each tool handled one part of the job, but the designer had to carry context between them. A captured issue was separated from the live build, the comparison that explained it, and the record where it would eventually be discussed.

My first response was narrow: a personal screenshot utility. It reduced one interruption but left the larger handoff intact. The recurring problem was not simply taking screenshots. It was keeping device access, evidence capture, visual comparison, and audit documentation connected around the same review task.

## I productized the sequence, not just the capture button

I rebuilt the utility as a local web workspace. Instead of treating screenshots as loose files, Audit Studio brought the live-device view and review actions into one place. A designer could work from the build, capture evidence, and continue toward an audit record without using Finder as the bridge between every step.

This reframed the product from a faster utility into workflow infrastructure. The useful unit was no longer an image; it was a traceable review sequence from build to selected evidence.

## Automation proposes; the designer decides

Screenshot Flow introduced the most consequential product boundary. The system detects candidate visual changes so designers do not need to find every difference manually. But detection does not decide what counts as an issue. The designer reviews the candidates, rejects irrelevant changes, and selects what enters the audit record.

That division of labor keeps automation useful without presenting machine-detected difference as design judgment. Audit evidence can depend on context, intent, and severity—questions the reviewer still owns. I designed the flow so automation narrows the search space while the designer remains accountable for the record.

## Facilitated trials changed what the product needed to become

More than ten designers joined facilitated trials. This was not self-serve adoption, and the workflow had not yet proven that it could spread independently. A stronger signal came when some designers returned with later builds. They were not only reacting to a demo; they were bringing the workspace back into continuing project work.

Those sessions also produced requests to upload design files to the in-car system. The request changed the product question. Audit Studio had started around fidelity checks—comparing what was built with what was intended—but designers were pointing toward a broader handoff between review evidence and the system under test.

> The strongest signal was not the size of the trial group. It was that **designers returned with later builds**, while their requests pushed Audit Studio beyond capture and fidelity checking toward a broader review workspace.

## What the system proved—and what remains open

Audit Studio shows how a personal shortcut can become a shared capability when the repeated task, decision points, and human responsibility are designed together. The trials support usefulness, repeat behavior, and product influence. They do not yet prove independent distribution or team-wide standardization.

The next meaningful signal would be whether designers can run the workflow without facilitation—and whether a returning designer ever introduces it to someone else. Until that happens, invitation remains a success criterion, not an adoption claim.

---

## Production notes

### Decision package

- Recommended archetype: Workflow / System
- Confidence: High. The case has repeated multi-tool friction, a working packaged workspace, real outputs, facilitated use by others, repeat behavior, and feedback that changed product scope.
- Story thesis: I turned a fragmented build-review chain into a local audit workspace that connects capture, automated candidate detection, designer judgment, and record creation.
- Selected length: Standard, 500–600 reader-facing words.
- Selected middle modules: Before Workflow; System Model; Encoding the Judgment; Adoption Loop; Boundary.
- Adoption level: Facilitated trial, with author-reported repeat use. No verified second-order adoption.

### Evidence map

- Observed: The defined workflow model; Screenshot Flow detects candidate changes; designer review and selection determine what enters the audit record; Audit Studio exists as a local web workspace.
- Author-reported: The confirmed before flow; origin as a personal screenshot utility; more than ten designers joined facilitated trials; some returned with later builds; designers requested design-file upload to the in-car system; that request expanded the product beyond fidelity checks.
- Hypothesis: Returning designers may invite other designers; independent use may become the next adoption signal.
- Unknown: Trial dates, participant roles, number of returning designers, whether trials covered complete audits, whether design-file upload was implemented, and whether anyone used the workspace without the creator present.

### Source-pattern adaptation

- MX-04, Repeated friction becomes a workflow: the disconnected Test APK → QtScrcpy → capture → Finder → Figma/Excel sequence becomes one review workspace organized around the audit task. Status: Author-reported, with the product model inspectable.
- MX-02, Feedback visibly changes the next version: requests for design-file upload shifted the scope beyond fidelity checking. Status: Author-reported; confirm implementation status before describing a shipped change.
- MX-09, Contribution expands product scope: participant requests changed the product direction. Status: Author-reported product influence, not adoption.
- MX-11, Second-order use is stronger than raw reach: designer-to-designer invitation is a future signal only. Status: Hypothesis; excluded from proof styling.

### Primary proof-statement specification

- Role: Primary proof statement
- Statement: The strongest signal was not the size of the trial group. It was that designers returned with later builds, while their requests pushed Audit Studio beyond capture and fidelity checking toward a broader review workspace.
- Inline emphasis: designers returned with later builds
- Evidence status: Author-reported
- Evidence IDs: AR-03 facilitated trials; AR-04 return behavior; AR-05 scope-expanding requests
- Intended placement: After the facilitated-trial and product-influence evidence.
- Originating source patterns: MX-02 and MX-09
- Visual intent: Full-width tinted callout; large text; one inline bold phrase; no visible category label.

### Visual receipts required

1. Before-workflow diagram showing the five handoffs and where context was lost.
2. Audit Studio workspace capture showing the live build and capture/review surfaces.
3. Screenshot Flow sequence: detected candidates → designer review/deselection → selected audit record.
4. An anonymized later-build return-use receipt or session artifact.
5. An anonymized request for design-file upload, paired with the resulting roadmap, flow, or implemented interface if available.

### Claims to avoid or qualify

- Do not call the facilitated trials self-serve adoption or organization-wide rollout.
- Do not claim measured time savings without a consistent task baseline.
- Do not say designers invited others unless a receipt confirms it happened.
- Do not imply Screenshot Flow determines correctness or audit severity.
- Do not describe design-file upload as shipped unless implementation evidence is available.
