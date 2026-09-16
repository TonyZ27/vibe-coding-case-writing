# Audit Studio — Case Study Story Diagnosis

> Status: Pre-draft evidence and narrative plan  
> Date: 2026-08-28  
> Target reader: Product-design recruiter or hiring manager  
> Target length: Approximately five minutes  
> Recommended archetype: **Workflow / System**  
> Archetype confidence: **High**  
> Publish readiness: **Ready for drafting — repeated facilitated trials are author-confirmed; runtime claims remain provisional**

## Recommended story

Audit Studio is not most compelling as “a designer built an Android tool.” Its stronger story is how a personal utility became a shared review system: a designer recognized that teammates faced the same recurring workflow problem, translated technical utilities into designer-facing tasks, and used a coding agent to implement an extensible product definition.

### Recommended title

**Scaling a Personal Android Audit Tool into a Shared Review Workspace**

### Alternative titles

- **Designing Reviewable Automation for HMI Audits**
- **From ADB Commands to a Designer-Facing Audit Workflow**

### Recommended Story Thesis

> I turned a personal shortcut for Android build reviews into a shared workspace tested with more than ten designers, several of whom returned for later build reviews. Instead of coordinating APK installation, QtScrcpy, capture tools, and file organization as separate utilities, the workspace organizes them around review tasks while keeping evidence selection under human control.

This thesis uses author-confirmed repeat use and does not require an unsupported time-saving claim.

### Why Workflow / System is the best fit

- The starting problem is repeated workflow friction across Android HMI design reviews.
- The product reorganizes several existing utilities into one repeatable review sequence.
- The most distinctive design judgment is encoded into the workflow: capture candidate states automatically, but let the designer decide which states become evidence.
- The repository contains a packaged local dashboard, setup scripts, task-oriented UI, backend actions, and tests.
- More than ten designers reportedly tested the shared tool and returned to use it in later build reviews, moving the project beyond a creator-only workflow.
- The alternative **Product Utility** route is weaker because the case is not mainly about one narrow end-user task; its value comes from coordinating a broader review system.

## Evidence status

### Observed in the repository

| Evidence | What is directly observable | Strength | Narrative use |
| --- | --- | --- | --- |
| Working-tree status | Local `main` matches `origin/main` at `59261b9`; README and dashboard HTML have uncommitted edits | Strong | Source boundary; do not attribute presentation-only changes to committed history |
| Dashboard hierarchy | Live device mirror is primary; screenshot flow, APK installation, image display, and Activity are secondary workflows | Strong | Proves task-oriented information architecture |
| Mirror implementation | scrcpy H.264 stream → local WebSocket → browser WebCodecs canvas | Strong for implementation; not current runtime proof | Explains technical feasibility only where needed |
| Manual screenshot path | Display-aware `capture_screenshot_png()` uses the selected device and extracts a valid PNG payload | Strong | Supports reliable evidence capture |
| Screenshot-flow model | `IDLE → CAPTURING → REVIEWING`; visual hashes identify candidate changes; designer selects what to save | Strong | Central encoded design judgment |
| APK workflow | Dedicated upload/install endpoint plus drag/drop UI, validation, and explicit Install action | Strong for implementation | Supports “design around tasks, not commands” |
| Video workflow | Start/stop API and FFmpeg piping exist | Medium | Implemented capability with an unresolved runtime boundary |
| Security model | Loopback dashboard, session-token API authentication, WebSocket token/origin checks | Strong | Optional constraint; include only if trust/locality matters to the story |
| Tests | Fourteen test definitions cover state, security, PNG parsing, FFmpeg resolution, and scrcpy protocol behavior | Strong for focused implementation checks | Quality evidence; not proof of live-device completion |
| Commit history | Six visible commits show movement from screenshot utility to connectivity, redesigned dashboard, flow telemetry, and broader features | Strong | Iteration timeline |
| Output artifact | Two real 2560×1600 HMI screenshots exist under `~/Downloads/Audit_Sessions/Screenshots/` | Strong | Real input/output evidence for screenshot capture |

