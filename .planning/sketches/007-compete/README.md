---
sketch: 007
name: compete
question: "How should a classroom competition module organize teams, schedule, rankings and the field management system so a teacher can run a match day without help?"
winner: null
tags: [module, compete, fms, teacher, schedule, rankings]
---

# Sketch 007: Compete

## Design Question
Compete is a module for teachers running competitions in class. The functionality is fixed: a teams list, a schedule generator, rankings, and an FMS (field management system) with a match timer, scorekeeping and state controls. The question is how to organize it so a teacher, possibly running their first competition, is never lost.

All three variants run the same engine: add or remove teams, generate a round-robin schedule that avoids back-to-back matches, load a match, run a real clock (0:30 autonomous, 2:00 teleop), tally tasks per alliance with plus and minus buttons, end, commit, and watch rankings update by wins then average score. A "fast clock" checkbox in the footer speeds the demo.

## How to View
open .planning/sketches/007-compete/index.html

## Variants
- **A: Two tabs, Event and Field** — the split from the brief. Event shows teams, schedule and rankings side by side. Field is the FMS: a big clock, red and blue score panels, and a row of six state buttons (Load next, Start, Pause, Abort, End early, Commit).
- **B: Run of show, one screen** — built around the match in progress. Schedule is a queue on the left, rankings live on the right, FMS in the middle with a single Advance button that changes with the state (Start match → Pause → Commit score → Load next). Teams live in a drawer. A Projector view fills the screen with the clock and scores for the board.
- **C: Competition day in four steps** — organized by time: Teams, Schedule, Play, Results. Each step says what to do and marks itself done. Play adds a pre-match checklist and keyboard shortcuts (Space, Enter, Esc). Results adds awards and certificate printing.

## What to Look For
- Generate, load Q1, Start, tick the fast clock, score a few tasks, let it end, Commit. Do this in each variant and notice where your eyes go.
- A is honest to the brief. Is the six-button row too much during a live match?
- B's Advance button: does one changing button feel safer or scarier than six fixed ones?
- C's steps: helpful on day one, annoying on day ten? Note that the same data drives all three, so a real module could offer C as onboarding and B as the day view.
- Projector view in B: is that the thing that sells the module to a teacher?
