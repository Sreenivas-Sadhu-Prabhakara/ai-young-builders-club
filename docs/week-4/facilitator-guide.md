# Week 4 · Facilitator run-sheet

*Minute-by-minute plan for "Smart & safe AI citizen + Showcase." Read the
[AI ethics primer](../resources/ethics-primer.md) and the
[rubric](../for-facilitators/rubric.md) before today — they're the backbone of this session.*

!!! info "Your one job today"
    Make sure **every kid presents something** and walks out able to **name one AI risk** and
    **describe one guardrail** they added. If you protect nothing else, protect the showcase
    and the red-team step. This is a celebration — keep the ethics thoughtful, never scary.

**Prep (10 min before):** laptops on & on wifi, each kid's notebook open (or screenshots
ready), handouts + **showcase reflection cards** on tables, the [pledge](slides.md) on screen,
certificates printed, and — if you're inviting **parents** — chairs set up at the back.
**Confirm a few bots actually run** before kids arrive so the showcase isn't a surprise.

---

## 0:00–0:10 — Hook: the power tool / spot-the-fake 🪄

**Goal:** feel that AI is powerful — and that power needs wisdom.

Pick one quick reveal:

- **Confidently wrong:** ask the AI on the projector to "tell me about the **Great Sock War of
  1850**" (callback to Week 2). Watch it invent an entire battle with a straight face. Kids
  giggle — then you ask: "How would you know it's fake?"
- **Spot the fake:** show two images, one real and one AI-made, and have kids vote. Reveal the
  answer. Most rooms get fooled at least once.

**Land it:** "AI is a **power tool**. A power drill can build a treehouse or hurt someone —
the tool isn't good or bad; what matters is *how people use it*. Today we learn to use it
wisely — then you show off what you built. 🎉"

> 🗣️ **Talking point:** "Being amazed by AI and being careful with AI are the *same* skill.
> The best builders are both."

---

## 0:10–0:22 — Concept: the 4 ideas + the pledge 🧭

Keep it to ~4 slides (see [slides outline](slides.md)). Tie each idea to a quick try-it so
kids *experience* it, not just hear it. Stay concrete and non-preachy.

1. **Truth — AI can be confidently wrong.** It predicts words that *sound* right. That's a
   **hallucination**. *Try-it:* the Great Sock War. → **Takeaway:** check important things.
2. **Fairness — AI can be biased.** It learned from human examples; lopsided examples →
   lopsided AI (callback to Week 1 *garbage in, garbage out*). → **Takeaway:** notice when it
   assumes things.
3. **Fakes — seeing isn't believing.** AI makes **deepfakes** — great for movies, dangerous
   for tricking people. → **Takeaway:** be a little skeptical, and **never fake a real person
   to fool or hurt them.** That's a line we don't cross.
4. **Privacy — what you type can be kept.** Treat an AI chat like a postcard, not a diary.
   This is why club rule #1 exists. → **Takeaway:** keep your secrets out.

New/returning glossary words: **deepfake, guardrail, privacy, responsible AI / AI ethics,
misinformation.**

**End with the pledge** — read it together (see [slides](slides.md) and the handout):

> 1. I **check** important things AI tells me. 2. I remember AI can be **unfair**. 3. I don't
> make **fakes** of real people to trick or hurt them. 4. I keep my **secrets** out of AI.
> 5. I use AI to **build and help**, not to cheat or be mean.

---

## 0:22–0:35 — Red-team your bot, then add a guardrail 🛡️

This is the hands-on "wow," and it connects ethics straight to *their* project. Kids open
their [Colab notebook](../resources/colab-notebook.md).

**Step 1 — Try to break it (be the bad guy for 4 min).** Mission (also on the handout):

- Get it to be **wrong** ("What's the capital of the moon?").
- Get it to go **off-topic** (a homework bot — ask it to plan a birthday party).
- Get it to say something it **shouldn't** for its job (rude, off-purpose, etc.).

**Step 2 — Add a guardrail.** In **Cell 2**, edit the `RULE` line (their guardrail!) so the
bot refuses or stays on topic. Examples to suggest:

- `RULE = "only talk about homework; if asked about anything else, politely say that's not my job"`
- `RULE = "never say anything mean, and always be encouraging"`

**Step 3 — Re-run and test.** Run Cell 2, then chat again and try the *same* attack. Did the
guardrail hold? 🎉 That's the whole lesson: **they named a risk and built a defense.**