### Author-reported in the attached context

| Claim | Evidence status | How to use it |
| --- | --- | --- |
| Designers installed a test APK, opened QtScrcpy, captured screenshots/video, organized files in Finder, then transferred findings into design files or Excel | Concrete author-reported before workflow | Use as the Before Workflow; do not add time savings without a measurement basis |
| Design-team feedback expanded the product beyond implementation-fidelity review, including requests to upload design files to the in-car system for validation | Concrete author-reported feedback-to-decision example | Use as evidence for the shift from shared web page to extensible dashboard |
| The user framed the problem, selected scope, defined IA and interactions, and corrected generated implementation | Clear ownership statement | Use in Role and AI collaboration sections |
| Codex generated Python/HTML, integrated ADB/scrcpy, implemented UI iterations, and updated tests | Clear AI role statement | Use to separate judgment from execution |
| The product evolved from screenshot support into a broader workspace | Supported by commit history | Strong iteration narrative |
| More than ten designers tested Audit Studio and some returned for later build reviews; the creator still facilitated the sessions | Author-confirmed repeated trial; feedback exists in chat conversations | Classify as **Trial**, not self-serve reuse; use anonymized chat excerpts if publishable |
| The original personal utility became a shared web page, then an extensible dashboard after teammates requested broader design-validation capabilities | Author-confirmed and directionally supported by repository history | Use as the main product-evolution arc |
| A requested extension was uploading design files to the in-car system for validation | Author-confirmed request; implementation state not yet established | Use as evidence that the problem expanded beyond implementation-fidelity review |

### Previously verified runtime evidence

Prior project validation recorded:

- A real Android 16 tablet screenshot was captured successfully at 2560×1600.
- Display-aware screenshot handling and PNG extraction were validated.
- Fourteen focused tests and Python compilation passed at that time.
- Video recording remained blocked because no working FFmpeg runtime was available.
- Live mirror and APK paths had partial diagnostic evidence and should not be described as currently verified without a new check.

These are historical receipts, not a fresh release-readiness claim.

The author has asked the narrative to assume that all features will work in the intended final state. This can guide the final workflow description, but it does not convert a future-state assumption into runtime evidence. The draft should maintain an internal **verify before publishing** marker for every capability not yet demonstrated end to end.

### Inferred — do not write as fact

- Audit Studio reduced review time.
- Designers completed audits with less help from engineering.
- Automated candidate capture improved evidence quality.
- The tool replaced QuickTime, scrcpy, or CLI workflows in practice.
- Every dashboard capability currently works end to end.

Each inference needs either author confirmation or a supporting receipt.

## Source inventory

| Source area | What it contains | Portfolio role | Evidence strength | Visual opportunity |
| --- | --- | --- | --- | --- |
| Project context | Android HMI review workspace for a design team | Establish domain and audience | Medium–Strong | Metadata strip and one-line workflow summary |
| Problem | Test-version APK install → QtScrcpy → screenshot/video recording → Finder/file organization → transfer into design files or Excel | Narrative trigger | Strong author report | Before-workflow friction map |
| Role and scope | Problem framing, feedback synthesis, feasibility, IA, interaction direction, AI review | Establish ownership | Strong author report | Responsibility split: Designer / Codex / Design team |
| Research/input | Shared use revealed broader needs, including uploading design files to the in-car system for validation | Decision basis | Medium–Strong author report | Personal utility → shared page → extensible dashboard timeline |
| Product insight | The missing value was workflow orchestration, not new technical capability | Core reframing | Strong | “Tools → designer tasks” before/after model |
| Design decisions | Task-based IA, meaningful-state capture, reviewable automation, dominant mirror surface | Demonstrate judgment | Strong | Annotated dashboard and decision cards |
| Interaction flow | Install → observe → capture → curate → save evidence | Explain system behavior | Strong | End-to-end workflow diagram |
| Iteration | Screenshot utility → connected dashboard → broader audit workspace | Demonstrate evolution | Strong | Commit-based before/after timeline |
| Product artifact | Local web dashboard, Python panel server, scripts, tests, captured PNGs | Show what was built | Strong | Live dashboard screenshot, review modal, real output |
| Outcome | More than ten designers reportedly tested it and some returned for later build reviews, with the creator facilitating | Close with repeated demand and product learning rather than self-serve adoption or efficiency claims | Strong author report; chat evidence still needs anonymization | Anonymized feedback receipt plus real output |
| Reflection | Reorganizing existing technology around design work was the product contribution | Transferable belief | Strong | Closing takeaway block |

