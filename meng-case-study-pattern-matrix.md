# Meng Xie AI-Native Case Study Pattern Matrix

Research snapshot: 2026-08-24. This is an analysis of the 17 public project pages listed on Meng Xie's AI-Native Design Portfolio. One page, **Subs Dogfooding for All Employees**, was classified from its portfolio-card summary because its detailed page could not be fetched during this pass.

## What repeats across the portfolio

Every full case begins with a compact metadata block and an **At a Glance** triad:

- **What** was made
- **How** it was made
- **Why it matters** beyond the feature itself

The following sections change with the project. The recurring narrative is:

> concrete friction or constraint -> shipped artifact or workflow -> evidence of use / adoption -> a transferable design belief

This is not a conventional UX-process template. Personas, journey maps, and research phases appear only when they are necessary to explain a decision. AI is described as a concrete capability or workflow, while the designer's judgement is visible in the framing, trade-offs, scope, and final lesson.

## Project matrix

| Project | Portfolio label | Best-fit narrative | Distinctive proof | Reusable structure pattern |
| --- | --- | --- | --- | --- |
| AI-Powered Group Order for WhatsApp | Hackathon AI Product | Product experiment | Top 10 / 200+; consumer and business sides | cultural behavior -> product bet -> solution scope -> response -> principle |
| WhatsApp Production Audit Platform | Vibe Designing Tool | Workflow / system | Internal self-serve tool; shared across design and engineering | deliverable gap -> tool -> build approach -> lessons -> redefine the deliverable |
| Little Color World | Community Game | Product utility | Live zero-install game; real child use | personal situation -> accessibility constraints -> product choices -> observed use -> principle |
| Passport Photo Generator | Community Tool | Product utility | Live free tool; community reactions / shares | specific personal friction -> minimal product -> user quote / response |
| Human-AI Collaborative Design | Workflow | Practice note, not a repo-led product case | 18K -> 8K SVG reduction; hybrid workflow | hard constraint -> failed pure-AI route -> handoffs -> result -> reusable tips |
| Parental Leave Calculator | Community Tool | Product utility | v2; community distribution; parents helped | rules-heavy pain -> v1 -> feedback-led v2 -> community response -> belief |
| Pencil.dev Evaluation | Tool Exploration | Practice note | landscape comparison triggered a request | market framing -> comparative model -> capabilities -> team decision |
| AI Design Learning Hub | Community Knowledge | Workflow / system | three-pillar curation system | information-overload problem -> system -> design intent -> value -> learning |
| Production Codebase Prototyping | Production Prototype AI Product | Product experiment | 5 directions; debug APK; 2.5K lines; org response | production constraint -> real build -> new framework -> method -> impact |
| Vibe Designing | Hackathon Claude Skill | Workflow / system | two reusable skills; ten design lenses | capability gap -> framework -> two modules -> why it scales |
| AI-Native Prototyping Playbook | Framework / Knowledge Sharing | Workflow / system | progressive playbook; co-creator feedback | scattered knowledge -> learning architecture -> delivery design -> adoption |
| Bloom Parenting Resource Hub | Community Deployed | Product utility, with community-build variation | live bilingual resource; 5+ contributors | fragmented community need -> product scope -> contributor model -> community thesis |
| AI Product Studio | Vision / Full-Stack Design | Portfolio-level point of view, not a project template | capability stack across prior work | synthesis of projects -> capability model -> future direction |
| Subs Dogfooding for All Employees | Workflow / Subs Dogfooding | Workflow / system | iOS + Android; a four-step audit workflow | portfolio summary only: gated-feature friction -> audit workflow -> reusable process |
| AI-Native Figma SoTs | Workflow / Claude Skill | Workflow / system | editable frames and flowcharts; reusable skill; community pull | two recurring pains -> two workflows -> output evidence -> packaging -> adoption |
| AI-Native Deck Creation | Workflow / Community | Workflow / system | 5+ approaches; office-hours adoption | landscape -> thesis -> selected workflow -> trade-offs -> second-order adoption |
| Status Scheduling Subscriber UX | Product Design / AI-Native Loop | Product experiment, with system spin-off | iOS + Android feature; review assistant shipped org-wide | 0->1 product decision -> core and trust journeys -> AI division of labor -> adjacent workflow bottleneck -> reusable tool -> outcomes |

## What the matrix validates

The three repo-led archetypes are valid:

1. **Product Utility** — a real, specific user problem; the case proves usefulness, focused scope, and often a tight feedback loop.
2. **Product Experiment** — a new product bet or high-fidelity prototype; the case proves the quality of a key decision under real constraints.
3. **Workflow / System** — a repeated organizational friction turned into a reusable workflow, skill, tool, or learning system; the case proves adoption beyond its author.

However, the portfolio also contains three **non-template formats**:

- **Practice note:** a documented method, failure, or tool evaluation. Use this for an essay or short capability card, not a full repo-to-case-study flow.
- **Portfolio thesis:** a synthesis of several projects. It should be authored after multiple cases exist, not generated from one repository.
- **Community-build variation:** Product Utility plus a visible contributor / governance section.

This distinction keeps a repo agent from pretending every project is a complete product case study.

## The narrative system to carry into a future skill

### 1. Lead with an editorial claim, not a tool list

The hero tells the reader what changed and why it matters. Tool names support the claim in **How**; they are not the headline.

### 2. Use an explicit claim-proof rhythm

Each major claim needs a nearby receipt: a real product state, version change, demo, number, community response, physical-device test, or named output. If none exists, write it as an intention or omit it.

### 3. Let the case choose its own middle

The fixed shell is only:

`At a Glance -> Context -> project-specific proof -> Outcome / response -> transferable lesson`

The middle changes: a utility case shows v1/v2; an experiment shows decision-making and constraints; a system case shows workflow and adoption.

### 4. Separate AI execution from design ownership

State what AI automated, generated, inspected, or accelerated. State what the designer framed, chose, corrected, scoped, or judged. Do not use tool activity as evidence of design quality.

### 5. Treat visuals as receipts

Every visual should prove a local claim:

| Claim | Suitable evidence |
| --- | --- |
| A product reduces a complex task | short end-to-end demo or input -> output sequence |
| A key interaction changes behavior | annotated final screen or 8-12 second interaction clip |
| Iteration was feedback-led | v1 / v2 comparison with the feedback source named |
| A system creates a reusable capability | workflow diagram plus real generated output |
| A decision held under production constraints | physical-device or real-state evidence |
| The work spread beyond one person | launch post, usage/reaction receipt, or contributor view |

## Template boundary for the future repo agent

The agent should select only from the three repo-led archetypes after creating an evidence map. If the repository instead supports only a hybrid workflow lesson or tool evaluation, it should recommend a **Practice Note** and say that a full case study would overstate the available evidence.

Before prose, the agent should produce:

1. observed evidence / inferred interpretation / missing context;
2. recommended archetype and an alternative;
3. one-sentence story thesis with supporting evidence;
4. the minimum interview questions; and
5. a claim-to-visual evidence plan.

Only then should it draft the case study.

## Primary sources

- https://mengxie.me/
- https://mengxie.me/projects/leave-calculator.html
- https://mengxie.me/projects/production-codebase-prototyping.html
- https://mengxie.me/projects/figma-sot.html
- https://mengxie.me/projects/status-scheduling.html
