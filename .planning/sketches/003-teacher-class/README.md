---
sketch: 003
name: teacher-class
question: "How does a teacher run a class of pseudonymous tags: see who is stuck, hand out the code, and keep names off the server?"
winner: null
tags: [layout, teacher, roster, privacy, class-code, progress]
---

# Sketch 003: Teacher Class View

## Design Question
The teacher holds the key. The server knows tags, picture passwords and progress events; names live only in the teacher's browser. Does the class view read as a wall of student cards, a progress matrix, or an assignment list? And is the class code prominent enough to project?

## How to View
open .planning/sketches/003-teacher-class/index.html

## Variants
- **A: Playful student cards** — yellow banner with the class code, four stat tiles, then a card per tag with avatar, picture password, progress ring and live status. Stuck students get a red outline. Click a card for actions.
- **B: Clean progress matrix** — one table: tag × 7 steps as colored cells, filters (here now, stuck, finished step 3), row click fills the side panel; class settings toggles for apps, 13+ and AI hints.
- **C: Classroom assignments** — tabs for Assignments, Roster and Settings; a "live now" strip of 12 dots; each assignment expands to a per-tag table; settings show the age band, app allowlist and the COPPA authorization attestation.
- **D: Experiential site** — site-brand chrome: blue navbar, a red class-code band like the site's red sections, four stat cards on grey, a striped Bootstrap-style roster table with progress bars, dark footer.
- **E: Experiential, playful** — navy-to-blue gradient class-code hero with a red slash, stat tiles with colored dots, then student cards with a colored top stripe (blue working, red stuck, grey away), brand-colored avatars and progress rings. Heading reads "Who needs you right now".
- **F: Calm class list** — no shapes, no stat tiles, no red. One sentence sums up the room, then a plain list: student, progress, "right now" in words (working in Blocks Lab, quiet for 14 min, not here today), robot. Class code sits in a quiet pill. Login cards replace picture passwords.
- **G: One thing at a time** — the open assignment as a single card with one segmented bar and three groups in words: Ahead, On track, Might want a hand. Below it, "Next up" with what to bring and read, and a small Class card. Nothing to configure on this screen.

## What to Look For
- "Put it on the board" opens a projector-sized code screen in every variant. Is the join URL clear enough for a nine-year-old?
- Toggle "Show my names": a local-only name column appears. Does it feel safe and obvious that names never leave the device?
- Add a tag: a new pseudonymous tag appears with a picture password. Where should the "shown once" password go?
- Which view answers "who needs me right now" fastest: the red outlines (A), the red cells (B), or the stuck chip in the live strip (C)?
- Settings only exist in B and C. Is A missing them, or does a playful teacher view belong elsewhere?
