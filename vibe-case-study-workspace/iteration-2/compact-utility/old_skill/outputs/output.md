# Direction and evidence package

**Recommended archetype:** Product Utility  
**Confidence:** High. The project begins with a specific personal trigger, has a complete narrow task, distinguishes designer and AI ownership, and includes real-use feedback that produced a visible v2 change.  
**Story thesis:** By focusing on a parent preparing a child's application, I turned a costly, overcomplicated passport-photo task into a direct upload-to-print flow—and learned that real photos and real users reveal the guidance automation misses.

**Length options:**

- Compact — 400–500 words: selected; enough room for the trigger, one detailed crop decision, and the feedback-led v2 change.
- Standard — 500–600 words: useful only with deeper evidence about alternatives, testing, and iteration.
- Expanded — 700–800 words: not supported by the current evidence set.

**Recommended length:** Compact, as selected.

**Observed evidence:** None independently inspected in the supplied materials.

**Author-reported evidence:** A paid service felt overcomplicated during the author's child's application; the working product supports upload, crop, dimension checking, and printable-sheet download; five parents used it; two requested a child-photo positioning guide; the guide was added in v2; the author framed the product and interactions; an AI coding agent implemented image processing; the author manually corrected crop behavior after testing real photos.

**Missing evidence:** Product URL or repository; exact dimensions or jurisdictions supported; screen recordings of the complete flow and corrected crop behavior; v1/v2 comparison; anonymized use and feedback receipts; whether use was self-directed or facilitated; evidence that downloaded sheets were successfully accepted.

**Relevant source patterns:** MX-01 Personal constraint sharpens scope; MX-02 Feedback visibly changes the next version; MX-06 Human-AI handoff beats full automation.

**Adapted candidate statements:**

- A specific application task narrowed v1 to the four actions needed to reach a printable sheet. — **Author-reported**
- After two parents asked for help positioning a child's photo, I added a guide in v2. — **Author-reported**
- The agent implemented the processing flow, while real-photo testing showed where I needed to retake control of crop behavior. — **Author-reported**

**Selected middle modules:** Minimum Useful Scope; Core Interaction and AI Collaboration; v1 → v2.

**Proof-block specifications:**

1. Type: Adoption  
   Statement: Five parents used the working product.  
   Optional qualifier: Use mode is not yet documented.  
   Evidence status: Author-reported  
   Evidence ID: AR-USE-01  
   Intended placement: Hero, after orientation  
   Originating source pattern: MX-01

2. Type: Influence  
   Statement: Two parent requests led to a child-photo positioning guide in v2.  
   Optional qualifier: Request and v2 receipts needed.  
   Evidence status: Author-reported  
   Evidence ID: AR-FEEDBACK-02  
   Intended placement: Beside the v1 → v2 section  
   Originating source pattern: MX-02

**Visual receipts required:** Product overview; 8–12 second upload-to-download task demo; annotated before/after of the crop correction; anonymized feedback beside the v1/v2 guide comparison.

**Claims to avoid or qualify:** Do not call the product officially compliant, claim successful application outcomes, describe five uses as broad adoption, imply independent/self-serve use without confirmation, or present the AI implementation itself as impact.

---

# A simpler path from family photo to printable passport sheet

I built a focused passport-photo utility after paying for a service that made a small but important task feel unnecessarily complicated. While preparing my child's application, I needed a clear path from an existing photo to a sheet I could print. The product turns that path into four actions: upload, crop, check the required dimensions, and download a printable layout.

> **Adoption**
> **Five parents used the working product**
> Their use provided the first signal beyond my own application task.

## Reducing the task to what a parent needs

The starting point was not a broad photo-editing product. It was one moment: a parent has a photo and needs to prepare it for an application without navigating a feature-heavy service.

I framed the product and its interactions around the shortest complete journey. Uploading establishes the source image. Cropping gives the parent control over composition. A dimension check makes the output requirements visible before export. Downloading a printable sheet produces something the parent can use outside the browser.

