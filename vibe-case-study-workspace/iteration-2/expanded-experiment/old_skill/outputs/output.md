# Pre-draft decision package

**Recommended archetype:** Product Experiment  
**Confidence:** High. The case contains a specific interaction question, three competing models, production-like builds on two platforms, device-test evidence, and a documented selection.  
**Alternative:** Workflow / System could frame the requirements-check assistant, but it is secondary and lacks evidence of repeated external use.  
**Product question:** Which scheduling model would let subscribers compose a message and understand its send state across iOS and Android once permission, keyboard, and background-state behavior became real?  
**Primary constraint:** Static Figma screens could not reproduce the operating-system behavior that shaped the flow.  
**Story thesis:** By testing three subscriber-scheduling models in production-like iOS and Android environments, I found that a calendar-first structure broke down under real device behavior and selected a conversational composer with explicit send-state confirmation; the same work also revealed a requirements-review bottleneck and prompted a small checking assistant.

**Length options:**

- Compact — 400–500: would preserve the pivot but compress the cross-platform and review-workflow evidence.
- Standard — 500–600: could carry the main product decision, with little room for the assistant spin-off.
- Expanded — 700–800: selected; justified by two platforms, three alternatives, several system constraints, a consequential rejection, and a separate workflow consequence.

**Recommended length:** Expanded.  
**Observed evidence:** None independently inspected for this response.  
**Author-reported evidence:** Production-like iOS and Android prototypes; three tested scheduling models; permission, keyboard, and background-state findings; rejection of calendar-first; selection of a conversational composer with explicit send-state confirmation; review decisions; device tests; a requirements-check assistant.  
**Missing evidence:** Exact third model; participants and test protocol; platform-specific findings; decision-maker roles; assistant inputs, outputs, and verified effect; AI contribution; launch, adoption, and return-use data.  
**Relevant source patterns:** MX-03 Production context reveals design constraints; MX-02 Feedback visibly changes the next version; MX-12 One artifact earns a broader belief.  
**Adapted candidate statements:**

- Building the flow on both mobile platforms exposed permission, keyboard, and background-state constraints, changing the selected interaction model. — **Author-reported**
- Device-test evidence led the team to reject calendar-first scheduling and choose a conversational composer with explicit confirmation. — **Author-reported**
- Real-state prototypes are decision instruments when system behavior is part of the experience. — **Author-reported insight**

**Proof-block specifications:** See production notes below.  
**Visual receipts required:** Same-state comparison of all three models; iOS and Android device-test captures; calendar-first failure annotations; selected composer and confirmation sequence; review-decision excerpt; requirements-check assistant input/output.  
**Claims to avoid or qualify:** No launch, adoption, retention, conversion, time-saved, or user-value claims. Do not describe stakeholder review as user validation, prototype behavior as production behavior, or the assistant as adopted or effective without separate evidence.

---

# Scheduling that survives the operating system

I designed a cross-platform scheduling flow for subscribers. The central question was whether people could compose a message, move through system interruptions, and still understand what would be sent and when.

Static Figma screens could describe the intended path. They could not reveal what happened when the keyboard covered an action, a permission request interrupted the sequence, or the app moved into the background. To make the interaction itself testable, I built production-like prototypes for iOS and Android and used them to compare three scheduling models on devices.

> **Constraint**
> **Permission, keyboard, and background-state behavior were part of the design problem.**
> The decision required working flows on both mobile platforms, not isolated screens.

## Phase 1 — Turning fidelity into a product question

The first prototype established a shared test: could a subscriber move from writing to scheduling without losing context or confidence? I implemented enough of the surrounding environment for operating-system behavior to appear during the flow. This shifted review from “Which layout feels clearest?” to “Which model remains understandable when the device changes the path?”

That distinction mattered across platforms. iOS and Android could express the same product intent while producing different transitions around permissions, keyboard dismissal, and backgrounding. The prototypes made those transitions inspectable.

## Phase 2 — Comparing three models under the same conditions

I tested three scheduling models in comparable environments. They represented different ways to organize the subscriber’s task. The most consequential contrast was between a calendar-first direction and a conversational composer.

Calendar-first made the scheduling object prominent at the beginning. On a static screen, that structure appeared direct. On devices, however, the interaction had to absorb composition, system interruptions, and state recovery. Device testing showed that leading with the calendar did not provide a strong enough thread through those transitions.

The conversational model started from the message being created and introduced scheduling within that context. This kept the subscriber’s intent visible while the interface handled platform behavior around it.

> **Influence**
> **Device testing changed the selected model.**
> The calendar-first direction was rejected; the conversational composer moved forward.

## Phase 3 — Making the send state explicit

Selecting the composer solved the structural question, but it introduced a trust question: after scheduling, what exactly had happened? The final system state could still be ambiguous.

I added explicit send-state confirmation so the flow did not rely on a dismissed sheet, a changed button, or a user remembering the chosen time. The confirmation made the transition from draft to scheduled message legible inside the experience. This was a product decision, not decorative feedback: the interface needed to distinguish an intention to schedule from a message that had actually entered a scheduled state.

