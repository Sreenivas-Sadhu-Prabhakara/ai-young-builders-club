# Week 3 · Facilitator run-sheet

*Minute-by-minute plan for "A taste of real code." Read the
[setup guide](../for-facilitators/setup.md) and **run the
[Colab notebook](../resources/colab-notebook.md) yourself once** before today — including
the save-a-copy step.*

!!! info "Your one job today"
    Get every kid to **edit Cell 2 and chat with their own assistant in real code**, and walk
    out able to say *"I commanded an AI with code — same code, my personality."* If you
    protect nothing else, protect the hands-on and the **save-a-copy** capstone.

**Prep (5 min before):** laptops on & on wifi, signed in to Google, the
`assistant_starter.ipynb` open on your canary laptop, **model access confirmed working on
the canary** (a real reply comes back — see
[Setup → Model access for Week 3](../for-facilitators/setup.md#model-access-for-week-3-important)),
the facilitator Drive folder open, handouts on tables, glossary on screen.

---

## 0:00–0:10 — Hook: your assistant, ALIVE in code 🔌

**Goal:** the jaw-drop — the Week 2 personality is now *running software*.

On the projector, open the notebook with **your** demo persona already in Cell 2. Run Cells
1–4 live, then **type a message and get a reply** in front of everyone.

> 🗣️ **Talking point:** "Last week you gave your assistant a personality. Today **YOUR
> assistant comes alive — in real code you write.** Watch — I type, it answers. That's not
> magic. That's a few lines of Python talking to an AI."

Then a quick **"what's an API?"** analogy — ordering at a restaurant:

- **You (your code)** decide what you want and ask.
- **The waiter + menu (the API)** is the agreed way to ask and what you're allowed to order.
- **The kitchen (the AI model)** does the real work and sends a dish back.

> 🗣️ **Talking point:** "You never walk into the kitchen. You ask through the waiter. Our
> code asks the AI model through its **API** — and the **API key** is like a members-only
> card. *I* hold the card. You never touch it."

---

## 0:10–0:25 — Concept: clicking → coding 📚

Keep it to ~3 slides (see [slides outline](slides.md)). Cover:

1. **From clicking to coding.** Last week you *clicked* a chatbot. Today you **command** one
   with code — more power, more control.
2. **The new words** (point at the [glossary](../resources/glossary.md)): **code**,
   **Python** (a friendly language that reads almost like English), **Colab** (run Python in
   your browser), **notebook** (a doc of runnable blocks), **cell** (one block you can run
   ▶️), **API** (one program asking another to do something), **API key** (a secret password
   — *the facilitator holds it*), **variable** (a labeled box that holds a value).
3. **How our notebook is built.** Four cells. **You only ever edit Cell 2** — your
   assistant's personality. Cell 1 connects to the model, Cell 3 is the "brain loop," Cell 4
   is the chat.

**Reassure the nervous ones:** "It's **fill-in-the-blanks**. You change about **4 lines**,
all marked 👉. You **can't break it** — if it acts weird, just **re-run the cell**."

**Check for understanding (quick):** "Where does the AI model actually live?" (Behind the
**API** — our code asks it.) "Who holds the secret key?" (The facilitator — never us.)

---

## 0:25–0:50 — Hands-on: bring your assistant to life 🦾

This is the magic. Kids open the
[notebook](../resources/colab-notebook.md) in Colab (or from your Drive). Demo once on the
projector, then let them go. The mission (also on their handout):

1. **Run Cell 1 — Setup.** It connects to the AI model. **Don't change it** — the key is
   handled for you. They should see `✅ Connected!`.
2. **Edit Cell 2 — their assistant.** This is the only cell they change. Using their **Week 2
   personality**, they fill the four 👉 lines:
   ```python
   ASSISTANT_NAME = "Sparky"
   PERSONALITY    = "cheerful, patient, and a little bit silly"
   PURPOSE        = "helping kids practice their times tables"
   RULE           = "give a friendly hint before the answer, and never be mean"
   ```
   Then **run Cell 2** — it prints `🤖 Meet <name>!` and the system prompt it built.
3. **Run Cell 3 — the brain loop.** Nothing visible happens; it just teaches the notebook
   *how* to ask the AI. (Curious kids can read it.)
4. **Run Cell 4 — chat!** Type a message, get a reply from **their** bot. 🎉

**Circulate and prompt thinking:**

- "Change your `PERSONALITY` to a pirate, re-run Cell 2 *and* Cell 4 — does it talk
  differently? **Same code, new assistant.**"
- "Does your bot actually follow your `RULE`? Try to make it break the rule."
- "What's different between your bot and your neighbor's? Only **Cell 2** changed!"

**Go Further** for fast finishers: change the Cell 4 greeting, add a second `RULE`, add a
`MOOD` variable, or give it a catchphrase.

!!! warning "When tech breaks (and the key rule)"
    - **Key safety — non-negotiable:** kids must **never see or paste a raw API key**. Use
      Colab **Secrets** (🔑) or a classroom proxy URL. See
      [Setup → Model access](../for-facilitators/setup.md#model-access-for-week-3-important).
    - **No internet / no key / quota hit:** switch the notebook to **canned-response fallback
      mode** (built into `assistant_starter.ipynb`). Kids **still edit Cell 2 and see the
      loop work** — replies are faked, but the idea lands: *same code, different assistant.*
    - **A kid's notebook won't run:** have them follow along on **your working copy on the
      projector**, calling out the `PERSONALITY` and message to type. The lesson still lands.
    - **Total outage:** do the **unplugged version** below.

??? note "Unplugged version (no devices)"
    Play **"Be the Computer."** You (or a kid) are the AI model. Another kid is the **code**.
    On paper, fill in the **Cell-2 blanks**: NAME, PERSONALITY, PURPOSE, RULE. The "code" kid
    reads out the system prompt ("You are *Sparky*, cheerful and silly, you help with times
    tables, your rule is...") **plus** a user message ("What's 6×7?"). The "model" kid must
    answer **in that personality and obeying that rule** (hint first, never mean). Then change
    just the PERSONALITY to "grumpy pirate," keep everything else, and re-read — the answer
    changes. Big point: *the system prompt (Cell 2) is what turns a general AI into THIS
    assistant.* Same lesson, zero tech.

---

## 0:50–0:58 — Capstone step: make it real & save it 🎯

Bring the energy together. Every kid now gets their **own** assistant running with their
**own** persona, then **saves it**:

1. Confirm Cell 2 has **their** real persona (from Week 2), not the demo `Sparky`.
2. **File → Save a copy in Drive**, into the **facilitator's cohort folder**, named
   **`assistant-<name>.ipynb`** (e.g. `assistant-maya.ipynb`).
3. They jot the file name on their handout so it survives to Week 4.

> 🗣️ **Talking point:** "This notebook *is* your assistant now — real software with your
> personality inside it. Save it carefully: **next week you show it off.**"

If a kid couldn't run live (tech issues), save their **Cell-2 values from the handout** into
the folder so nothing is lost.

---

## 0:58–1:00 — Wrap & tease 👋

- **One-line recap:** "You **commanded an AI with real code** — and changing **one cell**
  made it *yours*."
- **Safety reminder:** the **API key is a secret** the facilitator holds; same golden rule —
  **no secrets** into any AI.
- **Tease Week 4:** "Next time: **Smart & safe AI citizen + Showcase** — you'll make your bot
  **safer** with better guardrails, then **show it off**."

---

## Common kid questions today

- *"Did I really write code?"* → Yes! You edited real Python and ran it. You changed the
  variables that command the AI — that's coding.
- *"Where is the AI? Is it in my laptop?"* → No. It lives on a big computer far away. Your
  code asks it through an **API**, like ordering through a waiter.
- *"Can I see the key?"* → No — and that's the point. A key is a secret password for code.
  *I* hold it so it stays safe.
- *"I broke it!"* → You almost certainly didn't. Re-run the cell. If a `?` or red text shows,
  it's just a hiccup — run it again, top to bottom.
- *"Why does mine sound different from my friend's?"* → Because only **Cell 2** changed. Same
  code, your personality.

## Facilitator self-check (did the week land?)

- [ ] Every kid edited **Cell 2** and **chatted** with their own assistant (real or fallback).
- [ ] Every kid can say an **API** lets code ask an AI for a reply, and **the facilitator
      holds the key**.
- [ ] No kid ever saw or typed a raw API key.
- [ ] Every kid's notebook is **saved** as `assistant-<name>.ipynb` in the facilitator folder.
- [ ] You confirmed model access worked on the canary **before** kids arrived.