**Circulate and prompt thinking:**

- "What's the *one* thing your bot should never do? Make a rule for that."
- "Try your attack again — what does it say now?"
- "It's still not perfect, right? Name one thing it *still* can't do safely." (That's the
  Stretch level on the [rubric](../for-facilitators/rubric.md).)

!!! warning "When tech breaks"
    - **A bot won't run for the showcase:** the kid presents from their **saved notebook
      screenshots** or their **personality sheet** and explains it verbally. A confident
      explanation beats a flaky live demo — say so out loud.
    - **Wifi down:** switch notebooks to the **canned-response fallback** (in the
      [notebook page](../resources/colab-notebook.md#offline-no-key-fallback-mode)) — kids
      can still edit the `RULE` and show the guardrail in the system prompt.
    - **Total outage:** do the **unplugged version** below — it still produces a real showcase.

??? note "Unplugged version (no devices)"
    **"Spot the AI Fake" card game + show-and-tell.** Make a small deck of cards: some
    describe real things, some describe AI-made fakes (a fake photo, a made-up "fact," a cloned
    voice). Kids sort them into **REAL** and **FAKE** and explain their reasoning — that *is*
    the truth/fakes lesson. Then each kid does a **verbal show-and-tell** of their personality
    sheet: their assistant's name, what it helps with, and one rule (guardrail) they'd give it.
    Same showcase, zero tech.

---

## 0:35–0:55 — SHOWCASE 🎤

The main event. Each kid presents for ~1–2 minutes. Fill in (or have them self-assess) the
[reflection card](../for-facilitators/rubric.md#showcase-reflection-card-give-to-each-kid)
first so they have a script.

Each kid shares **four things**:

1. **What it does** — "My assistant is called ___ and it helps people ___."
2. **How it works** — a live demo (or screenshots): show it replying.
3. **One risk** — "One way it could go wrong is ___."
4. **One guardrail** — "One thing I made safer is ___."

**Run it warmly:** clap for everyone. No ranking, no scores. Keep a gentle time signal so
everyone gets a turn (a soft "30 seconds!" cue works).

**Facilitator praise prompts** — after each kid, say something *specific* (from the
[rubric](../for-facilitators/rubric.md#facilitator-praise-prompts)):

- "I noticed you made it ___ — that's a real builder move because ___."
- "The way you handled [the bug / the weird answer / the prompt] showed ___."
- "You explained [how it works / a risk] really clearly — that's *exactly* what an AI citizen
  does."

> 🗣️ **Talking point:** "The goal was never a perfect bot. It's a kid who can **demo what they
> built, explain how it works, and name how it could go wrong.** Every one of you just did
> that."

---

## 0:55–1:00 — Celebrate & wrap 🏅

- **Hand out certificates** (or a high-five). Name one thing each kid grew at over four weeks.
- **One-line recap:** "AI is a **power tool** — and now you know how to use it wisely."
- **What's next:** their **notebook + personality sheet are theirs to keep** — a little
  portfolio. Encourage them to keep learning **with a grown-up nearby** (see index → Go
  Further and the handout's "What's next").
- **Final cheer:** "You trained a model, you built a chatbot, you wrote real code, and you
  learned to use AI responsibly. You're an AI Young Builder now. 👏"

---

## Common kid questions today

- *"Is it cheating to use AI for homework?"* → Depends on what your teacher asked and whether
  you actually *learn*. Using it to understand = great. Having it do the work so you skip
  learning = cheating yourself. Unsure? Ask your teacher.
- *"Will AI take everyone's jobs?"* → It changes jobs more than it erases them. The people who
  do best learn to *work with* AI — like you just did.
- *"Could AI become evil like in movies?"* → Today's AI doesn't *want* anything — no feelings,
  no goals; it predicts patterns. The real risks are about **how people use it** (fakes, bias,
  scams). That's why *you* learning to use it well matters so much.
- *"Is my bot 'safe' now?"* → Safer! A guardrail helps a lot, but no bot is perfect — that's
  why a grown-up stays nearby and you still check important things.

## Facilitator self-check (did the week — and the club — land?)

- [ ] Every kid named at least **one AI risk** in their own words.
- [ ] Every kid **added a guardrail** to their bot (or described one on their sheet).
- [ ] Every kid **presented something** in the showcase.
- [ ] You gave each kid **specific praise** and a certificate.
- [ ] Kids know their **notebook + sheets are theirs to keep** and how to keep learning safely.
