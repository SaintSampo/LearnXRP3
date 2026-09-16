# Sketch Manifest

## Design Direction
LearnXRP3 follows the Launcher architecture (Proposal A): a thin shell that launches independent apps in iframes over a postMessage bridge, with teacher-held pseudonymous student tags instead of student accounts. Three vibes are in play and each sketch shows all three as variants so the layout question and the vibe question can be judged separately: **Playful workshop** (chunky, bright, Scratch energy for 9 to 13), **Clean maker tool** (calm, precise, Arduino Cloud / Onshape posture, 9 through college), and **Classroom-first** (structured, teacher-legible, assignments as the hero). Target is Chrome or Edge on laptops and Chromebooks; phone is Drive only.

## Reference Points
Scratch, Code.org (class codes, picture passwords, kid-safe), Arduino Cloud and Onshape (professional tools with a light touch). XRPWeb (WPI) is the real third-party app inside the frame.

## Themes
`themes/default.css` carries all three palettes scoped as `.theme-playful`, `.theme-clean`, `.theme-classroom`. The sketch toolbar can force one theme onto every variant.

## Sketches

| # | Name | Design Question | Winner | Tags |
|---|------|----------------|--------|------|
| 001 | student-home | What does a student see first, and how much of the class shows on the home screen? | — | layout, student, launcher, robot-connect, join-class |
| 002 | running-app | When XRPWeb runs inside the shell, where does the lesson live and how visible is the bridge? | — | layout, lesson, iframe, bridge, xrpweb, robot-lock |
| 003 | teacher-class | How does a teacher run a class of pseudonymous tags and keep names off the server? | — | layout, teacher, roster, privacy, class-code, progress |
