# Week 3 · A taste of real code

!!! abstract "At a glance"
    - **Big idea:** You can **command an AI with a few lines of real code**. A model lives
      behind an **API**, and code can talk to it — so today we go from **clicking to coding**.
    - **Hands-on "wow":** Open a real Colab notebook, change ~4 lines, and watch your
      Week 2 assistant **come alive in Python** — you type a message, *your* bot replies.
    - **Capstone step:** Get your assistant running in code with its persona, then **save a
      copy** named `assistant-<name>.ipynb` for the Week 4 showcase.
    - **Kids leave saying:** *"I wrote real code that talks to an AI — same code, but I made
      it MY assistant."*

## Why this week comes now

In Week 1 kids *trained* an AI; in Week 2 they gave their assistant a **personality** and a
**system prompt**. This week we pull back the curtain: that personality isn't magic — it's a
few lines of text inside **real code** that *asks a model* for a reply. Kids stop being users
and become **builders**. The whole hour is built so that changing **one cell** turns a
general AI into *their* assistant: **same code, different personality.** That's the gut
feeling we're after — *I can command an AI.*

## Learning goals

By the end of the hour, each kid can:

- Explain that an **API** is one program asking another to do something — and that a **model
  lives behind an API** that code can talk to.
- Point to the four things they edit in **Cell 2** (`ASSISTANT_NAME`, `PERSONALITY`,
  `PURPOSE`, `RULE`) and say what each does.
- Run a real **Python** notebook in **Colab** and chat with the assistant they built.
- Say why an **API key** is a secret (a password for code) and that **the facilitator holds
  it — kids never touch it**.

## What you'll need

- One laptop per kid (or pairs), modern browser, signed in to a Google account.
- Projector for the facilitator + a working copy of the notebook open on your canary laptop.
- The [Week 3 Colab notebook](../resources/colab-notebook.md) — the downloadable
  `assistant_starter.ipynb`.
- **Model access sorted out** — pick a brokering pattern in
  [Setup → Model access for Week 3](../for-facilitators/setup.md#model-access-for-week-3-important).
  Kids must **never** see or paste a raw key.
- Each kid's **Week 2 personality + system prompt** (their `PERSONALITY`/`RULE` ideas).
- Printed [Week 3 handout](handout.md) (one per kid) and the
  [glossary](../resources/glossary.md) handy for the new words.

## The hour in one glance

| Time | Segment | What happens |
|------|---------|--------------|
| 0:00 | Hook | Week 2's assistant — now **alive in code** on the projector |
| 0:10 | Concept | Clicking → coding; Python, Colab, cells, API & API key |
| 0:25 | Hands-on | Run the notebook, edit **Cell 2**, chat with your bot |
| 0:50 | Capstone | Get it running with your persona + **save a copy** |
| 0:58 | Wrap | Recap + tease Week 4 |

→ Full detail in the **[facilitator run-sheet](facilitator-guide.md)**.

## The capstone this week

This is the week the assistant **becomes real software**. Each kid takes the personality and
system prompt they wrote in Week 2 and types it into **Cell 2** of the notebook —
`ASSISTANT_NAME`, `PERSONALITY`, `PURPOSE`, and one `RULE`. They run the four cells, chat
with their bot, then **save a copy of the notebook to the facilitator's Drive** named
`assistant-<name>.ipynb`. That saved notebook is the artifact they'll present in Week 4.

!!! tip "Nervous about code? Read this to the kids"
    It's **fill-in-the-blanks** — you change about **4 lines**, all marked with 👉. You
    **can't break anything**: if something looks weird, just **re-run the cell**. You're not
    writing code from scratch; you're **commanding** an AI with code that's already there.

## Go Further (for kids who race ahead)

These match the notebook's own challenges:

- **Change the greeting** in Cell 4 to something in your assistant's voice.
- **Add a second `RULE`** to the system prompt and see how the bot changes.
- **Add a `MOOD`** variable (like `MOOD = "excited"`) and weave it into the personality.
- **Give it a catchphrase** it has to use in every reply.

## Catch-up path *(for anyone who missed it later)*

In 5 minutes: open the facilitator's working notebook, type your Week 2 personality into
**Cell 2** (the four 👉 lines), run Cells 1–4, and chat with your bot. Hear the one big idea
(*code can command an AI through an API*), and save your copy as `assistant-<name>.ipynb`.
You're caught up.
