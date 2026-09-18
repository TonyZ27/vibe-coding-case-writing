# Volvo Design Helper: Turning Design-System Rules into a Shared Preflight Workflow

I built Volvo Design Helper to make contributions to a shared Figma design system more consistent. The plugin makes asset rules visible at the point of contribution, helps designers resolve issues before handoff, and prepares validated assets for the engineering pipeline.

[media]
placement: hero-end
suggestion: A composite of the preflight dashboard showing scan scope, issue impact, and the Prepare Gerrit handoff action.

[resource]
title: View the plugin source
description: Explore the Figma plugin, its validation rules, and the guided Gerrit handoff implementation.
url: https://github.com/TonyZ27/volvo-design-helper

## At a Glance

- **What:** A Figma plugin for designers contributing icons and tokens to a shared design system.
- **How:** Checks assets against shared rules, supports naming fixes, and packages selected assets for a guided Gerrit handoff.
- **Why it matters:** Makes contribution rules visible and repeatable across designers, reducing reliance on manual checks and repetitive handoff documentation.

## Context: Shared contribution needs shared rules

Multiple designers collaborated on the Figma design system. Its flexible architecture made the system reusable, but it did not determine how decisions reached production. Designers still documented changes manually; engineers re-entered values and relied on clarification to understand what had changed.

An export feature could package assets, but it could not ensure that every contribution followed the same naming, structure, and variant rules. Manual review left enforcement dependent on the reviewer and the moment. The rules needed to be public and applied consistently inside the contribution workflow.

I reframed the opportunity from “make export faster” to “make readiness visible.” I defined and facilitated the workflow with stakeholders, then translated the agreed rules into a preflight experience inside Figma.

## Turning export into a readiness decision

The plugin scans icon component sets on the current page and local variables across the file, then summarizes issues before a designer chooses what to export.

I separated findings by consequence: blocking issues must be fixed, excluded assets will not enter the ZIP, and advisory issues can be deferred. A generic warning system would still leave the designer asking whether they could continue. The primary action instead names the remaining blockers, then changes to “Prepare Gerrit handoff” only when the selected assets are ready.

[media]
placement: inline
suggestion: An annotated dashboard state that shows the difference between blocking issues, excluded assets, and advisory recommendations.

## Automating corrections without hiding judgment

Some violations have predictable corrections. The plugin can normalize names and apply the same fix across a group. Each issue also links back to its source in Figma for inspection.

Other decisions should not be automated. A missing token category requires an understanding of the system’s architecture, so the plugin identifies the problem but leaves classification to the designer. This kept repetitive cleanup automated while structural design decisions remained visible and human-owned.

The final boundary follows the same principle. The plugin packages selected assets, then prepares a Terminal-based Gerrit handoff that creates a change for the existing review and CI/CD pipeline. Publishing happens outside the plugin, so the interface does not claim completion prematurely.

## Using AI to build reusable workflow infrastructure

I used AI primarily as a builder that turned my product intent into working code. I defined the workflow, rules, consequences, and handoff boundaries; AI helped implement the scanner, dashboard, fixes, exports, and handoff states.

[highlight]
content: Vibe coding worked best once the rules were explicit enough to become executable. The hard part was not generating the plugin UI; it was turning design-system judgment into checks with clear consequences, exceptions, and handoff boundaries.

## Outcome

For the design-system workflow I facilitated, Volvo Design Helper removed the need to produce repetitive screenshots and specification files for each change. It reduced the design-to-development feedback cycle from two or three days to under 30 minutes.

The durable result is not simply faster export. It is a shared, executable contribution standard: designers can see what is ready, what needs attention, and what still requires their judgment before a change enters engineering review.
