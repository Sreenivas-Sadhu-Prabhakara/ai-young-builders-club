# Week 1 · Facilitator run-sheet

*Minute-by-minute plan for "What even is AI?" Read the [setup guide](../for-facilitators/setup.md)
and do the Teachable Machine activity yourself once before today.*

!!! info "Your one job today"
    Get every kid to **train a model with their own hands** and walk out able to say *"AI
    learns from examples."* If you protect nothing else, protect the hands-on and the
    capstone step.

**Prep (5 min before):** laptops on & on wifi, webcams allowed in the browser, Teachable
Machine open on your canary laptop, handouts on tables, safety rules on screen.

---

## 0:00–0:10 — Hook: "Human vs Computer" 🎮

**Goal:** feel the difference between *rules* and *recognizing patterns*.

Play a fast spotting game on the projector. Show pictures (or just describe) and ask kids to
shout whether it's "easy for a computer with rules" or "needs learning from examples":

- Adding 7 + 12 → *easy with rules.*
- Telling a cat from a dog → *needs learning from examples!*
- Sorting names alphabetically → *rules.*
- Recognizing your friend's face → *examples.*
- Knowing if a review is happy or angry → *examples.*

**Land it:** "Computers have always been great at **rules**. The new superpower — AI — is
they can now learn the **fuzzy, patterny** stuff by seeing lots of examples. Today *you*
train one."

> 🗣️ **Talking point:** "Nobody can write a rule for 'what makes a cat a cat.' But show a
> computer thousands of cat pictures, and it figures out the pattern itself. That's AI."

---

## 0:10–0:25 — Concept: rules vs learning from examples 📚

Keep it to ~3 slides (see [slides outline](slides.md)). Cover:

1. **Old way (rules):** humans write every step. Great for math, sorting, clear rules.
2. **AI way (learning):** we show **examples**, the computer finds the **pattern** itself,
   and the result is a **model** that can guess about new things.
3. **The catch:** a model is only as good as its **examples** (training data). Lopsided or
   bad examples → a lopsided or bad model. *Garbage in, garbage out.*

Introduce just four words, point at the glossary: **AI, training, model, training data.**

**Check for understanding (quick):** "If I want an AI to recognize apples, what do I feed
it?" (Lots of apple examples!) "What if I only show it *red* apples?" (It might not know
green ones — that's the examples problem.)

---

## 0:25–0:50 — Hands-on: train a model in Teachable Machine 🦾

This is the magic. Kids go to
[teachablemachine.withgoogle.com](https://teachablemachine.withgoogle.com) → **Get Started**
→ **Image Project** → **Standard image model**.

Demo once on the projector, then let them go. The mission (also on their handout):

1. **Make 2–3 classes.** e.g. `Class 1 = Thumbs Up`, `Class 2 = Thumbs Down`, `Class 3 =
   Nothing/Neutral`. Rename the classes.
2. **Add examples:** hold the pose, click & hold **Hold to Record** to capture ~20–40 webcam
   images per class. More varied examples = better!
3. **Train:** click **Train Model** (stays in the browser; nothing uploads to us).
4. **Preview:** wave their hand around and watch the live confidence bars react. 🎉

**Circulate and prompt thinking:**

- "Add some examples from a different angle/lighting — does it get better?"
- "What happens if you only recorded one pose per class?" (It gets confident but wrong.)
- "Whose model is the most accurate? Why? What did they do differently?" → connects straight
  back to **training data quality**.

**Go Further** for fast finishers: 3+ classes, or feed it deliberately bad examples and
watch it fail, then fix it.

!!! warning "When tech breaks"
    - **Webcam blocked/missing:** use **Upload** mode with a few photos instead of live
      camera, or use sample images you saved beforehand.
    - **Wifi down:** run it on your canary laptop on the projector and have kids direct you —
      "more examples!", "try a new pose!" The lesson still lands.
    - **Total outage:** do the **unplugged version** below.

??? note "Unplugged version (no devices)"
    Play **"Train the Robot."** You are the robot. Kids are the trainers. They want to teach
    you to tell "apple cards" from "banana cards" but they may only show you example cards —
    **no telling you rules**. After ~10 examples each, test you on new cards. Then sabotage
    it: give only yellow apples as examples, then test a red apple — you "fail." Big
    discussion: *the examples decide what the model learns.* Same lesson, zero tech.

---

## 0:50–0:58 — Capstone step: pick your assistant's purpose 🎯

Bring the energy back together. Introduce the **big project**:

> "Over the next 4 weeks, each of you is going to build your **own AI assistant** — and show
> it off on the last day. Today you pick the most important thing: **what will it help
> with?**"

On the handout, each kid writes:

- **My assistant helps with:** ____ (homework? jokes? pet care? a game? practicing a
  language?)
- **Who it's for:** ____ (me? little kids? my class?)
- **A name idea (optional):** ____

Keep it loose and fun — they can change it later. Collect the handouts (or photograph them)
so purposes survive to Week 2.

> 🗣️ **Talking point:** "Just like Teachable Machine needed *you* to decide what it learns,
> your assistant needs *you* to decide what it's for. You're the boss of your AI."

---

## 0:58–1:00 — Wrap & tease 👋

- **One-line recap:** "AI learns from **examples** — you proved it by training one today."
- **Safety reminder:** point to the rules, especially **no secrets**.
- **Tease Week 2:** "Next time: how do the *talking* AIs — chatbots — actually work? And
  you'll give your assistant its personality."

---

## Common kid questions today

- *"Is the model alive now?"* → No — it's just really good at spotting your pattern. It can't
  think or feel.
- *"Did my photos get sent somewhere?"* → No, Teachable Machine trains right in your browser.
  (Still: good habit — no secrets ever.)
- *"Why is it sometimes wrong?"* → Because of the examples you gave it. Better, more varied
  examples → better guesses.

## Facilitator self-check (did the week land?)

- [ ] Every kid trained at least one working model.
- [ ] Every kid can say "AI learns from examples."
- [ ] Every kid wrote down a purpose for their assistant.
- [ ] You collected/saved the capstone purposes for next week.