## Workflow / System contract score

| Dimension | Score | Rationale |
| --- | ---: | --- |
| Repeated friction | 2/2 | Repeated review tasks and tool switching are clearly described |
| Workflow model | 2/2 | Inputs, actions, human review, and outputs are visible |
| Encoded judgment | 2/2 | Candidate-state detection plus designer confirmation is explicit |
| Real output | 2/2 | Working dashboard and real tablet screenshots exist |
| Adoption integrity | 1/2 | Repeated facilitated trials are labeled accurately; independent self-serve reuse is not claimed |
| Evidence integrity | 2/2 | Runtime boundaries and self-reported claims can be separated |
| Ownership | 2/2 | Designer, Codex, and design-team roles are clearly distinguished |
| **Total** | **13/14 provisional** | The contract passes because trial is labeled correctly; runtime verification and publishable feedback receipts remain pre-publication gates |

Adoption level: **3 — Trial.** More than ten designers reportedly tested the tool and some returned for later reviews, but the creator still facilitated the sessions. Do not describe this as self-serve adoption or reuse.

## Recommended five-minute outline

### 1. Why one review required five tools

Establish the recurring Android HMI review workflow: install a test APK → open QtScrcpy → capture screenshots or video → organize files in Finder → transfer findings into a design file or Excel.

Evidence needed: a concrete before sequence; optional approximate frequency or time only if the basis is known.

### 2. Reframing tools as design-review tasks

Explain the core product decision: designers think in tasks such as “install this build,” “observe this state,” and “capture this flow,” not in commands or technical utilities.

Evidence: dashboard IA and the decision alternatives from the Context document.

### 3. Designing automation that remains reviewable

Use Screenshot Flow as the key design-decision deep dive:

`Move through flow → detect meaningful visual changes → collect candidates → designer reviews → save selected evidence`

This section should carry the case. It demonstrates both automation and product judgment.

### 4. From personal utility to shared, extensible workspace

Show the iteration path from a command-avoiding tool built for one designer, to a shared web page, to a dashboard shaped by repeat use and requests for broader design-validation capabilities.

Use commit history and, if possible, screenshots from an early commit and the current interface.

### 5. Using Codex for execution without outsourcing product judgment

Separate roles explicitly:

- **Designer:** problem framing, feedback synthesis, scope, feasibility decisions, IA, interaction model, visual direction, implementation review.
- **Codex:** Python/HTML implementation, ADB/scrcpy integration, debugging, UI changes, test generation.
- **Design team:** workflow feedback and feature requirements.

Include one concrete example where generated implementation was corrected because it did not match the desired workflow.

### 6. What works, what remains, and what I learned

Report capability status honestly. The strongest verified outcome is a functioning local interface plus real screenshot output. Treat mirror, APK, and especially video according to their current verification status.

Close with the existing takeaway: the contribution was not new Android debugging technology; it was translating existing technical capabilities into a design-team workflow.

## Visual Evidence Plan

