# Decision package

Recommended format: Product Experiment

Confidence: High. The case contains a specific interaction question, three competing models, production-like prototypes on two platforms, device-test evidence, a rejected direction, and a documented selection. It does not contain launch or adoption evidence.

Alternative format: Workflow / System could become a separate, shorter case if the requirements-check assistant later has evidence of repeated use beyond the author. At present, it is best treated as a supporting spin-off.

Story Thesis: By testing subscriber scheduling inside production-like iOS and Android environments, I learned that the strongest model was not the one that organized time most visibly, but the one that kept composition primary and made the final send state unmistakable.

Observed evidence: None was directly inspected for this response.

Author-reported evidence: iOS and Android coded prototypes; three scheduling models; device tests covering permission, keyboard, and background-state behavior; rejection of a calendar-first direction; selection of a conversational composer with explicit send-state confirmation; review decisions; and a small requirements-check assistant prompted by review friction.

Missing context: Product and team setting; exact subscriber use case; names and behavior of all three models; participant count and test protocol; exact device findings by platform; decision-makers and collaborators; engineering and AI division of labor; requirements-assistant inputs and outputs; dates; and anonymizable source artifacts.

Recommended length: Expanded, interpreted as the skill's Extended mode of 1,300–1,800 reader-facing words, because the user has already selected it. The material can support that length if the final publication includes the reported comparison, device-state receipts, and review evidence.

Length rationale: The case spans two platforms, three alternatives, several system states, a consequential rejection, and a workflow spin-off. The long format is justified by decision depth, not by prototype volume.

Length options for user selection: Compact — 450–650 words for the calendar-first rejection alone. Standard — 800–1,100 words for the main product decision without much workflow detail. Expanded / Extended — 1,300–1,800 words, selected, to preserve the cross-platform experiments, decision logic, and bounded system spin-off.

Selected narrative modules: The Bet; Why Existing Fidelity Was Insufficient; Competing Directions; Real-State Validation; Decision Moment; System Spin-Off.

Candidate proof blocks: Static screens could not expose operating-system behavior; three models were tested in working flows; device testing reversed the calendar-first direction; explicit send-state confirmation became part of the selected model; review friction produced a requirements-check assistant.

Visual Evidence Plan: An annotated map of permission, keyboard, and background states; the three models at the same scale and task state; paired iOS and Android device captures; calendar-first failure evidence; selected composer and confirmation sequence; review-decision receipt; requirements-assistant input/output example.

Claims to avoid or soften: Do not claim launch, adoption, conversion, retention, time savings, user validation, production release, or organizational impact. Do not describe stakeholder review as subscriber validation. Do not claim the assistant improved review speed or quality without measured or documented evidence. Do not name AI tools or describe an AI working method without a concrete, verifiable episode.

---

# Scheduling is not a calendar problem

## Testing a subscriber scheduling flow where static screens stopped being truthful

I was designing a cross-platform flow for scheduling messages to subscribers. The apparent task was straightforward: choose what to send, choose when to send it, and confirm the schedule. But the important design questions sat outside the static interface. What happens when the operating system asks for permission? Does the keyboard compress, cover, or interrupt the composer? What does the sender see after the app moves into the background and returns? And at what point does a scheduled message feel committed rather than merely drafted?

Figma could describe the intended path, but it could not answer those questions. I built production-like prototypes for iOS and Android so the scheduling models could be tested inside the states that would determine whether the experience felt dependable.

> **Constraint**
> **The decisive behavior lived between screens.**
> Permission prompts, keyboard transitions, and background-state changes required working device flows.

## At a glance

**What** — A cross-platform experiment for scheduling subscriber messages.

**How** — I implemented three scheduling models in production-like iOS and Android environments, tested them on devices, and used the resulting behavior to guide review.

**Decision** — I rejected a calendar-first direction and selected a conversational composer with explicit confirmation of the final send state.

**Secondary output** — When the prototypes exposed a bottleneck in checking requirements during review, I created a small assistant to make that check more consistent.

**Evidence boundary** — The work produced a reviewed product direction and documented device findings. It did not reach launch, and there is no adoption data.

## The bet: scheduling should fit the act of composing

The experiment began with an unresolved product question: should scheduling be organized around the calendar, or should it remain part of the conversation the sender is already composing?

