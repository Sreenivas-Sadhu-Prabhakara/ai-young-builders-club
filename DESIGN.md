# AI Young Builders Club — Program Design

*A discussion document for the founding team. Last updated 2026-06-27.*

This is the "why and how" behind the curriculum. The published site (`docs/`) is the
"what" — the actual sessions, handouts, and reference materials. Read this first to
align on intent; edit it freely as we pressure-test the idea together.

---

## 1. One-line pitch

> A 4-weekend club where 11–13 year olds go from *"AI is magic"* to *"I built an AI
> assistant and I know how it works"* — one hour at a time.

## 2. Who it's for

- **Age:** 11–13 (early teens). Language and examples pitched here; older kids can go
  deeper via optional "Go Further" challenges, younger kids can stick to the core path.
- **Group size:** ≤8 — small enough that one facilitator can supervise live tool use and
  give everyone individual attention.
- **Setup:** Each kid has a laptop with internet. Tools are used **with supervision**.
- **Prerequisites:** None. No prior coding. Curiosity and a willingness to type.

## 3. What success looks like

By the end of Week 4, every kid can:

1. **Explain in their own words** what AI is — that it *learns from examples* rather than
   following rules a human typed, and that it can be confidently wrong.
2. **Use AI tools deliberately** — write a clear prompt, judge whether an answer is
   trustworthy, and generate text/images on purpose rather than by luck.
3. **Show something they built** — their own AI assistant, with a personality they
   designed, running from a few lines of Python they can read.
4. **Act as a responsible AI citizen** — name real risks (bias, deepfakes, privacy,
   hallucination) and describe one thing they'd do to use AI safely.

We measure success not by a test but by the **Week 4 showcase**: can each kid stand up,
demo their assistant, and answer "how does it work?" and "how could it go wrong?"

## 4. Design principles

- **Build something real, fast.** Every single session ends with the kid's own project
  further along. Wonder comes from making, not from listening.
- **One hour is sacred.** Each session is timeboxed to the minute (see facilitator
  run-sheets). The concept portion is short; hands-on is the majority.
- **Concrete before abstract.** Kids train a model *before* we explain training. They
  prompt a chatbot *before* we explain tokens. The mental model lands on top of an
  experience they already had.
- **Safety is designed in, not bolted on.** Supervised tool use, no personal data in
  prompts, account/setup handled by the facilitator, and a whole session on responsible
  use. See `docs/for-facilitators/safety.md`.
- **Inclusive by default, stretchy on demand.** The core path needs no typing of code
  beyond fill-in-the-blanks. Keen kids get optional "Go Further" extensions.
- **Catch-up friendly.** Each week opens with a 5-minute recap path so a kid who missed
  a session can rejoin without being lost.

## 5. The spine: one capstone, four layers

Everything builds toward **"Build your own AI Assistant."** Each week adds one layer:

| Week | Theme | Big idea kids leave with | Hands-on "wow" | Capstone layer added |
|------|-------|--------------------------|----------------|----------------------|
| **1** | What even *is* AI? | AI learns from examples; it's pattern-matching, not rules. | Train an image/sound model in the browser with Teachable Machine. | **Purpose** — what will my assistant help with? |
| **2** | Talking machines | Chatbots predict the next word; prompts steer them; they can be *confidently wrong* and biased. | Prompt a supervised chatbot; generate images; compare results. | **Personality + system prompt** — how does it talk? |
| **3** | A taste of real code | From clicking to coding; an "API" lets a few lines of Python command an AI. | A fill-in-the-blank Colab notebook that actually calls a model and replies. | **Running in code** — the assistant comes alive. |
| **4** | Smart & safe AI citizen | Ethics, deepfakes, privacy, limits, responsibility. | Red-team your own bot; add a guardrail. | **Showcase** — present to the group & parents. |

## 6. Pedagogical shape of every session (60 min)

| Time | Segment | Purpose |
|------|---------|---------|
| 0:00–0:10 | **Hook** | A demo, question, or game that creates curiosity for today's idea. |
| 0:10–0:25 | **Concept** | Short, concrete explanation of the big idea (slides + discussion). |
| 0:25–0:50 | **Hands-on** | The main activity — kids do the thing. |
| 0:50–0:58 | **Capstone step** | Apply today's skill to *their own* assistant. |
| 0:58–1:00 | **Wrap & tease** | One-sentence recap, save work, tease next week. |

## 7. Tooling choices (and why)

- **Teachable Machine (Week 1):** browser-based, no account, instant "I trained an AI"
  payoff. Perfect first contact.
- **A supervised chat + image tool (Week 2):** facilitator-driven accounts; kids drive the
  prompting. See setup guide for age-appropriate options and account handling.
- **Google Colab (Week 3):** zero local install, runs Python in the browser, easy to share
  a fill-in-the-blank notebook. The model call is brokered so kids never handle raw API
  keys (facilitator-provided key or a classroom proxy endpoint).
- **MkDocs Material (this site):** content is Markdown so non-developers can edit it;
  output is a polished, searchable, printable site that auto-deploys on push.

> **Open question for the team:** which chat/image tools do we standardize on, and do we
> run the Week 3 model calls through a hosted key or a classroom proxy? Captured in the
> "Decisions to finalize" section below.

## 8. Risks & mitigations

| Risk | Mitigation |
|------|------------|
| A kid sees inappropriate AI output | Supervised use, kid-safe tools, facilitator circulates, clear "flag it" rule. |
| Tech fails mid-session (wifi, account, quota) | Every facilitator guide has a "When tech breaks" fallback (offline/unplugged version). |
| Pace too fast/slow for mixed abilities | Core path + optional "Go Further"; buffer time built into run-sheets. |
| Kids over-trust AI | Hallucination & bias are taught explicitly in Weeks 2 and 4. |
| Privacy / personal data in prompts | "No real names, no secrets" rule taught Week 1, reinforced throughout. |
| A kid misses a week | 5-minute recap path opens each session. |

## 9. What we are deliberately NOT doing (YAGNI)

- No grades, exams, or homework.
- No deep math or neural-network internals.
- No building/training models from scratch beyond Teachable Machine.
- No personal accounts created by/for kids without guardian consent.
- No unsupervised use of open-ended AI tools.

## 10. Decisions to finalize with co-founder

- [ ] Final program name & branding (currently "AI Young Builders Club").
- [ ] Which specific chat + image tools we standardize on (cost, age policy, account model).
- [ ] Week 3 model access: hosted API key vs. classroom proxy endpoint.
- [ ] Guardian consent flow and data policy (draft in `docs/for-facilitators/safety.md`).
- [ ] Pilot cohort: when, where, who, and how we collect feedback.
- [ ] Pricing / free / sponsored, and whether this ties into our startup brand.

---

*Once these are settled, the site content in `docs/` is ready to run a pilot as-is.*
