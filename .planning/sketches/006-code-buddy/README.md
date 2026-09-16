---
sketch: 006
name: code-buddy
question: "What shape should AI take in LearnXRP: a chat, a persistent companion, notes on the blocks, a hardware diagnostician, or a teacher-only copilot?"
winner: null
tags: [ai, code-buddy, cloudflare, classroom, guardrails]
---

# Sketch 006: Code Buddy

## Design Question
The working group's principle: AI should increase the student's ability to think, not reduce the need to think. Five concepts, deliberately different in where the AI lives and who talks to it, all in the playful Experiential style with a classroom bias. Every one runs on tags, never names, and the teacher can see or switch off whatever students see.

## How to View
open .planning/sketches/006-code-buddy/index.html

## Variants
- **A: Sidekick chat** — a drawer beside XRPCode with context chips (step, program, telemetry, docs). Socratic: asks before it tells, refuses "just tell me" and offers a worked example on a different sensor. Teacher can read every chat.
- **B: A buddy that remembers (Cloudflare Agents)** — one persistent agent per student tag as a Durable Object at the edge: its own memory, WebSocket to the browser, wakes on robot errors, `schedule()` for "before class tomorrow" nudges, follows the tag across Chromebooks. A per-class teacher agent aggregates. The architecture is drawn under the frame.
- **C: Notes in the workspace** — no chat. Numbered notes on the blocks like a kind code review, tap for the why, teacher sets the note level (none / few / many). A predict-before-run gate that needs no model at all.
- **D: Pit crew** — AI for the hardware: runs a checkup, reads telemetry and shell lines, lights up the failing part on a robot map, and says one thing to try. Structured JSON input, so cheap and testable. The working group's log-analyzer idea, made friendly.
- **E: Teacher's copilot** — no student-facing AI. Reads the room by tag, groups students by what they are stuck on, drafts what to say next, tomorrow's warm-up and pairings. Drafts stay on the teacher's device.

## What to Look For
- A: try "Just tell me the answer" and the three quick questions.
- B: press the three demo buttons: a robot error wakes the agent, a nudge gets scheduled, the student switches Chromebooks and the agent follows.
- C: tap the blue dots, change the note level, press RUN and answer the prediction.
- D: run the checkup and watch the left motor light up.
- E: group the class, then draft the three things.
- Which of these would the consortium approve for an under-13 class first? E needs no student-facing review. C needs no model. B is the most ambitious and the most "platform".