A calendar-first model offered an obvious advantage. It made time visible and gave the schedule a familiar structure. That clarity was attractive in static review because a reviewer could immediately see dates, slots, and planned sends. But it also risked changing the center of gravity of the task. The user was not arriving primarily to manage a calendar; they were trying to prepare a message for subscribers and decide when it should go out.

I tested three models rather than treating that framing as settled. The alternatives were useful only if they represented different product behavior, so I compared them as complete flows rather than as isolated screen treatments. Each had to carry the sender from composition through timing and into a legible final state.

> **Experiment**
> **Three scheduling models were implemented as working flows.**
> The comparison focused on how each model connected composing, choosing a time, and understanding what would happen next.

## Raising fidelity to expose the real interaction

The coded prototypes were not an exercise in making polished mockups. They were test instruments. Their purpose was to reveal behavior that the design file could only imply.

Permission was one of those behaviors. A system prompt can interrupt the designed sequence, change what the user believes has been completed, or return them to a state the static happy path never shows. The keyboard created another set of constraints. In a scheduling flow, composition and timing controls compete for limited space, especially when the sender is editing content and adjusting delivery details in the same session. Backgrounding added a third question: after leaving and returning to the app, would the sender still understand whether the message was a draft, scheduled, or awaiting confirmation?

Building both iOS and Android versions made those transitions part of the design material. It also prevented a single platform's behavior from being mistaken for the universal interaction. Instead of reviewing only the intended sequence, I could bring the actual interruptions, layout changes, and resumed states into the decision.

This changed the role of the prototype. It was no longer a presentation of a preferred answer. It became a way to discover which answer remained coherent when the operating system participated in the flow.

## The device test that changed the direction

On a static canvas, the calendar-first direction looked structured and reassuring. On devices, that structure came with a cost: it made the act of choosing a date feel like the primary task and pushed the message—the thing being scheduled—into a supporting role.

That trade-off became harder to ignore once the flow had to accommodate the keyboard, system permissions, and returning from the background. These states did not merely add edge cases around the calendar. They made continuity more important. The sender needed to retain a clear sense of the message they were composing, the timing attached to it, and whether the action had actually been committed.

The device tests therefore changed the decision. I rejected the calendar-first direction, not because calendars are unfamiliar, but because its hierarchy did not hold up under the full cross-platform task. Familiarity at the control level was not enough if the overall flow made the user's object of attention less stable.

> **Decision**
> **Device testing reversed the calendar-first direction.**
> Its visible time structure could not compensate for the loss of continuity around the message being composed.

This was the point of using production-like environments: the selected direction was not simply the one that looked clearest in a review frame. It was the one that remained understandable through the states the real product would have to survive.

## Keeping the conversation primary

The selected model used a conversational composer as the main surface. Scheduling became part of preparing the message rather than a separate planning destination. This preserved the relationship between content and timing: the sender could understand what they were sending while deciding when it should be delivered.

That choice created a new responsibility. If the interface stayed conversational, the final scheduled state could not be left implicit. A message that looks ready, queued, or sent can carry very different consequences. The flow therefore included explicit send-state confirmation so the sender could distinguish composing from commitment and see what the system believed would happen next.

This confirmation was not decorative reassurance added at the end. It completed the interaction model. The conversational composer protected continuity during preparation; the explicit final state protected certainty after the scheduling action. Together, they answered the two parts of the original question: where scheduling belonged and how commitment should be communicated.

> **Insight**
> **Preserve continuity while composing; become explicit at commitment.**
> The selected model kept the message central and made the scheduled send state unmistakable.

## A prototype can also reveal a review problem

The coded experiments surfaced a second bottleneck: reviewing realistic flows required repeatedly checking whether each direction covered the agreed requirements and critical states. As the number of platform conditions and alternatives grew, that check became a small workflow of its own.

I created a requirements-check assistant to support that review. Its role was narrow: help compare the prototype against the requirements that mattered to the decision. It did not make the product choice, replace device testing, or turn subjective judgment into an automated score. The product decision still depended on seeing the flow on devices and weighing the trade-offs.

The assistant belongs in this case because it emerged directly from the experiment. Building at higher fidelity increased what the team could learn, but it also increased the review surface. The assistant was a response to that new cost: a lightweight way to keep requirement coverage visible while human reviewers focused on interaction quality and product fit.

