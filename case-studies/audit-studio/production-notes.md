# Audit Studio — Production Notes

This companion document contains visual-production guidance, evidence checks, and publication safeguards. None of it belongs in the reader-facing case-study word count.

## Editorial Target

- Public case: Standard mode, 500–600 rendered words, including headings, captions, and evidence-callout copy.
- Structure: hero, a visually neutral At a Glance, four causal project stages, and three evidence callouts placed after their supporting events.
- Captions: fewer than 25 words each.
- Voice: short paragraphs, one idea per paragraph, design judgment before technical mechanism.

## Visual Evidence Slots

| Slot | What to provide | Source basis | Claim supported | Risk / preparation |
| --- | --- | --- | --- | --- |
| Connected-device hero | Full Audit Studio dashboard with an authorized Android tablet mirrored | Current dashboard and connected-device workflow | One workspace coordinates the review | Capture fresh; do not use the offline `Mirror Disconnected` render |
| Before-workflow diagram | `Test APK → QtScrcpy → screenshot/video → Finder → Figma or Excel` | Author-confirmed prior workflow | Review required multiple tools and handoffs | Label as reconstructed; do not add time estimates |
| Annotated dashboard | Full dashboard with four restrained annotations | Repository UI and confirmed design decisions | The interface is organized around review tasks | Annotate mirror hierarchy, contextual actions, workflow cards, and collapsed Activity only |
| Screenshot Flow demo | Start → changing HMI states → candidate count → Review → deselect → Save | Screenshot Flow state model | Automation captures candidates while the designer curates evidence | Record 10–15 seconds; keep the dashboard visible |
| Anonymized chat feedback | Two or three excerpts showing a trial, return request, or scope-expanding request | Author-reported chat-platform feedback | More than ten designers tried it and feedback changed the product direction | Remove names, project identifiers, and confidential product details |

## Suggested Public Captions

Each caption stays below 25 words:

1. **Hero:** “A personal shortcut became a shared HMI review workspace after designers used it and asked it to do more.”
2. **Before workflow:** “One review moved through five separate tools before evidence reached the design record.”
3. **Dashboard:** “Primary review actions stay with the device; setup and diagnostics remain secondary.”
4. **Screenshot Flow:** “The system detects candidate states; the designer decides what becomes evidence.”
5. **Trial feedback:** “Designers returned with new builds—and requests that pushed the tool toward broader in-car validation.”

## Evidence-Callout Specifications

| Role | Statement | Inline emphasis | Evidence status | Evidence IDs | Placement | Source patterns |
| --- | --- | --- | --- | --- | --- | --- |
| Workflow impact | `The first shift was five tools to one review workspace: installing, mirroring, capturing, organizing, and recording evidence became part of the same task flow.` | `five tools to one review workspace` | Author-reported | AS-WORKFLOW-01 | Personal Shortcut, after the before-workflow diagram | MX-01 |
| Return use | `More than ten designers joined facilitated trials. The stronger signal was returning with later builds, which brought the workflow back into real review work.` | `returning with later builds` | Author-reported | AS-TRIAL-01 | Shared Problem, after the facilitated-trial account | MX-09, MX-11 qualified to repeat use only |
| Product influence | `Designers asking to test design files in the car changed the scope: reviewing before implementation became part of Audit Studio's next direction.` | `reviewing before implementation` | Author-reported | AS-FEEDBACK-02 | Broader Review Workspace, after the scope-expanding request | MX-02 |

**Visual intent:** Render each callout as a full-width tinted panel with generous padding, rounded corners, large sentence-scale text, one inline bold phrase, and no visible category label. Keep At a Glance typographically neutral. Separate callouts with the narrative section or its visual; do not stack them together.

### Source-derived candidate

| Type | Candidate statement | Status | Public-use rule | Source pattern |
| --- | --- | --- | --- | --- |
| Next signal | `The next test is whether returning designers begin bringing others into the workflow without me.` | Hypothesis | Keep as ordinary prose or a production-note question; never style it as proof unless the behavior is confirmed | MX-11 |

## Internal Evidence Ledger

Remove this section before publication if the notes are ever exposed publicly.

| Claim | Status | Required receipt |
| --- | --- | --- |
| Five separate tools formed the prior review workflow | Author-confirmed | Reconstructed before-workflow diagram using the confirmed sequence |
| More than ten designers tested the tool | Author-reported | Anonymized chat excerpts or participant record |
| Some designers returned for later build reviews | Author-reported | Anonymized return request or session evidence |
| Returning designers invited others without creator facilitation | Hypothesis | Anonymized invitation or participant trail before presenting as Adoption |
| Trials were facilitated by the creator | Author-confirmed | Preserve this boundary in public copy |
| Manual screenshot capture works | Historically verified | Existing 2560×1600 device screenshot |
| Live mirror works end to end | Assumed final state | Fresh connected-device demo |
| Screenshot Flow review/save works end to end | Assumed final state | Short complete workflow recording |
| APK installation works end to end | Assumed final state | Install-and-launch demo or Activity receipt |
| Video recording works end to end | Assumed final state | Playable output file and in-product success state |
| Image display/upload works end to end | Assumed final state | Target-device demo |

## Claim Boundaries

- Describe the 10+ sessions as facilitated trials, not self-serve adoption.
- Do not claim measured time savings without a consistent before/after task baseline.
- Do not use automated tests as proof of live-device compatibility.
- Do not call the tool production-ready while runtime and device dependencies remain.
- Keep assumed final capabilities in the public walkthrough only after their evidence receipts are complete.
- Codex supported implementation; product framing, workflow definition, information architecture, and design judgment remained with the designer.
- Do not convert repeat use into second-order adoption. Invitations, teaching, or redistribution require their own receipt or explicit author confirmation.

## Confidentiality and Capture Guidance

- Use a real Android tablet or emulator at its native aspect ratio, never generic phone chrome.
- Keep enough of the dashboard visible to show how the device relates to the review workflow.
- Redact project names, map data, device identifiers, internal paths, and confidential HMI content.
- Use an early repository version for any evolution comparison; do not recreate a fictional first interface.
- Keep demos task-focused and remove unnecessary cursor movement.

## Source-to-Visual Mapping

| Public section | Primary visual | Evidence source |
| --- | --- | --- |
| Hero / At a Glance | Connected-device dashboard | Audit Studio dashboard plus fresh runtime capture |
| Personal Shortcut | Before-workflow diagram | Author-confirmed tool sequence |
| Shared Problem | Anonymized early trial and return-use excerpts | Chat-platform feedback supplied by the author |
| Productized Workflow | Annotated dashboard and Screenshot Flow demo | Dashboard hierarchy plus candidate-review model |
| Workflow-impact callout | Full-width tinted narrative callout | Confirmed before-workflow sequence plus Audit Studio product overview |
| Return-use callout | Full-width tinted narrative callout | Author-reported trial and return-use receipts |
| Product-influence callout | Full-width tinted narrative callout | Scope-expanding feature-request receipt |
| Broader Review Workspace | Scope-expanding feature request | Chat feedback requesting in-car design-file validation |
