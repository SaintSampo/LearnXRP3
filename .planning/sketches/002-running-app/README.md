---
sketch: 002
name: running-app
question: "When a third-party app (XRPWeb) is running inside the shell, where does the lesson live and how visible is the bridge?"
winner: null
tags: [layout, lesson, iframe, bridge, xrpweb, robot-lock]
---

# Sketch 002: Running App

## Design Question
The Launcher's central bet is a lesson from us wrapped around an app from someone else. Does the lesson sit beside, above, or under the frame? How much of the bridge (app id, robot lock, save state, progress events) should a student see, and how much only a teacher or developer?

The framed app is a mock of XRPWeb's Blockly view: navbar (Connect, Run, Stop, Save, Blocks/Python), toolbox with the "3rd Party" category, a line-follower block program, and the MicroPython shell.

## How to View
open .planning/sketches/002-running-app/index.html

## Variants
- **A: Playful coach** — a 340px "coach" column of speech-bubble cards on the left, the current step in yellow with a big step number, bridge tucked in a small card at the bottom.
- **B: Clean panel + status bar** — collapsible lesson panel with the full step list, breadcrumb header, and a mono status bar across the bottom that shows every bridge field.
- **C: Classroom assignment** — assignment header with due date, progress bar and a Turn in button; lesson panel on the right with a teacher note; bridge as a small footer inside the panel.
- **D: Experiential site** — site-brand chrome: blue navbar with breadcrumb, a grey "Connected app" strip carrying the bridge fields as badges, lesson panel left in Montserrat with red actions, dark footer bar like the site footer.
- **E: Experiential, playful** — coach column of rounded tiles on a soft blue-grey ground: a ring-and-eyebrow header tile, the current step on a white-to-blue gradient tile, pill step list, bridge in a navy tile at the bottom; the frame gets rounded corners and a soft shadow.
- **F: Real XRPCode (Blocks)** — E's coach column, calmer, wrapped around a faithful mock of xrpcode.wpi.edu: dark navy navbar with File / View / Help and the grey CONNECT XRP button, the Filesystem panel with My View / System View, editor tab for line_follow_v2.blocks, the real toolbox categories (DriveTrain, Individual Motors, Servos, Sensors → Reflectance / Distance / Gyro, Gamepad, Control Board), and the xterm shell. The lesson text refers to XRPCode's own buttons.
- **G: Real XRPCode (Python + Dashboard)** — the 13+ path: same chrome, MicroPython editor in XRPCode's dark theme with a Dashboard tab showing its real widget set (Reflectance L/R, Distance, Voltage, Gyro, Accelerometer, Encoders). Run the program and the Reflectance widget moves with the shell output.

## What to Look For
- Play the loop in each: Connect (robot lock goes to `wpi.xrpweb`) → Run (shell prints reflectance values) → the step's auto-check turns green → Next step (new context sent to the app).
- Switch to the simulator: the robot lock is released and the frame tag changes. Is that visible enough?
- Which variant makes the lesson feel like part of the app rather than a sidebar bolted on?
- Bridge visibility: B shows everything, A hides most, C shows a summary. Which is right for students, and does a teacher need B?
- Toggle Blocks/Python in the frame. Python Lab is 13+; the shell hides the app, not the toggle.