> **Workflow spin-off**
> **Higher-fidelity experiments created a new review surface.**
> A small assistant helped check requirement coverage; documented review decisions remained the source of product judgment.

There is evidence that the assistant and review process were used for this project. Without evidence of repeated use, measured review improvement, or adoption by others, I treat it as a project output rather than a proven team system.

## What the experiment resolved

The work resolved a product direction before launch. Three models were tested in working cross-platform flows. The calendar-first direction was rejected after device testing. A conversational composer with explicit send-state confirmation was selected, and the review decisions and device tests provide receipts for that choice.

The experiment did not establish whether subscribers or senders would adopt the feature, whether scheduling would improve engagement, or whether the selected flow would perform better in market. Those questions require launch or subsequent behavioral research. The evidence here supports a narrower—and still consequential—claim: realistic prototyping changed the interaction decision and exposed the system states the final design needed to handle.

## The principle I carried forward

High fidelity is valuable when it answers a question that lower fidelity cannot. In this project, code mattered because the product experience depended on operating-system behavior, physical-device constraints, and state continuity. The implementation was not proof of impact; it was a way to make hidden conditions available to design judgment.

The resulting principle is specific: when a workflow crosses composition, system interruption, and delayed execution, design the continuity first and make commitment explicit. Test that logic in the environments that can break it. Then use tooling to support the review, while keeping the final decision with the people accountable for the product.

---

# Production notes

## Evidence gaps and verification requests

- Replace general device-test language with the exact observed behavior for permission, keyboard, and background states. Record device model, OS version, build, date, task, and observer where available.
- Name and describe the third scheduling model before publication. The public draft truthfully says three models were tested but only contrasts the calendar-first and selected conversational directions because no details for the third were supplied.
- Confirm who selected or approved the final direction and what role the author, product partners, engineers, and any AI tools played.
- Verify that “production-like” is the team's accepted description. Do not upgrade it to “production” or “production-validated.”
- Document the requirements-check assistant's actual inputs, outputs, and use during review. Keep claims limited to project use unless there is evidence of reuse.
- Confirm the object being scheduled is accurately described as a “message to subscribers.” Adjust terminology if the product used posts, notifications, campaigns, or another content type.

## Capture requests

1. One annotated state map showing composition, scheduling, confirmation, permission interruption, keyboard-open state, backgrounding, and return.
2. The three scheduling models at the same device scale and equivalent task state, with one sentence identifying the product question each tested.
3. Paired iOS and Android captures of the same critical transition.
4. A short device recording of the calendar-first failure point and the selected composer's corresponding behavior.
5. A review receipt showing the rejection and selection rationale; redact names or internal links as needed.
6. The explicit send-state confirmation sequence, including the state after returning from the background.
7. One real, redacted requirements-assistant input/output pair next to the requirement it checked.

## Confidentiality guidance

Anonymize subscriber data, message content, account identifiers, internal product names, unreleased dates, employee names, repository paths, and review-channel metadata. Preserve timestamps only when they are necessary to establish sequence. Prefer redaction of authentic artifacts over reconstructed UI. If reconstruction is unavoidable, label it clearly as a reconstruction and do not use it as proof of device behavior.

## Claim verification before publication

- Supported once receipts are attached: three implemented models; iOS and Android device testing; calendar-first rejection; conversational-composer selection; explicit send-state confirmation; documented review decisions; creation and project use of the requirements-check assistant.
- Keep bounded: “the prototypes exposed,” “device testing changed the direction,” and “the assistant supported requirements checking.”
- Do not claim without new evidence: launch, self-serve use, adoption, conversion, retention, engagement, subscriber satisfaction, time saved, fewer review errors, organizational rollout, or a causal business result.
- Do not describe stakeholder or team review as user validation. If test participants were actual users, document who they were, how many participated, what tasks they completed, and what was observed before changing this language.

## Editorial lineage

The outline uses two optional source-library patterns: “Production context reveals design constraints” for the main decision arc and “One artifact becomes a broader belief” for the bounded closing principle. The requirements-check assistant is presented as a system spin-off under the Product Experiment contract, not as evidence of adoption or a separate workflow transformation.
