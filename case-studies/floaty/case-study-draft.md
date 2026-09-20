# Floaty: Directing AI to Build a Context-Aware Native Mac App

Floaty began as a basic desktop framework that could create floating notes. I turned that foundation into a native macOS note and to-do experience designed to stay with the work it belongs to—and used AI across the process as a product manager and technical lead, from defining behavior to reviewing implementation and preparing the release.

[media]
placement: hero-end
suggestion: Record Floaty binding a note to one specific application window, following that window into its full-screen Space, and returning to ordinary behavior after unbinding.

[resource]
title: Explore Floaty on GitHub
description: Review the product requirements, implementation plans, source code, tests, and release notes.
url: https://github.com/TonyZ27/Floaty

## At a Glance

- **What:** A local macOS note and to-do app with Markdown editing, shortcuts, reminders, and notes that can be attached to specific work windows.
- **How:** A user selects an exact application window from a note, and Floaty manages the note’s Space, layering, visibility, and recovery states while preserving its own position and content.
- **Why it matters:** A note can remain available in the context where it is useful without becoming a permanent overlay across unrelated work.

## From floating notes to working context

The starting framework could create independent floating notes. My work was to define the product beyond that foundation: the text-editing experience, interface, keyboard shortcuts, cross-Space pinning, and a window-bound note model for macOS.

The central shift was treating a note as part of a specific task context. Instead of pinning a note above every application, a user can bind it to one exact window. The note keeps its own position and size, appears with the selected window—including in its full-screen Space—and returns to normal behavior when it is unbound.

“Exact” was an important product decision. Two browser windows may belong to different tasks even when they come from the same application or have similar titles. Floaty therefore associates a note with a particular runtime window rather than guessing from the application name. If that window closes or Floaty restarts, the note remains intact and asks the user to reconnect it instead of silently attaching to something else.

[media]
placement: inline
suggestion: Show the window picker followed by the same note attached to one of two windows from the same application. Then close the target to show the explicit reconnection state.

## Defining the behavior before generating the code

Window binding looks like a small control in the note header, but it changes how the app responds to permissions, focus, full-screen Spaces, minimized windows, manual hiding, app restarts, and disconnected displays. I documented those conditions as product requirements, interaction rules, edge cases, and acceptance criteria before treating them as implementation tasks.

For example, a note hidden because its target was minimized should return when the target is restored. A note the user deliberately hid should stay hidden. Binding also temporarily supersedes global pinning, so Floaty remembers the previous pin preference and restores it after unbinding. The window picker uses application names, icons, and titles without capturing the contents of other windows.

These were product decisions, not implementation details to leave for generated code to resolve. Writing them down gave each state an expected behavior and made the experience testable across the React interface, local persistence, and native macOS window layer.

## Working with AI as a product manager and technical lead

I used AI throughout implementation, but my role was larger than prompting it to generate a feature. I supplied the product requirements and expected behavior, divided the work into small tasks, reviewed the generated code, ran tests, and requested revisions when the result did not match the intended interaction.

The repository reflects that progression. The work moves from design and technical PRDs into phased plans. I kept the work bounded through commits and used the same requirements to decide whether each implementation step was complete.

[media]
placement: inline
suggestion: Present a compact artifact sequence: the window-bound note PRD, its edge-case table, the implementation task breakdown, representative feature and fix commits, passing tests, and the prepared v0.2 release notes.

The working principle was to convert design intent into observable behavior before delegating implementation. AI could produce and revise code across the frontend and Rust backend, while I retained responsibility for what the product should do, how edge cases should resolve, and whether the resulting behavior met the specification.
