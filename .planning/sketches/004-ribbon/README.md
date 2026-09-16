---
sketch: 004
name: ribbon
question: "What is the one bar every app inherits, how much does it carry, and how does it behave inside a third-party app that has its own navbar?"
winner: null
tags: [component, ribbon, shell, brand, i18n, robot-state]
---

# Sketch 004: The Ribbon

## Design Question
In the Launcher architecture the ribbon is the only chrome every app shares, so it is the unified look and feel. This sketch isolates it: what it contains, what changes by context, what a brand config may touch, and what happens when the app below draws its own navbar (XRPCode does).

Each variant renders the same ribbon in six places: student home, inside XRPCode on a lesson step, inside the Educabot simulator, teacher hosting the room, a camp session with no wifi, and Drive on a phone. Controls at the top change robot state, sync state, brand config and language (including Arabic, right-to-left) across all six at once.

## How to View
open .planning/sketches/004-ribbon/index.html

## Variants
- **A: Slim and constant** — 48px, identical everywhere. Lesson lives in the page or a drawer. Cheapest; stacks on XRPCode's navbar.
- **B: Two tiers** — 56px ribbon plus a 36px context tier only inside apps: app and provider, step progress, bridge state, Hint and Next. Most informative, most height.
- **C: Collapses in apps** — 56px on shell pages, 28px inside an app with a step pill that opens the lesson drawer. Expands on the chevron; would auto-collapse on Run. Most app space.

## What to Look For
- The XRPCode row: is a second dark bar under the ribbon tolerable (A), justified (B), or solved (C)?
- Switch robot state through none → searching → connected → low → lost. Does the chip read at a glance in every brand?
- Switch to Educabot or FIRST Global: the ribbon should still feel like the same product with a different badge.
- Switch to Arabic: the ribbon mirrors. Anything that does not mirror is a bug in the pattern.
- The teacher row and the phone row: does the right side stay recognizable when the content changes?
- The rules card lists what the ribbon promises apps. Argue with it.
