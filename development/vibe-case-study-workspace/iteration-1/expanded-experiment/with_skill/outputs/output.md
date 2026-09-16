# Direction decision

**Recommended archetype:** Product Experiment  
**Confidence:** High  
**Selected length:** Expanded, 700–800 words of reader-facing copy  
**Product question:** Which scheduling model would preserve subscriber confidence across iOS and Android when permissions, keyboards, and background transitions became part of the experience?  
**Primary constraint:** Static Figma screens could show layout but not the system behavior that determined whether scheduling felt trustworthy.  
**Story thesis:** By testing three scheduling models in production-like iOS and Android environments, I learned that explicit state continuity mattered more than calendar-led organization, changing both the product direction and the way requirements were reviewed.

**Observed evidence:** No project artifacts were independently inspected for this draft.  
**Author-reported evidence:** Working iOS and Android prototypes; three scheduling models; device tests covering permission, keyboard, and background-state behavior; rejection of the calendar-first direction; selection of a conversational composer with explicit send-state confirmation; review-decision receipts; and a requirements-check assistant created after the prototypes exposed a review bottleneck.  
**Missing evidence:** The third model’s interaction logic; test participants and protocol; exact review criteria and decision owners; collaborator and AI roles; assistant inputs, outputs, and actual use; launch status; adoption; and behavioral outcomes.  
**Relevant source patterns:** MX-03, production context reveals design constraints; MX-12, one artifact earns a broader belief.  
**Adapted candidate statements:** “Building the scheduling flow on both platforms exposed state transitions that changed the selected interaction model” — **Author-reported**. “For stateful mobile interactions, fidelity should be chosen by the uncertainty the team needs to resolve” — **Author-reported insight**.  
**Directions worth showing:** All three models at the same task and state; identify the unnamed third model before publication.  
**Decision evidence:** Device-test captures paired with the review record that documents why calendar-first was rejected and the conversational composer selected.  
**Claims to avoid or qualify:** Do not call the work launched, adopted, production-validated, or proven to improve completion, trust, or review speed. Do not describe stakeholder review as user validation.

---

# Designing scheduling around state, not the calendar

I designed a cross-platform scheduling flow by testing three interaction models inside production-like iOS and Android environments. The work shifted from a calendar-first experience to a conversational composer with explicit send-state confirmation.

This was a design decision, not a launch result. The evidence shows what the prototypes revealed and which direction reviewers selected; it does not yet show adoption or behavior after release.

> **Constraint**
> **Static screens could not reveal the states that determined trust.**
> Permissions, keyboards, and background transitions had to be experienced on-device.

## The real question lived between the screens

At first, scheduling appeared to be an interface-organization problem: choose content, set a time, and confirm. Figma could represent each moment, but not answer the consequential questions. What happened when a permission interrupted the flow? Would the keyboard obscure the next action? After leaving and returning, would the scheduled state remain legible?

Those transitions were not edge decoration. They shaped whether a subscriber could understand the commitment they had made. I therefore treated prototype fidelity as part of the research method and built both platform versions far enough inside production-like environments to encounter native behavior.

*[Visual 1: Bet-and-constraint diagram connecting the scheduling question to permission, keyboard, and background states.]*

## Three models, one comparable task

I tested three scheduling models against the same task. One made the calendar the primary surface. Another kept scheduling inside a conversational composer. The third should be named in the final publication once its interaction logic is documented.

The point of the comparison was not visual variety. Each model proposed a different answer to where subscribers should form intent and where the product should confirm it. Keeping the task and state consistent made the behavioral trade-offs visible across platforms.

*[Visual 2: The three directions at the same scale and task state, annotated by the product question each tested.]*

## Device behavior changed the decision

On-device testing exposed what the static sequence had hidden. Permission prompts could break the apparent continuity of the task. Keyboard behavior changed the usable space and action hierarchy. Moving the app into the background introduced a gap between scheduling something and feeling certain that it remained scheduled.

These findings weakened the calendar-first direction. It gave time selection a strong visual home, but it separated the scheduling decision from the composition context and made continuity harder to communicate through interruptions.

The conversational composer kept intent, content, and timing closer together. I selected it with an explicit send-state confirmation so the subscriber could see not only that an action had been accepted, but also what the system now believed would happen.

> **Influence**
> **Device tests moved the product away from calendar-first scheduling.**
> The selected composer preserved context and made the committed send state explicit.

*[Visual 3: Calendar-first and composer directions shown before and after an interruption.]*

