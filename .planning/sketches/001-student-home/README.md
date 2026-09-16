---
sketch: 001
name: student-home
question: "What does a student see first in the Launcher shell, and how much of the class shows on the home screen?"
winner: null
tags: [layout, student, launcher, robot-connect, join-class]
---

# Sketch 001: Student Home

## Design Question
The Launcher shell's home screen is the only screen every student sees every time. Is it an app grid, a workbench with a rail, or a "today" queue from the teacher? And where do the robot connection and the class code live?

## How to View
open .planning/sketches/001-student-home/index.html

## Variants
- **A: Playful workshop** — chunky app tiles with 3px borders and offset shadows, a yellow "keep going" hero, robot card beside it. Scratch energy, aimed at 9 to 13.
- **B: Clean maker tool** — left rail, search, compact app cards with metadata chips, recent work table, robot panel on the right. Arduino Cloud posture, works to college age.
- **C: Classroom-first** — class banner, "Today" assignment queue with step counts and due dates, teacher announcements, apps demoted to a "free explore" row.
- **D: Experiential site** — built from experiential.bot: blue navbar (#22527B) with the white wordmark, red primary buttons (#D1182C), Montserrat, white/grey/dark section bands, the site's isometric hero illustration. Reads as "the website turned into an app".
- **E: Experiential, playful** — same brand, played up: pill nav and buttons, the red-and-blue X diagonal as a motif in the navbar and footer, a gradient hero card with a progress ring, app cards with a colored "puzzle knob" and tilted icon tiles, the logo's bright blue (#0A6EFF) as a second accent. Still soft shadows and Montserrat, no cartoon borders.
- **F: Cards that say where** — E's look, a notch more classroom tool: a "Today in Period 3" strip on top, then app cards that each carry a mock screenshot of the destination, an "opens XRPCode by WPI" badge, one line on what you do there, and a "You need / Last time / Stays in" block. The button says "Open Blocks Lab", never just "Open".
- **G: Pick, preview, open** — same strip, then a list of apps on the left and a sticky preview on the right: a large mock screenshot, "When you press Open" as four numbered sentences, what you need, last time, and one Open button. Answers "where does this take me" before the click.

## What to Look For
- Which one makes a nine-year-old start in under two minutes, and which one a sixteen-year-old is not embarrassed by.
- Robot connect: hero card (A), side panel with board/firmware/battery (B), or a header button (C). Click Connect in each; it cycles searching → connected.
- Join a class: modal in all three. Try a bad code, then `XRP-7K2Q`.
- Clicking any app shows the launch overlay with the bridge context line. The app itself is sketch 002.
- Toolbar: force one theme onto all three layouts to separate the layout question from the vibe question.
