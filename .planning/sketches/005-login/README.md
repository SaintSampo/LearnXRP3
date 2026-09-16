---
sketch: 005
name: login
question: "One entry page for six kinds of people: how do we get an under-13 student into class in seconds without ever asking for an email, while teachers, parents, camp leaders and home explorers still find their door?"
winner: null
tags: [login, onboarding, coppa, student, teacher, parent, camp]
---

# Sketch 005: Login

## Design Question
The people this page must serve, on the same page:

| person | what they need | what we never ask |
|---|---|---|
| Student under 13, in a class | class code + first name, teacher lets them in | email, birthday, password |
| Student 13 to 17 | same; may add an email later to keep work across computers | |
| Teacher or mentor | Google, Microsoft or an emailed link; attests school authorization once | a password |
| Parent at home | educator sign-in, then a family class code for their kid | the kid's email |
| Camp or club leader | educator sign-in; gets a session code that expires | |
| Just exploring | nothing; local profile on this computer; can join a class later | |

The age band comes from the room, not from the student, so the page never asks how old anyone is.

## How to View
open .planning/sketches/005-login/index.html

## Variants
- **A: Two doors** — students left (code + first name), adults right (Google, Microsoft, emailed link), an explore bar underneath. Classic, everything visible.
- **B: One question at a time** — "Is there a code on the board?" Then first name. Then wait for the teacher. "There is no code" branches to home / educator / 13+ account. One input per screen, built for nine-year-olds.
- **C: Code first** — the code entry is the page, Kahoot-sized, in the brand gradient. Everything else is four quiet cards on the right.
- **D: Pick your role** — four role cards (student in a class, student at home, teacher or mentor, parent); the form and a plain-words "what happens" panel change with the pick.
- **E: Welcome back** — for shared classroom computers: the device remembers who used it in this class; tap your name and the teacher lets you back in. Code entry and educator sign-in are secondary.

## What to Look For
- Type a bad code in any variant, then `XRP-7K2Q` and a name: every student path ends in "hang on, your teacher is letting you in", the same moment as sketch 003 variant H.
- Which variant gets a nine-year-old to the waiting screen fastest with the fewest wrong turns? Which one a teacher can explain in one sentence?
- E assumes Chromebook carts. Is remembering first names on a shared device acceptable to a school, given the names never reach the server?
- D's "what happens" panel: is that the right place to explain COPPA to a parent?
- Phone width via the toolbar: B and C survive, A and D stack, E gets long.
