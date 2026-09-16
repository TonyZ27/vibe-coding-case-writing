# Decision package

**Recommended archetype:** Product Experiment

**Confidence:** High. The story contains a specific product uncertainty, three meaningfully different scheduling models, production-like builds on two platforms, decisive device findings, and a documented selection. Workflow / System is a secondary lens for the requirements-check assistant, but it should not displace the scheduling decision.

**Product question:** Which scheduling model helps subscribers compose and trust a future send when mobile permissions, keyboard behavior, and background state affect the experience?

**Primary constraint:** Static Figma screens could not reveal the system behavior that determined whether scheduling felt understandable and dependable on iOS and Android.

**Story thesis:** By testing three subscriber-scheduling models in production-like iOS and Android environments, I learned that calendar-first scheduling did not withstand device testing as well as a conversational composer with explicit send-state confirmation; the same experiment also revealed a review bottleneck worth addressing with a lightweight requirements-check assistant.

**Length options:** Compact (400–500) would force the cross-platform findings and workflow spin-off into captions. Standard (500–600) could carry the main decision but would compress the three-model comparison. Expanded (700–800) is appropriate because the evidence spans two platforms, several system states, three alternatives, one product pivot, and one bounded workflow consequence. Expanded is already selected.

**Observed evidence:** None independently inspected for this response. The brief states that review decisions and device-test evidence exist; those artifacts should be attached before publication.

**Author-reported evidence:** iOS and Android prototypes were built in production-like environments; three scheduling models were tested; permission, keyboard, and background-state behavior were examined; calendar-first was rejected after device testing; a conversational composer with explicit send-state confirmation was selected; coded prototypes exposed a review bottleneck; a small requirements-check assistant was created; no launch or adoption data exists.

**Missing evidence:** Product/team context and stakes; names and behavioral definitions of all three models; exact device findings by platform; participant and decision-maker roles; the review criteria and decision record; the before/after review workflow; the assistant’s inputs, outputs, and actual use; author/AI/engineering division of labor; dates, scope, and confidentiality limits.

**Relevant source patterns:** MX-03, Production context reveals design constraints; MX-02, Feedback visibly changes the next version; MX-12, One artifact earns a broader belief.

**Adapted candidate statements:**

- MX-03 — Building the scheduling flow in production-like iOS and Android environments exposed permission, keyboard, and background-state behavior that static screens hid, changing the selected interaction model. **Status: Author-reported.**
- MX-02 — Device-test and review evidence led to rejecting calendar-first scheduling and selecting a conversational composer with explicit send-state confirmation. **Status: Author-reported.**
- MX-12 — For stateful mobile interactions, implementation fidelity is part of design reasoning when system behavior can determine a concept decision. **Status: Author-reported bounded lesson.**

**Primary proof-statement specification:** Use the device-driven decision as the sole proof statement. Evidence status: Author-reported. Evidence IDs: DT-01 iOS device-test capture, DT-02 Android device-test capture, RD-01 scheduling-model review decision. Placement: after the selected-direction section. Originating source pattern: MX-03. Visual intent: full-width tinted callout; large text; one inline bold phrase; no visible label.

**Visual receipts required:** Same-state comparison of the three models; iOS and Android device captures showing permission, keyboard, and background-state behavior; annotated calendar-first failure sequence; selected composer and explicit send-state sequence; anonymized review decision; review bottleneck before-flow; assistant input/output example.

**Claims to avoid or qualify:** Do not claim launch, adoption, retention, conversion, subscriber preference, usability validation, production release, team-wide efficiency, or review-time reduction. Do not call stakeholder review user validation. Do not imply the assistant was reused or adopted unless a receipt shows it.

---

# Designing Scheduling Where Static Screens Couldn’t Reach

I designed and built a cross-platform scheduling experiment to answer a deceptively simple question: how should a subscriber prepare a message now and trust that it will be sent later? The difficult part was not drawing a date picker. It was understanding how scheduling behaved when permissions, the mobile keyboard, app backgrounding, and send state all entered the same flow.

## At a glance

I built production-like prototypes for iOS and Android, compared three scheduling models on devices, rejected a calendar-first direction, and selected a conversational composer with explicit send-state confirmation. The work produced a product decision and a lightweight requirements-check assistant for a review problem exposed during the experiment. The concept was not launched, so this case makes no adoption or business-impact claim.

## The question hidden by polished screens

Static Figma flows made each direction look coherent. They could show the intended sequence, but not the moments where the operating system became part of the experience: a permission request interrupting intent, a keyboard compressing the available controls, or a scheduled action becoming ambiguous after the app moved into the background.

Those were not implementation details to resolve after selection. They could change which concept deserved to be selected. I therefore treated working code as an experimental medium and built the key states inside production-like iOS and Android environments.

## Three models, three different bets

I tested three scheduling models rather than three visual treatments. Each represented a different idea about how subscribers would understand future sending.

The set included a calendar-first direction, a conversational composer, and a third scheduling model documented in the comparison artifacts. The conversational direction kept the message as the primary object and introduced scheduling within the act of composing. I compared the models in equivalent states so review could focus on behavior: where intent began, what interrupted it, and how the interface communicated what would happen next.

