# Floaty — editorial and evidence notes

Status: revised English draft based on repository inspection and author context supplied on 2026-09-20. The narrative can use first person for the window-bound concept, editing experience, UI, shortcuts, cross-Space pinning, product requirements, interaction rules, edge cases, acceptance criteria, AI direction, testing, and release preparation.

## Story direction

- **Story Thesis:** Starting with a basic floating-note framework, the author directed AI as a product manager and technical lead to build Floaty into a native macOS workspace tool, translating interaction intent into PRDs, edge-case rules, acceptance criteria, implementation tasks, and tested window behavior.
- **Recommended depth:** Standard; the middle connects the contextual-note product decision with the author’s AI-directed development method.
- **Repository establishes:** Window selection, exact runtime identity, explicit reconnection, separate manual-hide and minimize states, restoration of prior pinning, native macOS integration, a concrete revision to focus handling, tests, and prepared release documentation.
- **Author reports:** The starting point was a basic floating-note framework. The author defined the window-bound concept, editing experience, UI, shortcuts, cross-Space pinning, requirements, interaction rules, edge cases, and acceptance criteria; directed AI through small implementation tasks; reviewed code; ran tests; requested revisions; and prepared release materials.
- **Proposed structure:** Hero → At a Glance → basic framework to contextual note → product behavior as specification → AI collaboration as product and technical leadership → bounded outcome.
- **Useful visuals:** Real window-binding behavior and an artifact sequence connecting the PRD, edge-case table, implementation plan, commits, tests, and release notes. No product recordings were inspected; the draft’s media blocks remain recommendations.

The README retains download and development links to `cn-qlg/floaty`. Describe the author as starting with a basic floating-note framework and defining the subsequent product experience; do not imply that every part of the base application was created from scratch. The AI workflow and ownership statements come from author context, while the repository provides implementation evidence.

## Evidence map

Inspected main tree: `17279c184516719d63a2fcd69b9eb82c9b100c20`. Links below pin relevant evidence to that revision.

| Draft claim | Source | Boundary |
| --- | --- | --- |
| Context and intended behavior | [Design PRD](https://github.com/TonyZ27/Floaty/blob/17279c184516719d63a2fcd69b9eb82c9b100c20/docs/prds/2026-07-23-window-bound-notes-design-prd.md) | Documented problem framing, not user research or an author-reported personal trigger. |
| Picker, keyboard access, permission explanation | [WindowPickerPage](https://github.com/TonyZ27/Floaty/blob/17279c184516719d63a2fcd69b9eb82c9b100c20/src/assignment/WindowPickerPage.tsx) | Source inspection; no live UI verification. |
| Metadata-based discovery | [Window catalog](https://github.com/TonyZ27/Floaty/blob/17279c184516719d63a2fcd69b9eb82c9b100c20/src-tauri/src/platform/macos/window_catalog.rs) | Discovery reads window metadata including titles; avoid claiming it reads no information about other apps. |
| Target status, rebind and unbind | [BindingButton](https://github.com/TonyZ27/Floaty/blob/17279c184516719d63a2fcd69b9eb82c9b100c20/src/sticky/BindingButton.tsx) | Implemented UI states. |
| Manual hide survives minimize/restore | [State reducer and tests](https://github.com/TonyZ27/Floaty/blob/17279c184516719d63a2fcd69b9eb82c9b100c20/src-tauri/src/assignment/state.rs) | Tests were read, not executed. |
| Reconnection and pin restoration | [Binding persistence](https://github.com/TonyZ27/Floaty/blob/17279c184516719d63a2fcd69b9eb82c9b100c20/src-tauri/src/db/window_bindings.rs) | Stored window titles are descriptive metadata, not automatic identity recovery. |
| Native integration and focus management | [Coordinator](https://github.com/TonyZ27/Floaty/blob/17279c184516719d63a2fcd69b9eb82c9b100c20/src-tauri/src/assignment/coordinator.rs), [native backend](https://github.com/TonyZ27/Floaty/blob/17279c184516719d63a2fcd69b9eb82c9b100c20/src-tauri/src/platform/macos/window_spaces.rs) | Uses private macOS framework symbols. A same-Space placement check does not establish subsequent full-screen behavior. |
| Live focus revalidation iteration | [July 28 correction](https://github.com/TonyZ27/Floaty/commit/772a29eec9e357f60a2c7e78d0c5dcc122636413) | The patch supports the mechanism and change; no invented user feedback or measured improvement. |
| Native behavior as an early acceptance gate | [Implementation plan](https://github.com/TonyZ27/Floaty/blob/17279c184516719d63a2fcd69b9eb82c9b100c20/docs/superpowers/plans/2026-07-25-window-bound-notes.md) | Describe what the plan requires, not proof that the gate was passed. |

## Publication checks

- Preserve the distinction between the starting framework and the author’s product and implementation contribution.
- Describe the feature as built and tested by the author, without implying wider adoption or measured productivity gains.
- Do not claim reduced distraction, time savings, validated productivity, or reliable behavior across macOS versions without evidence.
- Do not equate the v0.2.0 release-notes document with a verified downloadable release in TonyZ27/Floaty. No release availability was verified.
- Keep screenshots and recordings authentic. In particular, test two windows from the same app and fast switching, not only switching between different apps.
- The current implementation restores ordinary layering in unrelated foreground contexts. Avoid broad claims that the note becomes hidden on every focus change.
- Attribute product direction, task decomposition, review, testing, revision requests, and release preparation to the author. Do not claim that AI worked autonomously or that development speed was measured.
