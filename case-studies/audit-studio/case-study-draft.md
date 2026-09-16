# From Five Tools to One HMI Review Workspace

I built Audit Studio to make Android HMI reviews easier for myself. Sharing that first tool showed me the problem was broader—and changed what I decided to build next.

## At a Glance

Audit Studio is a web workspace for installing builds, mirroring a device, and capturing evidence during HMI reviews.

*Personal shortcut → Shared problem → Productized workflow → Team validation → Broader review workspace*

## Personal Shortcut

Before Audit Studio, reviewing a test build meant installing an APK, opening QtScrcpy, recording screenshots or video, organizing the files in Finder, then moving the evidence into Figma or Excel.

I knew the tools worked. I just did not want to keep switching between them, memorizing terminal commands, or installing another program for each task. So I built a small utility for myself, starting with screenshot capture.

*Test APK → QtScrcpy → screenshot/video → Finder → Figma or Excel*

> The first shift was **five tools to one review workspace**: installing, mirroring, capturing, organizing, and recording evidence became part of the same task flow.

## Shared Problem

I later put the utility on a web page and shared it with the design team. More than ten designers tried it in sessions I facilitated. Some came back when they had another build to review.

> More than ten designers joined facilitated trials. The stronger signal was **returning with later builds**, which brought the workflow back into real review work.

That repeat use showed I was not solving only my own setup annoyance. Other designers also needed a clearer path from a test build to evidence they could use in their design work.

## Productized Workflow

I reorganized the page around review tasks rather than Android utilities. The connected device became the main surface. Installing a build, taking a screenshot, recording a flow, and checking activity became parts of the same sequence instead of separate destinations.

The most important decision was how Screenshot Flow handled automation. While a designer moves through the interface, the tool detects visual changes and collects candidate screens. It does not save everything automatically. At the end, the designer reviews the candidates, removes noise, and chooses what enters the audit record.

*Move through the interface → detect change → collect candidates → review → save evidence*

A visual change is easy for software to detect. Whether that change matters is a design judgment. I automated the repetitive capture work, then deliberately returned control to the designer.

I defined the product flow, information architecture, and interaction model. Codex helped implement and debug the Python, HTML, ADB, and scrcpy pieces.

## Broader Review Workspace

Once people used the web version, their requests changed again. They were not only comparing a build with the intended design. Some wanted to upload design files to the in-car system and review concepts in context before implementation.

> Designers asking to test design files in the car changed the scope: **reviewing before implementation** became part of Audit Studio's next direction.

That request changed how I understood Audit Studio. It could be more than a fidelity-checking tool; it could become a workspace for different kinds of design validation. I rebuilt the page around a larger live-device view and moved APK installation and Screenshot Flow into dedicated task cards.

Because I facilitated the sessions, I treated them as product validation rather than self-serve adoption. The useful signal was that designers returned with real review work and asked the tool to cover more of it.

Audit Studio started as a shortcut. It became a product when other designers used it and changed what I thought it should do.
