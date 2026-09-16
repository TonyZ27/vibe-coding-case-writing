# Decision package

Recommended archetype: Product Utility  
Confidence: High  
Story thesis: By focusing on parents preparing a child’s application, I reduced a costly, overcomplicated photo task to a focused printable-sheet workflow—and learned that real photos and real requests should determine where AI implementation ends and product judgment begins.  
Length options: Compact (400–500 words) for this single clear arc; Standard (500–600) only with stronger v1/v2 and testing receipts; Expanded (700–800) only with multiple consequential decisions and richer adoption evidence.  
Recommended length: Compact, as selected.  
Observed evidence: None independently inspected; no repository, product, or artifacts were supplied.  
Author-reported evidence: Personal trigger; working upload, crop, dimension-validation, and printable-sheet flow; five parent users; two requests for a child-photo positioning guide; guide added in v2; designer/AI ownership split; manual crop correction after real-photo testing.  
Missing evidence: Product URL or build; screenshots; anonymized use and feedback receipts; v1/v2 comparison; examples of the crop failure and correction; exact passport-photo specification supported.  
Relevant source patterns: MX-01 Personal constraint sharpens scope; MX-02 Feedback visibly changes the next version; MX-06 Human–AI handoff beats full automation; MX-12 One artifact earns a broader belief.  
Adapted candidate statements: A costly personal task constrained v1 to the shortest complete path; two parent requests produced a visible v2 change; real-photo failures moved crop judgment back to the designer; a narrow utility can improve through concrete use rather than speculative scope.  
Candidate status: All four are Author-reported.  
Proof-block specifications: Adoption—“5 parents used the working product” (Author-reported; E-USE-01; after core flow; MX-01). Influence—“2 requests led to a child-photo positioning guide in v2” (Author-reported; E-FEEDBACK-01; beside v2 section; MX-02).  
Visual receipts required: Final product overview; 8–12 second upload-to-download demo; annotated crop before/after using a real photo; anonymized feedback beside a v1/v2 guide comparison.  
Claims to avoid or qualify: Do not call the product launched, compliant with every passport standard, broadly adopted, or proven to save money or time without supporting receipts.

---

# A simpler way for parents to prepare passport photos

After paying for an overcomplicated passport-photo service while preparing my child’s application, I built the focused utility I had expected to find: a parent can upload a photo, crop it, validate its dimensions, and download a printable sheet.

The project was small by design. It was not an attempt to replace the application process or interpret every passport rule. I focused on the shortest complete path from an existing photo to a file a parent could print.

> **Adoption**
> **5 parents used the working product**
> Author-reported use of the complete upload-to-download flow.

## Turning a frustrating purchase into a minimum useful flow

The original experience made a straightforward task feel like a service package. My response was to remove everything that did not help a parent finish the photo itself.

I framed the product around four actions: upload, crop, validate dimensions, and download. The sequence keeps attention on the photo and gives dimension feedback before the printable sheet is created. That boundary mattered: the utility needed to complete one job clearly, not accumulate adjacent application features.

[Visual: 8–12 second demo showing upload → crop → dimension validation → printable sheet.]

## Real photos exposed where the agent needed direction

I defined the product scope and interactions, then used an AI coding agent to implement the image-processing flow. The first implementation made the workflow functional, but testing with real photos exposed problems in the crop behavior.

I manually corrected that behavior and tested the flow again with real images. This was the pivotal build decision: implementation could be delegated, but the quality bar for how a parent positions a child’s face still required direct observation and adjustment. The useful boundary was not “human versus AI”; it was repeatable processing versus interaction judgment.

[Visual: annotated before/after showing the crop behavior that failed and the corrected result.]

## Two requests shaped v2

Five parents used the product. Two asked for guidance on positioning a child’s photo, so I added a positioning guide in v2. Their request revealed that correct output dimensions were only part of the uncertainty. Parents also needed confidence before downloading that the face was placed appropriately within the crop.

> **Influence**
> **2 parent requests → 1 positioning guide in v2**
> Feedback changed the product, not just the backlog.

[Visual: anonymized feedback receipt beside the v1 crop view and v2 positioning guide.]

The project changed how I approach small AI-built utilities. Start with the narrow task, use working software to expose interaction failures, and let specific behavior—not speculative feature ideas—earn the next version.

---

# Production notes

## Evidence and capture requests

1. **Core flow**
   - Claim supported: The working product completes upload, crop, dimension validation, and printable-sheet download.
   - Asset filename: `01-core-flow.mp4`
   - Capture: One uninterrupted end-to-end task.
   - Length: 8–12 seconds.
   - Must show: Input photo, crop adjustment, validation state, downloaded sheet.
   - Avoid: Personal application data or a full product tour.

2. **Crop correction**
   - Claim supported: Real-photo testing exposed crop behavior that the designer manually corrected.
   - Asset filename: `02-crop-correction.png`
   - Capture: Side-by-side failed and corrected crop with short annotations.
   - Must show: The same anonymized or consented photo in both states.
   - Avoid: Claiming the change guarantees official acceptance.

3. **v1 → v2**
   - Claim supported: Two parent requests led to the positioning guide.
   - Asset filename: `03-v1-v2-feedback.png`
   - Capture: Anonymized request excerpts beside matched v1 and v2 screens.
   - Must show: The guide as an inspectable product change.
   - Avoid: Names, child images, or identifying message metadata without consent.

## Claim verification

- E-PRODUCT-01 — Working four-step flow — Author-reported; verify with product demo or repository.
- E-USE-01 — Five parents used the product — Author-reported; verify with anonymized test/use log and clarify whether use was facilitated or self-serve.
- E-FEEDBACK-01 — Two requested positioning guidance — Author-reported; verify with anonymized messages or notes.
- E-V2-01 — Positioning guide added in v2 — Author-reported; verify with matched screenshots or version history.
- E-AI-01 — AI agent implemented image processing; designer framed interactions and corrected crop behavior — Author-reported; verify with prompts, diff/history, or annotated build notes if publicly appropriate.

## Confidentiality guidance

Use only consented or anonymized child photos. Remove names, application details, message metadata, and document identifiers. If feedback receipts cannot be published, retain careful attribution in the article and note privately that the evidence was reviewed.
