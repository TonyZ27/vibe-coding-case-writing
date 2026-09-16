# Direction

Recommended archetype: Product Utility  
Confidence: High  
Story thesis: By focusing on a parent completing a child's passport application, I reduced a costly, rules-heavy task to a focused upload-to-print flow, showing how a small utility becomes useful through precise interaction judgment rather than feature breadth.  
Selected length: Compact (400–500 words)  
Selected middle modules: Minimum Useful Scope; AI Collaboration; v1 → v2  

Observed evidence: None supplied for independent inspection.  
Author-reported evidence: The paid service was overcomplicated; the working utility supports upload, crop, dimension validation, and printable-sheet download; five parents used it; two requested a child-photo positioning guide; the guide was added in v2; the author framed the product and interactions; an AI coding agent implemented image processing; real-photo testing led the author to manually correct crop behavior.  
Missing evidence: Product URL or screen captures, anonymized feedback receipts, v1/v2 comparison, crop-failure example, and confirmation of whether use was independent or facilitated.  

Relevant source patterns: MX-01 Personal constraint sharpens scope; MX-02 Feedback visibly changes the next version; MX-06 Human-AI handoff beats full automation.  
Adapted candidate statements: A personal application task constrained v1 to the shortest complete path from photo to printable sheet. Two parents' requests led to a visible v2 positioning guide. Real-photo failures established a boundary between agent implementation and human interaction judgment.  
Candidate status: Author-reported.  

Primary proof-statement specification: Product influence; the request from two of five parent users changed v2. Evidence status: Author-reported. Evidence IDs: AR-04, AR-05. Placement: after the v1 → v2 passage. Originating source pattern: MX-02. Visual intent: full-width tinted callout, large text, one inline bold phrase, no visible label.  

Visual receipts required: Final product overview; 8–12 second upload-to-print demo; annotated crop correction; anonymized request beside v1/v2 guide comparison.  
Claims to avoid or qualify: Do not call five uses broad adoption, imply self-serve use without confirmation, claim compliance beyond dimension validation, or describe AI implementation as autonomous product design.

---

# A simpler path from family photo to passport print

While preparing my child's passport application, I paid for a photo service that turned a straightforward need into an overcomplicated process. I wanted one thing: a correctly sized photo I could print. That experience became the brief for a small working utility designed around the parent completing the task.

## The shortest complete flow

I limited the first version to four steps: upload a photo, crop it, validate its dimensions, and download a printable sheet. The product did not try to become a general photo editor or reproduce every service surrounding an application. Its job was to help a parent move from an existing photo to a print-ready output without navigating unrelated options.

The interaction sequence made the requirements visible at the moment they mattered. Upload established the source image; cropping let the parent control the composition; dimension validation checked the output before download. The printable sheet completed the real task rather than stopping at a digital passport image.

*Visual: the upload-to-download flow, shown as an 8–12 second task demo.*

## Directing AI, correcting the crop

I framed the product, defined the task flow, and designed the interactions. An AI coding agent implemented the image-processing flow. That division accelerated the build, but real photos exposed a quality boundary: the crop behavior did not consistently match the composition a parent intended.

I tested the flow with actual family photos, identified where the crop result diverged from the selected frame, and manually corrected the behavior. The useful handoff was not “AI builds, designer reviews.” It was more specific: I could delegate the repeatable processing logic, but I needed to retain judgment over the interaction connecting a parent's visual choice to the generated image.

*Visual: annotated before-and-after showing the crop mismatch and corrected output.*

## Five uses changed the next version

Five parents used the product. Two asked for guidance on positioning a child's face in the photo. Their request revealed that correct dimensions were only one part of feeling ready to print: parents also needed confidence in how the child should sit within the frame.

I added a child-photo positioning guide in v2, placing guidance inside the task instead of expecting parents to interpret the requirement elsewhere.

> The strongest signal was not that five parents tried the utility. It was that **their use changed v2**: two requests exposed a missing confidence cue, and the positioning guide became part of the product.

*Visual: anonymized feedback beside the v1 crop screen and v2 positioning guide.*

## What I learned

This project changed how I approach small AI-built products. A narrow scope can make a utility useful quickly, but implementation speed does not settle the experience. Real inputs reveal where automation needs product judgment, and real requests show which missing guidance is worth adding next.

---

# Production notes

## Evidence register

- AR-01 — Trigger: paid for an overcomplicated passport-photo service while preparing a child's application.
- AR-02 — Working flow: upload, crop, validate dimensions, download printable sheet.
- AR-03 — Ownership: author framed product and interactions; AI coding agent implemented image processing; author corrected crop behavior after real-photo testing.
- AR-04 — Use: five parents used the product.
- AR-05 — Influence: two parents requested a child-photo positioning guide; it was added in v2.

All evidence is author-reported. Before publication, link each claim to an inspectable receipt where practical.

## Capture requests

1. **Core-task demo**  
   Claim supported: The product completes the path from upload to printable sheet.  
   Asset filename: `passport-utility-core-flow.mp4`  
   Capture: One uninterrupted run using a consented or synthetic photo.  
   Length: 8–12 seconds.  
   Must show: Upload, crop, dimension validation, and printable-sheet output.  
   Avoid: Personal data, official application identifiers, or unverified compliance claims.  
   Caption intent: A deliberately limited flow completes the parent's actual print task.

2. **Crop correction**  
   Claim supported: Real-photo testing caused a manual interaction correction.  
   Asset filename: `crop-behavior-before-after.png`  
   Capture: Side-by-side selection frame, incorrect result, and corrected result.  
   Must show: The specific mismatch and the same photo after correction.  
   Avoid: A reconstructed failure presented as historical evidence.  
   Caption intent: The build exposed where image-processing logic diverged from the parent's intended composition.

3. **Feedback-led v2**  
   Claim supported: Two parents' requests led to the positioning guide.  
   Asset filename: `feedback-to-v2-guide.png`  
   Capture: Anonymized feedback excerpts beside v1 and v2 screens.  
   Must show: Request language, removal of names and contact details, and the implemented guide.  
   Avoid: Implying that two requests represent broad demand.  
   Caption intent: Use exposed a confidence gap that dimension validation alone did not solve.

## Claim verification and confidentiality

- Confirm whether all five parents completed the flow independently or with guidance; use “used” only if that wording remains accurate.
- Verify that the positioning guide shown in the product is the same change prompted by the two requests.
- Describe dimension validation precisely. Do not imply government approval, guaranteed acceptance, or full passport-rule compliance unless verified.
- Use a synthetic, staged, or explicitly consented child photo in public visuals. Remove names, timestamps, application details, metadata, and identifiable feedback information.
- Public article length: 478 words including title, headings, captions, and proof statement; production notes excluded.
