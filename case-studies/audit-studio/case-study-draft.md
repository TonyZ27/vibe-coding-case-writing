# Audit Studio: From a Screenshot Shortcut to a Shared Review Workspace

I built Audit Studio to bring Android HMI review tasks into one local web workspace. What began as a screenshot utility grew through trials with other designers—and a decision to automate capture while keeping evidence selection in their hands.

[media]
placement: hero-end
suggestion: Connected Audit Studio dashboard showing the live HMI device as the primary surface, with review tools visible around it.

[resource]
title: View the GitHub Repository
description: Source code and setup instructions for Audit Studio.
url: https://github.com/TonyZ27/audit-tool

## At a Glance

- **What:** A local web workspace for designers reviewing Android human–machine interfaces (HMI).
- **How:** Brings build installation, live-device viewing, and screenshot capture into one review flow; designers select which captured screens become evidence.
- **Why it matters:** Gives designers a common workspace for tasks previously spread across several tools, while keeping control of the review record in their hands.

## Context: One review, several handoffs

My review workflow moved from installing a test APK to opening QtScrcpy, capturing screenshots or video, organizing files in Finder, and transferring evidence into Figma or Excel.

Each tool covered part of the job. I still had to coordinate the sequence, switch between windows, and remember commands. I started with a small screenshot utility to make my own reviews easier, then put it on a web page and shared it with the design team.

[highlight]
content: Other designers tried it in sessions I facilitated. When some returned with another build to review, I had a reason to develop the utility around a recurring team task.

## Organizing the workspace around a review

I structured the interface around what a designer needs to do with a connected device: install a build, observe the interface, and capture states for review.

The live-device view became the main surface. APK installation and Screenshot Flow had dedicated task cards, with activity information available alongside the work. This gave the growing set of capabilities a common starting point: the device under review.

[highlight]
content: My contribution was defining that flow and the relationships between its actions. Codex supported implementation and debugging; I directed the product structure, interactions, and implementation review.

## Designing a reviewable flow that could expand

Screenshot Flow made the boundary between automation and design judgment explicit. As a designer moves through an interface, the system detects visual changes and collects candidate screenshots. Stopping the flow opens a review step, where the designer can remove unwanted screens and save the chosen set.

**Software can identify a changed screen; the designer decides whether it is useful evidence.** I kept selection as a separate step so the system could handle capture without deciding what belonged in the review record.

[media]
placement: inline
suggestion: Screenshot Flow sequence showing capture, candidate review, deselection, and the final saved evidence set.

Sharing that workflow also brought requests beyond checking an implemented interface. Designers wanted to upload design files to the in-car system and review concepts before implementation. That request broadened the direction from build review toward earlier design validation, and influenced the larger device view and dedicated workflow cards.

In-car design-file review remains an extension prompted by those requests. The meaningful signal was that other designers saw more work they wanted to bring into the workspace beyond my original screenshot task.

## Outcome

Audit Studio progressed from a personal capture utility to a workspace tried by more than ten designers. Some returned with later builds, and their requests helped shape its direction.

Those sessions were facilitated by me. They establish trial and repeat use; they do not yet establish independent adoption or measured time savings.

The clearest product lesson was where to put the handoff: let the system collect possible evidence, then let the designer decide what is worth keeping.

[highlight]
content: The project taught me to make that boundary explicit when working with Codex too: automate deterministic capture and state handling, but keep contextual judgment in the designer’s review step.
