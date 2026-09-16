# LearnXRP demo1

A throwaway, static, navigable demo that stitches the winning sketches together. Not a commitment to any direction. Plain HTML, CSS and JS, no build step.

Live: https://saintsampo.github.io/LearnXRP3/ (deployed from this folder by `.github/workflows/pages.yml`).

## What is in it

| page | from sketch | what it does |
|---|---|---|
| `index.html` | Login A (two doors) with the code-first card from Login C; Welcome back from Login E | Students type a code and a first name and wait for the teacher. Educators sign in. Explorers skip accounts. When this device remembers students, the Welcome back view shows first. |
| `home.html` | Student home F | Today strip plus app cards that say where they open, what you do there, and what you need. |
| `app.html?app=…` | Running app G, Ribbon A | Lesson coach on the left, the real app in an iframe on the right. `xrpcode` loads https://xrpcode.wpi.edu/ with `allow="bluetooth; serial; usb"`. `docs` loads https://introtoroboticsv2.readthedocs.io/. Others are placeholders. |
| `teacher.html` | Teacher view H | Teacher hosts the room. Start class, names arrive in the queue, Let in. |
| ribbon | Ribbon A + language + settings | 48px bar on every page: brand, crumb, robot chip, sync dot, language (EN / ES / AR with RTL), identity, and a gear that opens the demo settings menu. |

## Demoing the teacher-hosted room for real

The join handshake runs through `localStorage`, so two tabs in the same browser talk to each other:

1. Open `teacher.html`, press **Start class**.
2. Open `index.html` in a second tab, type `XRP-7K2Q` and a first name, press **Join**.
3. The name appears in the teacher tab's "Asking to join". Press **Let in** (or turn on auto-admit for known names). The student tab proceeds.

If no teacher tab is open, the student is let in after four seconds and a toast says so.

## Demo settings (gear in the ribbon)

Role, robot state, sync state, brand config (Experiential, plus placeholder Educabot and FIRST Global), language, lesson step, device name, remembered students on this device, page links, and Reset demo. State lives in `localStorage` under `lx.demo1`.

Deep links seed state, for example: `home.html?lx={"role":"student","name":"Maya","robot":"ok"}`.

## Run locally

Any static server works:

```
cd brainstorming/demo1
python -m http.server 8765
```

Then open http://localhost:8765/. Chrome or Edge, since the framed XRPCode needs Web Bluetooth and Web Serial.