This distinction mattered. A gallery of attractive options would only ask which screen looked clearest. The prototypes asked which mental model survived contact with the device.

## Device testing changed the decision

Calendar-first gave future time a familiar visual structure, but static screens could not show whether that structure would remain coherent as system behavior entered the flow. On devices, permission moments, keyboard transitions, and background-state changes changed the comparison enough for me to reject that direction.

I selected the conversational composer with an explicit confirmation state. The intended logic kept composition central while distinguishing between a message being drafted, a schedule being confirmed, and the next state in the flow. The exact platform-specific findings should sit beside this claim in the published case rather than being reconstructed from incomplete context.

I rejected calendar-first and selected the conversational direction. This was not a preference decision dressed up as validation. It was a bounded product decision based on how the alternatives behaved in the states the final experience would have to survive.

> The most important result was not producing three polished prototypes. It was that **device behavior determined the decision**: testing gave the team a concrete basis for rejecting calendar-first scheduling and selecting a composer with explicit send-state confirmation.

## The experiment also changed the review workflow

Building at higher fidelity improved the decision, but it also exposed a bottleneck. Reviews now had more states, platform differences, and requirements to reconcile. The coded prototypes could reveal a missing condition, yet reviewers still needed a reliable way to check whether the evidence covered the intended requirements.

I created a small requirements-check assistant to support that step. Its role was narrow: help connect a reviewable flow to the requirements that needed confirmation. It did not replace the product decision or automate design judgment. The assistant emerged because the experiment made a coordination gap visible.

## What this changed in my practice

This project changed where I place fidelity in the design process. For stateful mobile interactions, code is not simply the final representation of an already-settled idea. When operating-system behavior can alter comprehension or trust, a production-like build becomes part of deciding what the product should be.

The transferable method is straightforward: define alternatives as behavioral hypotheses, test them in the smallest environment that exposes consequential states, and record the decision against those states. Then inspect the review process itself for friction created by the richer evidence.

The next proof is deliberately still open. A launch would need to test whether subscribers understand scheduled state without assistance, recover from permission or background interruptions, and return to manage future sends. Until then, the supported outcome is a stronger design decision—not adoption.

---

# Production notes

## Evidence register

| ID | Requested receipt | Supports | Status before receipt |
| --- | --- | --- | --- |
| DT-01 | iOS device recording with permission, keyboard, and background transitions | Real-state constraint and decision | Author-reported |
| DT-02 | Android device recording of equivalent states | Cross-platform comparison | Author-reported |
| ALT-01 | Same-scale capture of all three scheduling models in the same task state | Meaningful alternatives | Author-reported |
| RD-01 | Anonymized review note, decision log, or marked comparison | Rejection and selection | Author-reported |
| SC-01 | Selected composer sequence through explicit send-state confirmation | Final interaction logic | Author-reported |
| RB-01 | Review artifact showing the requirements bottleneck | System spin-off trigger | Author-reported |
| RA-01 | Requirements-check assistant input/output example | Spin-off existence and scope | Author-reported |

## Primary proof statement

Role: Primary proof statement  
Statement: The most important result was not producing three polished prototypes. It was that device behavior determined the decision: testing gave the team a concrete basis for rejecting calendar-first scheduling and selecting a composer with explicit send-state confirmation.  
Inline emphasis: device behavior determined the decision  
Evidence status: Author-reported  
Evidence IDs: DT-01, DT-02, RD-01  
Intended placement: After “Device testing changed the decision”  
Originating source pattern: MX-03  
Visual intent: full-width tinted callout; large text; one inline bold phrase; no visible label

## Capture and layout plan

1. Open with a compact annotated diagram of the product question and the system states static screens omitted.
2. Show the three directions at the same scale and same point in the scheduling task; annotate behavioral hypotheses, not visual styling.
3. Pair iOS and Android clips by state: permission, keyboard, background/resume.
4. Place the calendar-first breakdown immediately beside the rejection rationale.
5. Follow with the selected composer and confirmation sequence, then RD-01 near the proof statement.
6. Keep the requirements-check assistant to one before-flow and one input/output example so it remains subordinate to the product experiment.

## Verification and confidentiality

- Confirm whether “production-like” means a production codebase, production components, realistic service/state behavior, or only native platform shells; use the precise term in publication.
- Name who participated in device testing and who made the final decision. If these were internal reviews, describe them as reviews, not user tests.
- Confirm that the three models differed behaviorally as summarized. Replace the generic second-model description with its actual name and hypothesis.
- Attribute engineering and AI contributions explicitly. The current brief supports first-person ownership of building and deciding, but not a detailed division of labor.
- Anonymize subscriber data, internal requirements, names, roadmap details, and message content in every receipt.
- Keep the requirements-check assistant’s claims at output level until there is evidence of use, changed review behavior, or measured review performance.

## Publication gate

Before publishing, attach DT-01, DT-02, ALT-01, RD-01, and SC-01; reconcile the prose with those artifacts; confirm participant and ownership language; and re-count the reader-facing article at 700–800 words. If the receipts do not support the stated reversal, demote the proof statement to an ordinary design lesson and revise the case around the narrower constraint finding.