Keeping those steps together mattered more than adding editing tools. Each screen needed to answer one practical question: What should I do next, and is this image ready to print?

## The crop worked in code—but not yet with real photos

I used an AI coding agent to implement the image-processing flow. My role was to define the experience, direct the interaction behavior, and decide whether the result held up against the task.

That boundary became clear when I tested the utility with real photos. The generated crop behavior technically processed the images, but the interaction did not behave the way I expected with varied source photos. I manually corrected it, testing the revised behavior against those images rather than treating a functioning pipeline as a finished experience.

This was the project's most useful AI-building lesson: implementation can establish the flow, but product judgment still has to set—and verify—the behavior users encounter.

## Five uses revealed the missing guidance

Five parents used the product. Two asked for help positioning a child's photo, exposing a gap in the first version: the utility could provide the controls without making a good composition obvious.

In v2, I added a child-photo positioning guide. The request did not expand the product into a larger editor; it sharpened the existing crop step with guidance specific to the situation.

> **Influence**
> **Two parent requests changed v2**
> Their feedback became a positioning guide inside the crop experience.

The result is a working, deliberately narrow utility shaped by one family task, corrected through real-photo testing, and improved through parent feedback. It reinforced a principle I would carry into similar tools: the minimum useful product is not only the shortest route to an output. It also includes the guidance people need to make the key decision along that route.

---

# Production notes

## Evidence and capture requests

### 1. Product overview

- **Section:** Hero
- **Claim supported:** The working product covers upload, crop, dimension check, and printable-sheet download.
- **Asset filename:** `passport-utility-overview.png`
- **Capture:** Final product state with the complete flow visible or represented.
- **Dimensions:** 1600 × 1000 px minimum.
- **Must show:** Real interface, task sequence, and printable output.
- **Avoid:** Personal data, a fabricated acceptance badge, or unsupported compliance language.
- **Caption intent:** One narrow flow takes a parent from source photo to printable sheet.

### 2. Core-task demo

- **Section:** Reducing the task to what a parent needs
- **Claim supported:** The product provides a complete upload-to-download journey.
- **Asset filename:** `passport-utility-core-flow.mp4`
- **Capture:** Upload → crop → dimension check → download.
- **Length:** 8–12 seconds.
- **Must show:** State changes and final sheet.
- **Avoid:** Long cursor travel or hidden manual intervention.
- **Caption intent:** Four actions complete the task.

### 3. Crop correction

- **Section:** The crop worked in code—but not yet with real photos
- **Claim supported:** Real-photo testing led to a manual correction of crop behavior.
- **Asset filename:** `passport-crop-before-after.png`
- **Capture:** Same anonymized photo under the initial and corrected behavior, with concise annotations.
- **Dimensions:** 1600 × 900 px minimum.
- **Must show:** The specific behavioral difference and why the correction matters.
- **Avoid:** Reconstructed UI presented as an original screenshot.
- **Caption intent:** A functioning image pipeline still needed interaction-level correction.

### 4. Feedback-led v2

- **Section:** Five uses revealed the missing guidance
- **Claim supported:** Two requests led to the positioning guide.
- **Asset filename:** `passport-v1-v2-feedback.png`
- **Capture:** Anonymized feedback excerpt beside the v1/v2 crop comparison.
- **Dimensions:** 1600 × 1000 px minimum.
- **Must show:** Feedback source, guide placement, and visible change.
- **Avoid:** Names, application details, or invented quotations.
- **Caption intent:** Parent feedback added guidance without expanding the tool's core scope.

## Verification and confidentiality

- Confirm the five people completed meaningful use, and document whether sessions were self-directed, facilitated, or mixed.
- Preserve the original wording or a faithful anonymized paraphrase of the two positioning requests.
- Verify the dimensions and jurisdictions the checker supports before naming any standard.
- Do not claim that applications or printed photos were accepted unless there is a receipt.
- Use a consented or synthetic source photo in visuals; obscure names, faces, filenames, and application details where needed.
- Treat all current project claims as author-reported until product, repository, analytics, or feedback receipts are inspected.
