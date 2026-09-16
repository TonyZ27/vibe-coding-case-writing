# A simpler way for parents to make printable passport photos

After paying for an overcomplicated passport-photo service while preparing my child’s application, I built a focused utility for the task I actually needed: turn a photo into a correctly sized, printable sheet without navigating an oversized service.

## At a glance

**What:** A working passport-photo utility for parents.  
**Core flow:** Upload a photo, crop it, validate its dimensions, and download a printable sheet.  
**My role:** I framed the product and interactions, directed an AI coding agent, tested the result with real photos, and corrected the crop behavior.  
**Response:** Five parents used the product; feedback from two of them shaped v2.

## Starting with the job, not the service

The trigger was personal and immediate. I was preparing my child’s application, but the service I paid for made a narrow task feel needlessly complicated. That experience gave me a clear product boundary: this did not need to become a broad photo editor or application platform. It needed to help a parent move from an existing photo to a printable output.

I reduced the experience to four connected actions: upload, crop, validate dimensions, and download. Each step answered a practical question in sequence: Is this the right photo? Is the subject framed correctly? Does the output have the required dimensions? Can I print it now?

> **Insight**  
> **The minimum useful product was one complete task, not more photo-editing features.**

## Correcting the crop where the design met real photos

I framed the flow and interaction behavior, then an AI coding agent implemented the image-processing path. The first working build made the idea tangible, but testing it with real photos exposed a gap in the crop behavior. A technically functioning crop was not enough if it made positioning the subject difficult or produced an unexpected result.

I manually corrected that behavior after testing. This became the clearest human–AI boundary in the project: the agent could assemble the processing flow, while I remained responsible for judging whether the interaction behaved predictably with the material people would actually use.

> **Insight**  
> **A working image pipeline still required hands-on interaction judgment.**

## Five uses led to one focused v2 change

Five parents used the utility. Two asked for help positioning a child within the photo, pointing to uncertainty that dimension validation alone did not resolve. In v2, I added a child-photo positioning guide so parents could make a better framing decision while cropping, before reaching the final sheet.

That request did not justify expanding the product in every direction. It revealed one missing piece inside the existing task: parents needed guidance before they needed validation. The change strengthened the original flow instead of turning the utility into a larger service.

> **Influence**  
> **2 of 5 parent users requested positioning help, leading to the v2 guide.**

## What I took forward

This project changed how I use AI coding agents in product work. Framing the task precisely helped the agent build a complete flow quickly, but real inputs were what exposed the important interaction flaw. My role was not finished when the implementation ran; it shifted to testing behavior, correcting the boundary cases I could see, and deciding which feedback belonged in the product.

The lesson was deliberately small: for rules-heavy utilities, reduce the journey to a complete task, then use real material and real requests to decide where guidance is more valuable than another feature.

---

## Production notes

### Editorial decision

- **Recommended format:** Product Utility
- **Confidence:** High
- **Alternative format:** Practice Note, only if the working flow or parent-use claims cannot be evidenced publicly
- **Story Thesis:** By focusing on a parent preparing a child’s application, I reduced a needlessly complicated photo task to one guided flow, showing that small utilities become useful through clear boundaries and targeted guidance.
- **Selected length:** Compact, as provided by the author; the story has one clear arc, one detailed interaction correction, and one feedback-led v2 change.
- **Selected narrative modules:** Minimum Useful Scope; AI Collaboration; v1 → v2

### Evidence map

- **Observed:** None independently inspected for this draft.
- **Author-reported:** The paid-service trigger; the working upload, crop, dimension-validation, and printable-sheet flow; five parent users; two requests for a child-photo positioning guide; the v2 addition; the division of work between the author and AI coding agent; manual correction of crop behavior after testing real photos.
- **Inferred:** The existing service contained more scope than this task required. The draft keeps this qualitative and does not claim specific steps, cost savings, speed gains, or compliance outcomes.
- **Missing context:** Whether use was self-serve or facilitated; exact passport standard or country; what specifically failed in the original crop behavior; what was deliberately excluded from v1; dates, URL, screenshots, and anonymized feedback receipts.

### Visual evidence plan and capture requests

1. **Product overview**
   - Claim supported: The utility provides one complete parent task.
   - Asset filename: `passport-photo-final-flow.png`
   - Capture: Final interface showing the flow from upload through printable output.
   - Must show: Real product UI and the four core capabilities.
   - Avoid: Generated replacement UI or personal application data.

2. **Core-task demo**
   - Claim supported: A parent can upload, crop, validate dimensions, and download a printable sheet.
   - Asset filename: `passport-photo-core-flow.mp4`
   - Capture: An 8–12 second recording of the complete task using a consented or synthetic photo.
   - Must show: State changes and downloaded sheet.
   - Avoid: A real child’s identifiable photo without explicit permission.

3. **Crop correction comparison**
   - Claim supported: Real-photo testing led to a manual interaction correction.
   - Asset filename: `crop-behavior-v1-v2.png`
   - Capture: Side-by-side v1 and corrected behavior with annotations naming the specific issue.
   - Must show: The same test photo and the changed crop result or control behavior.
   - Avoid: Claiming the correction improved success rate unless measured.

4. **Feedback-to-v2 receipt**
   - Claim supported: Two parent requests led to the positioning guide.
   - Asset filename: `positioning-feedback-and-v2.png`
   - Capture: An anonymized feedback excerpt paired with the implemented guide.
   - Must show: The request and inspectable v2 change.
   - Avoid: Names, profile photos, contact details, or wording that implies a broader study.

### Claims to verify, soften, or avoid

- Verify the count of five users and two guide requests before publication.
- Describe the five uses as facilitated trials if the parents required the author’s help; do not imply self-serve adoption unless confirmed.
- Say the tool validates dimensions, not that it guarantees passport acceptance or compliance with every jurisdiction.
- Do not claim time or cost savings without a documented comparison.
- Do not describe the crop correction as AI failure unless the original output and causal diagnosis can be shown.
- The outline uses the source-library patterns “Personal constraint sharpens scope,” “Feedback visibly changes v2,” and “Human-AI handoff beats full automation.”
