# Meng Xie Case-Study Source Library

This library converts the validated Meng Xie corpus into optional narrative lessons. Use a pattern only when the current project's evidence matches it. Do not copy wording, headings, visual styling, or unsupported claims.

The detailed corpus and source boundaries remain in the [validated Pattern Matrix](../../../meng-case-study-pattern-matrix-validated.md).

## How to use the library

1. Diagnose the current project's archetype and evidence gaps first.
2. Retrieve only patterns that match a real event, decision, proof type, or presentation need.
3. Adapt the narrative logic to the project rather than forcing its facts into the source case.
4. Record which source pattern influenced the outline in production notes, not necessarily in public prose.
5. Prefer the current project's stronger evidence when it conflicts with a source pattern.

## Narrative pattern cards

| Pattern | Useful when | Source cases | Adaptable lesson | Required evidence | Avoid |
| --- | --- | --- | --- | --- | --- |
| Personal constraint sharpens scope | A project begins with a specific personal situation | Little Color World; Passport Photo; Leave Calculator | Start with the triggering moment, then show how it constrained the minimum useful product | Concrete situation, working task, use receipt | Inflating a personal problem into a market claim |
| Feedback visibly changes v2 | Requests caused a material product change | Leave Calculator; Bloom | Show request -> implementation change -> changed understanding | Feedback receipt and inspectable version difference | Calling an unsourced change feedback-led |
| Production context reveals design constraints | Static mocks could not answer the real question | Production Codebase Prototyping; Status Scheduling | Explain what the working environment exposed and how it changed the decision | Real build/state and specific discovered constraint | Treating code volume as design impact |
| Repeated friction becomes a workflow | Several people repeat the same manual process | Production Audit; Dogfooding; Figma SoTs | Make the before flow concrete, then show the new input/decision/output model | Repeated actors, workflow, real output | Presenting a tool list as a system |
| Packaging separates reuse from the creator | A method becomes installable or teachable | Figma SoTs; Vibe Designing; Playbook | Show how judgment was encoded and how others accessed it | Packaged artifact and external use | Claiming adoption from availability |
| Human-AI handoff beats full automation | AI reaches a hard quality or system boundary | Human-AI Collaborative Design | Constraint -> failed route -> changed division of labor -> better result | Failed output, intervention, verified result | Generic “human in the loop” language |
| Choose tools by task fit | Multiple tools were actually tested | Pencil.dev Evaluation; AI-Native Deck Creation | Compare capabilities against the decision context and name unsuitable uses | Real comparative trial and selection criteria | Declaring a universal winner |
| Information architecture is the product | Discovery or learning friction is central | AI Design Learning Hub; Playbook | Show how content structure reduces the cost of acting | Before-state friction and inspectable architecture | Treating categories alone as user impact |
| Contribution expands product scope | Other people add requests, content, or features | Bloom; Group Order | Show how participation changed ownership or scope | Named contribution behavior and resulting change | Equating reactions with contribution |
| Distribution creates product trade-offs | Access and setup determine whether a workflow travels | Dogfooding; Figma SoTs | Treat installation, security, and maintenance as part of the design | Channel comparison and real distribution evidence | Hiding setup friction |
| Second-order use is stronger than reach | A user teaches or redistributes the method | AI-Native Deck Creation; Playbook | Highlight behavior that no longer depends on the creator | Teaching, reuse, or redistribution receipt | Calling views or comments adoption |
| One artifact becomes a broader belief | The project earns a transferable conclusion | Across the corpus | End with the narrow belief demonstrated by the events | Clear causal chain and bounded lesson | Producing a symmetrical slogan by default |

## Presentation pattern cards

| Pattern | Use | Boundary |
| --- | --- | --- |
| Hero claim | State artifact, difference, and significance in one or two sentences | Do not lead with the AI tool |
| Proof strip | Surface two to four high-value numbers or states | Every item needs a basis and should not duplicate the body verbatim |
| Variable middle | Name sections after actual decisions, tasks, or project stages | Do not force Research / Ideation / Design |
| Claim-to-visual pairing | Place demos, comparisons, and receipts next to their claim | Do not use generated product UI as evidence |
| Colored proof block | Emphasize a verified impact or earned insight | Color cannot upgrade the strength of a claim |

## Expansion schema

Add future sources as pattern cards rather than copying whole articles. Each addition should record:

```text
Pattern name:
Source and access date:
When useful:
Narrative mechanism:
Evidence required:
Visual or proof treatment:
Known weaknesses or claims not to inherit:
Related archetypes:
```

Keep source facts and current-project facts separate. A reference can suggest a question or structure; only project evidence can support the resulting claim.
