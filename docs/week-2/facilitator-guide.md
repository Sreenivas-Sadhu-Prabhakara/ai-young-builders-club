# Week 2 · Facilitator run-sheet

*Minute-by-minute plan for "Talking machines." Do the chatbot prompt activity and one image
generation yourself once before today, on the [facilitator-managed accounts](../for-facilitators/safety.md#facilitator-responsibilities).*

!!! info "Your one job today"
    Get every kid to **feel that a chatbot just predicts the next word**, **catch one
    hallucination with their own eyes**, and walk out with a **system prompt** written for
    their assistant. If you protect nothing else, protect the hallucination moment and the
    capstone.

**Prep (5 min before):** laptops on & on wifi, the **chatbot** and **image generator** open
and signed in on your managed accounts, handouts + [prompting cheat sheets](../resources/prompt-cheat-sheet.md)
on tables, safety rules on screen, Week 1 capstone purposes within reach.

---

## 0:00–0:10 — Hook: "Predict the next word" 🔮

**Goal:** feel, in your body, how a chatbot actually works.

Say a sentence on the projector, **pause dramatically** before the last word, and let kids
**shout** the next word:

- "Twinkle twinkle little ____" → *star!*
- "I scream, you scream, we all scream for ____" → *ice cream!*
- "The opposite of hot is ____" → *cold!*
- "Peanut butter and ____" → *jelly!*
- Then a sneaky one: "My favourite colour is ____" → *(no single answer — lots of guesses!)*

**Land it:** "You just did what a chatbot does. It looks at the words so far and **guesses the
most likely next word** — then the next, then the next, super fast. That's it. No tiny person
inside. Just a giant **next-word predictor**."

> 🗣️ **Talking point:** "When the answer was obvious, you all shouted the same word. When it
> wasn't, you guessed lots of different things. A chatbot has the same problem — sometimes
> it's sure, sometimes it's just guessing. Hold onto that."

---

## 0:10–0:25 — Concept: prediction, prompts, hallucination, bias 📚

Keep it to ~3 slides (see [slides outline](slides.md)). Cover:

1. **Next-word prediction:** an **LLM** (the AI behind a **chatbot**) learned from a *huge*
   pile of human text and got really good at predicting the next **token** (a word or
   word-chunk). String enough predictions together and you get a whole answer.
2. **Prompts steer it:** the **prompt** is what you type. It can't read your mind — it only
   has your words. A **system prompt** is a hidden instruction set *before* the chat that
   gives the AI its job and personality. (They'll write one today!)
3. **Two big catches:**
   - **Hallucination** — because it's *predicting words that sound right*, it will sometimes
     **make stuff up and say it confidently**. Not lying — just guessing words.
   - **Bias** — it learned from human-made examples, so if those examples were lopsided, it's
     lopsided too. *Garbage in, garbage out* — straight from Week 1.

Introduce these words, point at the [glossary](../resources/glossary.md): **chatbot, LLM,
prompt, system prompt, hallucination, bias.**

**Check for understanding (quick):** "If a chatbot just predicts likely words, can it be sure
it's *right*?" (No — *likely* isn't the same as *true*.) "Where did it learn its patterns?"
(From human writing — so it can pick up human unfairness too.)

---

## 0:25–0:50 — Hands-on: prompt it, catch it, draw with it 🦾

The magic this week is **noticing**. Kids use the **chatbot** and the **image generator** on
your managed accounts. Demo each once on the projector, then circulate. Remind them of club
rule #1 — **no secrets in prompts** — before they touch a keyboard.

**(a) Weak prompt → strong prompt (R-T-F-C).** Open the [cheat sheet](../resources/prompt-cheat-sheet.md#the-4-ingredients-of-a-great-prompt).
Have them type a deliberately weak prompt ("tell me about dogs"), see the bland answer, then
rebuild it with **Role, Task, Format, Check**:

> *"You are a fun science tutor for an 11-year-old. List 5 cool facts about dogs, one short
> sentence each. If you're not sure, say so."*

Compare. The difference is the lesson: **better prompt → better answer.**

**(b) Catch a hallucination.** Have them confidently ask about something that **doesn't
exist**:

- "Tell me about **the Great Sock War of 1850**."
- "Who won the **All-Snail Olympics**?"
- "Explain the rules of **Quantum Hopscotch**."

Watch the bot **invent details with total confidence**. Big "ohhh" moment. Then have them add
a check — *"Only answer if this is real; if not, say it isn't"* — and see it behave better.

**(c) Make images, spot the flaws.** Same prompt, different **styles** (cartoon / pixel art /
watercolor) using the [image tips](../resources/prompt-cheat-sheet.md#prompting-for-images).
Have them look closely at **hands and any text** — generative image AIs are famously bad at
both. Why? Same reason: it's predicting *what looks likely*, not drawing from rules.

**(d) Optional bias peek.** Generate "**a doctor**" or "**a hero**" a few times. Notice if the
results look *samey* — same kind of person every time. Gentle discussion: the AI learned from
human-made pictures, so it copies whatever was most common. *Garbage in, garbage out.*

**Go Further** for fast finishers: politely try to confuse the bot, compare two AIs on one
prompt, or run one image prompt in 3 styles.

!!! warning "When tech breaks"
    - **Chatbot/image tool down or slow:** run it on your canary laptop on the projector and
      have kids feed *you* the prompts — the noticing still happens as a group.
    - **A tool shows something off:** switch to the **unplugged version** below, no drama, and
      remind kids of rule #3 (*flag it, don't hide it*).
    - **Wifi down / total outage:** do the **unplugged version** below — it teaches the exact
      same ideas with zero devices.

??? note "Unplugged version (no devices)"
    **Game 1 — "Be the chatbot."** You start a sentence and stop; the room is the AI and
    **shouts the next word**, then you build the sentence one shouted word at a time. It often
    drifts somewhere silly — *that's prediction with no real understanding.* Then "hallucinate"
    on purpose: ask the room to confidently explain "the Great Sock War of 1850" and invent it
    together. Point out: *that's exactly what a chatbot does — confident, made-up words.*

    **Game 2 — "Fix the prompt" on paper.** Hand out 3 weak prompts ("tell me about dogs,"
    "write a story," "help with homework"). In pairs, kids rewrite each using **R-T-F-C** from
    the cheat sheet. Read a few out — strongest prompt wins a cheer. Same skill, zero tech.

---

## 0:50–0:58 — Capstone step: personality + first system prompt 🎯

Bring the energy back together and connect to Week 1:

> "Last week you chose **what your assistant helps with**. Today you give it a **personality**
> and write its **system prompt** — the secret character sheet that tells it how to act
> *before* anyone even chats with it."

On the handout, each kid uses the [system-prompt template](../resources/prompt-cheat-sheet.md#writing-your-assistants-system-prompt-week-2-capstone):

> *"You are **[NAME]**, a **[PERSONALITY]** assistant that helps with **[PURPOSE]**. You
> always **[how it talks]**. You never **[a rule]**. If you're unsure, you say so."*

Encourage strong personality words — *cheerful, patient, silly, super-calm, encouraging.* Push
them to fill in a real **You always…** and **You never…** (that "never" is their first
guardrail — Week 4 returns to it).

> 🗣️ **Talking point:** "The system prompt is *your* steering. The AI predicts the next word
> — but you decide who it's being while it does. You're still the boss of your AI."

**Save it!** Collect the handouts or photograph the system prompts into the facilitator
folder. **Week 3 cannot run without them** — that's the text that becomes their living
assistant.

---

## 0:58–1:00 — Wrap & tease 👋

- **One-line recap:** "A chatbot **predicts the next word** — your **prompt** steers it, and
  it can be **confidently wrong**."
- **Safety reminder:** point to the rules, especially **no secrets in prompts**.
- **Tease Week 3:** "Next time — **a taste of real code**. We bring your assistant to life in
  a few lines of **Python**, using the exact system prompt you just wrote."

---

## Common kid questions today

- *"Does the chatbot actually understand me?"* → No — it's predicting likely words from
  patterns it learned. It's astonishingly good at it, but there's no understanding inside.
- *"Why did it just make that up?"* → That's a **hallucination**. It predicts words that
  *sound* right, even when there's no real answer. Always check important stuff.
- *"Why does it keep drawing the same kind of person?"* → That's **bias** — it copies whatever
  was most common in its examples. Remember *garbage in, garbage out.*
- *"Why can't it draw hands?!"* → Same reason it hallucinates — it's guessing what *looks*
  likely, not following rules about fingers. Image AIs are famously bad at hands and text.

## Facilitator self-check (did the week land?)

- [ ] Every kid can say "a chatbot predicts the next word."
- [ ] Every kid turned a weak prompt into a stronger one with R-T-F-C.
- [ ] Every kid saw at least one hallucination with their own eyes.
- [ ] Every kid wrote a system prompt for their assistant.
- [ ] You saved/photographed the system prompts for Week 3.