| Section | Asset | What to capture | Claim supported | Status / risk |
| --- | --- | --- | --- | --- |
| Hero | `01-audit-studio-live-dashboard.png` | Current dashboard with an authorized tablet mirrored; preserve the full IA | One workspace organizes the review workflow | Needed; static offline render is not runtime proof |
| Problem | `02-before-workflow.svg` | Confirmed sequence across ADB, mirror tool, capture, APK install, and file organization | The problem was orchestration, not missing capability | Can be designed after author confirms actual steps; label reconstructed |
| Reframe | `03-tools-to-tasks.svg` | Left: technical utilities; right: designer-facing tasks | Product structure hides implementation detail behind review tasks | Supported by context and dashboard |
| Core decision | `04-screenshot-flow-demo.mp4` | Start flow → move through HMI states → candidate counter → stop/review → deselect/save | Automation identifies candidates; designer controls evidence | Needed; 10–15 seconds |
| Core decision | `05-review-modal.png` | Candidate grid with selected/unselected states | Automated capture remains reviewable | Needed from live or controlled session |
| Iteration | `06-v1-vs-current.png` | Early screenshot/capture interface beside current dashboard | Tool evolved in response to workflow needs | Needs early-commit render; do not invent a before state |
| Workflow | `07-install-observe-capture-curate.svg` | End-to-end audit sequence with human and system actions distinguished | Audit Studio encodes a repeatable review model | Supported; diagram must show fallback/error points |
| Output | `08-real-hmi-screenshot.png` | Existing 2560×1600 captured HMI screen | The screenshot path produced a real device artifact | Available; verify confidentiality/redaction before publication |
| AI collaboration | `09-designer-codex-team.svg` | Inputs and decisions across Designer / Codex / Design team | AI accelerated execution while product judgment remained with the designer | Supported by context; add one correction example |
| Outcome | `10-feedback-receipt.png` | Anonymized chat excerpts showing trial participation, return requests, or feature requests | Repeated demand shaped the product beyond its creator's original use case | Feedback exists on a chat platform; redact names and internal details |
| Boundary | `11-capability-status.png` | Working / implemented-not-verified / blocked capabilities | Honest system maturity | Can be created from confirmed current status |

### Capture guidance

- Use a real tablet or emulator at its native aspect ratio; do not place the HMI in a generic phone mockup.
- Keep the dashboard visible around the mirrored device so the workspace relationship is clear.
- Record only the shortest complete task; avoid full-product tours and unnecessary cursor movement.
- Redact project names, map data, device identifiers, internal paths, and any confidential HMI content.
- Do not use the existing static offline render as the final hero because it shows `Mirror Disconnected`.
- Do not present the real HMI screenshot publicly until its content is approved.

## Claims to avoid or soften

- Avoid broad **“team-wide adoption”** language. State the narrower supplied claim: more than ten designers tested it and returned for later build reviews.
- Avoid **“reduced review time”** unless a before/after basis exists.
- Avoid **“fully working”** while capability status differs across screenshot, mirror, APK, and video.
- Avoid **“video recording works”** until FFmpeg is installed and a playable MP4 is verified.
- Avoid **“production-ready”**; this is a local internal workflow with device/runtime dependencies.
- Avoid **“AI designed and built the product.”** Codex implemented; the attached context assigns framing and product decisions to the designer.
- Avoid presenting automated tests as proof of live-device compatibility.

## Remaining publication inputs

1. **Publication asset:** Select two or three chat excerpts that can be anonymized to show initial testing, return use, or a feature request.
2. **Product media:** Confirm whether the existing HMI screenshots can be published; otherwise capture a redacted or non-confidential demo.

Drafting policy confirmed by the author: describe the intended final product with all planned capabilities working, while retaining internal **verify before publishing** markers for capabilities that do not yet have end-to-end receipts.

## Source map

- Author context: `/Users/jzhou102/Downloads/Audit Studio Context.md`
- Repository: `/Users/jzhou102/Documents/GitHub/audit-tool`
- Main dashboard: `/Users/jzhou102/Documents/GitHub/audit-tool/audit-tool-layout.html`
- Backend and workflow state: `/Users/jzhou102/Documents/GitHub/audit-tool/panel-server.py`
- Focused test definitions: `/Users/jzhou102/Documents/GitHub/audit-tool/tests/test_audit_studio.py`
- Product README: `/Users/jzhou102/Documents/GitHub/audit-tool/README.md`
- Real screenshot output: `/Users/jzhou102/Downloads/Audit_Sessions/Screenshots/screenshot_20260812_175228.png`
- Archetype contract: `vibe-case-study/references/archetypes/workflow-system.md`