> **Insight**
> **A natural composer still needs an explicit contract with the system.**
> Conversation organized the task; confirmation made the resulting state trustworthy.

## Phase 4 — Using coded prototypes as review evidence

The prototypes changed the review. Instead of asking collaborators to imagine keyboard collisions or background recovery, I could show the behavior on both platforms and connect a decision to a visible state. The evidence captured the rejected direction and the reason for choosing the composer.

This work supports a decision claim: production-like testing exposed constraints that changed the flow. It does not yet support a market claim. The selected model was not launched, and I do not have adoption or return-use data.

## Phase 5 — Addressing the bottleneck around the experiment

Building at higher fidelity also exposed a process problem. Requirements review became a bottleneck: the prototypes could surface more states than reviewers could consistently check against the intended behavior. I created a small requirements-check assistant to help compare the work with the requirements before review.

The assistant is a bounded spin-off, not proof that the product succeeded. It shows how the method evolved when richer prototypes created a coordination cost. Its inputs, flagged gaps, and resulting decisions would be needed before claiming improved speed or quality.

## What I would carry forward

This experiment changed how I choose prototype fidelity. When permission, keyboard, and lifecycle behavior can change the interaction model, code is not just a more realistic presentation layer; it is part of the decision method. I would use the same sequence again: define competing behavioral models, run them in the relevant system context, record the states that change the choice, and separate the selected direction from any later claim of adoption.

> **Next signal**
> **Test whether subscribers can recover and verify a scheduled message without assistance.**
> Launch, repeat use, and trust outcomes remain unmeasured.

---

# Production notes

## Evidence map and claim verification

All project facts in the draft are **Author-reported** because the underlying receipts were not independently inspected for this response. Before publication, link each claim to the relevant device recording, build, review excerpt, or decision artifact. If a receipt contradicts the prose, revise the claim rather than broadening the interpretation.

Confirm before publishing:

1. Name and behavioral hypothesis of the third scheduling model.
2. Who participated in device testing, what tasks they attempted, and whether they were users, collaborators, or stakeholders.
3. The specific iOS and Android observations behind the calendar-first rejection.
4. Who made or approved the final selection.
5. Whether “production-like” means production code, a local app shell, realistic integrations, or another environment.
6. Whether the requirements-check assistant used AI, rules, or both; what the author and any collaborators each owned.

## Proof blocks

### PB-01

- **Type:** Constraint
- **Statement:** Permission, keyboard, and background-state behavior were part of the design problem.
- **Optional qualifier:** Working flows were built for iOS and Android.
- **Evidence status:** Author-reported
- **Evidence ID:** EV-DEVICE-CROSS-PLATFORM
- **Intended placement:** Opening orientation
- **Originating source pattern:** MX-03

### PB-02

- **Type:** Influence
- **Statement:** Device testing changed the selected model.
- **Optional qualifier:** Calendar-first was rejected and the conversational composer moved forward.
- **Evidence status:** Author-reported
- **Evidence ID:** EV-DECISION-REVIEW
- **Intended placement:** After the alternatives comparison
- **Originating source pattern:** MX-02

### PB-03

- **Type:** Insight
- **Statement:** A natural composer still needs an explicit contract with the system.
- **Optional qualifier:** Conversation organized the task; confirmation made the resulting state legible.
- **Evidence status:** Author-reported
- **Evidence ID:** EV-SEND-STATE
- **Intended placement:** After the confirmation decision
- **Originating source pattern:** MX-12

### PB-04

- **Type:** Next signal
- **Statement:** Test whether subscribers can recover and verify a scheduled message without assistance.
- **Optional qualifier:** Launch, repeat use, and trust outcomes remain unmeasured.
- **Evidence status:** Hypothesis
- **Evidence ID:** NEXT-VALIDATION-01
- **Intended placement:** Conclusion
- **Originating source pattern:** none

## Capture plan

1. **Bet and constraint:** One diagram connecting composition, permission, keyboard, backgrounding, and confirmation.
2. **Comparable directions:** All three models at the same scale and equivalent point in the task; annotate behavioral differences.
3. **Real-state evidence:** Paired iOS and Android recordings showing the decisive states.
4. **Decision receipt:** An anonymized review excerpt beside the calendar-first and conversational comparison.
5. **Selected sequence:** Compose, schedule, interruption or state transition, and explicit confirmation.
6. **Spin-off:** A real requirement input, the assistant's check, and the review decision it informed.

Do not recreate product UI to stand in for a missing receipt. If confidentiality prevents showing an artifact, use a clearly labeled reconstruction that preserves the interaction sequence while removing product names, personal data, message content, dates, and internal identifiers.

## Publication boundary

Safe with receipts: three models were tested; cross-platform device behavior exposed constraints; calendar-first was rejected; the conversational composer with explicit confirmation was selected; a requirements-check assistant was created.

Not yet supported: the selected flow improved comprehension or trust, reduced errors, shipped, gained adoption, saved review time, or improved review quality. Those belong in future updates only after launch analytics, task-based usability evidence, repeated use, or measured review outcomes exist.
