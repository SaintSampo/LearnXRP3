# Sketch Manifest

## Design Direction
LearnXRP3 follows the Launcher architecture (Proposal A): a thin shell that launches independent apps in iframes over a postMessage bridge, with teacher-held pseudonymous student tags instead of student accounts. Three vibes are in play and each sketch shows all three as variants so the layout question and the vibe question can be judged separately: **Playful workshop** (chunky, bright, Scratch energy for 9 to 13), **Clean maker tool** (calm, precise, Arduino Cloud / Onshape posture, 9 through college), and **Classroom-first** (structured, teacher-legible, assignments as the hero). Target is Chrome or Edge on laptops and Chromebooks; phone is Drive only.

## Reference Points
Scratch, Code.org (class codes, picture passwords, kid-safe), Arduino Cloud and Onshape (professional tools with a light touch). XRPWeb (WPI) is the real third-party app inside the frame.

A fourth variant, **Experiential site**, was added to every sketch on Jacob's request: it uses the live experiential.bot brand as-is (Odoo theme values: red #D1182C, blue #22527B, dark #343A40, grey #E9ECEF, Montserrat 300/400/600 with 500-weight headings, the white wordmark logo, the isometric hero illustration) so the team can judge "our website turned into an app" against the three invented vibes.

A fifth variant, **Experiential, playful**, extends the site brand with playful but professional elements: rounder shapes, pill buttons, the X-mark diagonal as a recurring motif, progress rings, puzzle-knob app cards, and the logo's bright blue as a second accent.

Jacob liked the playful Experiential aesthetic and asked for two revisions per screen on it, each leaning a notch more "classroom tool": student home cards must say where they go (F: cards with destination screenshots, G: list plus preview with "when you press Open"); the running app must show the real look of the apps in the frame (F: XRPCode Blocks as on xrpcode.wpi.edu, G: XRPCode Python plus its Dashboard); the teacher view must put less pressure on teachers and drop the picture-password shapes (F: calm list in words, G: one assignment, three groups).

Jacob then asked to remove printed login cards entirely and proposed that a student's computer send their name directly to the teacher's computer. Sketch 003 variant H ("Teacher hosts the room") models this: presence is the password, names are end-to-end encrypted student-to-teacher, and the server stores only tags.

## Themes
`themes/default.css` carries all five palettes scoped as `.theme-playful`, `.theme-clean`, `.theme-classroom`, `.theme-experiential`, `.theme-experiential-play`. The sketch toolbar can force one theme onto every variant.

## Sketches

| # | Name | Design Question | Winner | Tags |
|---|------|----------------|--------|------|
| 001 | student-home | What does a student see first, and how much of the class shows on the home screen? | — | layout, student, launcher, robot-connect, join-class |
| 002 | running-app | When XRPWeb runs inside the shell, where does the lesson live and how visible is the bridge? | — | layout, lesson, iframe, bridge, xrpweb, robot-lock |
| 003 | teacher-class | How does a teacher run a class of pseudonymous tags and keep names off the server? | — | layout, teacher, roster, privacy, class-code, progress |
| 004 | ribbon | What is the one bar every app inherits, and how does it behave inside a third-party app with its own navbar? | — | component, ribbon, shell, brand, i18n, robot-state |
| 005 | login | One entry page for six kinds of people, never asking an under-13 student for an email or birthday | — | login, onboarding, coppa, student, teacher, parent, camp |
| 006 | code-buddy | What shape should AI take: chat, persistent Cloudflare agent, notes on blocks, hardware pit crew, or teacher-only copilot? | — | ai, code-buddy, cloudflare, classroom, guardrails |