*[Visual 4: Final cross-platform sequence from composition through explicit send-state confirmation.]*

## The prototype also revealed a review problem

The coded flows also revealed a bottleneck: checking whether each build still covered the intended requirements had become a separate task. I created a small requirements-check assistant to compare the evolving experience against the expected flow and surface gaps.

This assistant is a spin-off, not evidence of product adoption. Its relevance is narrower: building at higher fidelity created more inspectable behavior, which in turn required a more structured way to review that behavior. The case should show the assistant’s actual input and output before claiming that it saved time or changed team performance.

> **Insight**
> **Higher-fidelity prototypes need higher-fidelity review.**
> More realistic behavior creates better decisions only when requirements remain traceable.

*[Visual 5: An anonymized requirement, the corresponding prototype state, and the assistant’s review output.]*

## What this experiment established—and what remains open

The experiment established a direction: a conversational composer with explicit confirmation was selected over the calendar-first model after cross-platform device testing. Review records and device-test receipts can substantiate that decision. They should appear beside the comparison rather than as an unsupported outcome statement.

The work did not establish that subscribers complete scheduling more often, trust it more, or return to use it. Those questions require launch and behavioral evidence.

> **Next signal**
> **Can subscribers schedule, leave, return, and correctly verify the send state without assistance?**

*[Visual 6: Anonymized review decision linking device evidence to the selected direction.]*

The transferable lesson is bounded but useful: for stateful mobile interactions, choose prototype fidelity according to the uncertainty that must be resolved. When the decision depends on operating-system behavior and continuity across interruptions, the experience between screens is part of the product—not implementation detail.

---

# Production notes

## Evidence and capture requests

1. **Bet and constraint** — Create a compact, clearly labeled reconstruction of the initial decision question. Do not invent research inputs.
2. **Comparable directions** — Capture all three models at the same scale, platform, task, and state. Add the third model’s verified name and behavioral hypothesis.
3. **Device-test receipt** — Use an original video or frame sequence showing at least one permission interruption, keyboard collision or resize, and background/return state. Identify platform and build version.
4. **Selected flow** — Capture both iOS and Android from composition through explicit send-state confirmation. Avoid implying pixel parity if native behavior differs.
5. **Review decision** — Anonymize names and sensitive product details while preserving date, decision, rationale, and connection to device evidence.
6. **Requirements-check assistant** — Show one real requirement, its checked prototype state, and the resulting output. Do not claim time savings without comparative evidence.

## Proof-block specifications

### Block 1

- **Type:** Constraint
- **Statement:** Static screens could not reveal the states that determined trust.
- **Optional qualifier:** Permissions, keyboards, and background transitions had to be experienced on-device.
- **Evidence status:** Author-reported
- **Evidence ID:** E1 — cross-platform device-test capture
- **Intended placement:** After the opening orientation
- **Originating source pattern:** MX-03

### Block 2

- **Type:** Influence
- **Statement:** Device tests moved the product away from calendar-first scheduling.
- **Optional qualifier:** The selected composer preserved context and made the committed send state explicit.
- **Evidence status:** Author-reported
- **Evidence ID:** E2 — device-test comparison plus review decision
- **Intended placement:** After the decision explanation
- **Originating source pattern:** MX-03

### Block 3

- **Type:** Insight
- **Statement:** Higher-fidelity prototypes need higher-fidelity review.
- **Optional qualifier:** More realistic behavior creates better decisions only when requirements remain traceable.
- **Evidence status:** Author-reported
- **Evidence ID:** E3 — requirements-check assistant input/output
- **Intended placement:** In the system spin-off section
- **Originating source pattern:** MX-12

### Block 4

- **Type:** Next signal
- **Statement:** Can subscribers schedule, leave, return, and correctly verify the send state without assistance?
- **Optional qualifier:** None
- **Evidence status:** Hypothesis
- **Evidence ID:** H1 — proposed post-launch validation question
- **Intended placement:** In the limitations section
- **Originating source pattern:** none

## Verification and confidentiality

- Confirm the third model, test protocol, reviewer roles, and decision date before publication.
- Replace broad references to “subscribers” with the verified audience definition if the product serves a narrower segment.
- Confirm whether “production-like” means production code, a debug build, realistic services, or only native-device execution; use the most precise supported term.
- Obtain permission or anonymize all review excerpts, account data, notification content, and internal requirements.
- Keep the assistant claim at artifact level until there is evidence of repeated use, independent use, or measurable review improvement.
- Recheck that no caption or proof block implies launch, adoption, user validation, or improved trust.
