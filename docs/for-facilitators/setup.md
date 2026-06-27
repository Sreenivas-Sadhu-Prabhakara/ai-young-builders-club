# Setup & accounts

*Do this once before Week 1, then a 5-minute check before each session.*

You do **not** need to be an AI expert to run this club. You do need the room, the
devices, and the accounts ready so the hour is spent building, not troubleshooting.

## One-time setup (before the club starts)

- [ ] **Read** the [Safety, consent & parent letter](safety.md) and send the consent form home.
- [ ] **Devices:** one laptop per kid + a facilitator laptop connected to a projector/screen.
- [ ] **Internet:** test wifi with all devices on it at once (bandwidth matters for image tools).
- [ ] **Browser:** install/update a modern browser (Chrome or Edge work best for Teachable Machine and Colab).
- [ ] **Decide your tool stack** (see the table below) and create the **facilitator-managed accounts**.
- [ ] **Bookmarks:** add the day's tool links to the browser bookmark bar on every laptop.
- [ ] **Dry run:** do each week's activity yourself once. This is the single best prep you can do.
- [ ] **Print** the kid handouts for each week (see each week's *Kid handout* page).

## Tool stack by week

| Week | Tool | Account needed? | Notes |
|------|------|-----------------|-------|
| 1 | [Teachable Machine](https://teachablemachine.withgoogle.com) | **No account** | Runs in the browser. Webcam permission needed. |
| 2 | A supervised **chatbot** + **image generator** | **Facilitator-managed** | Kids drive the prompt; the facilitator owns the account. See options below. |
| 3 | [Google Colab](https://colab.research.google.com) + a model API | **Google account; one API key** | Kids run a notebook; the **facilitator's key** is brokered (see "Model access"). |
| 4 | Same as Weeks 2–3 | — | Plus offline red-team worksheet. |

!!! warning "Account rule"
    **Kids do not create their own accounts for AI tools.** Accounts are created and owned
    by the facilitator, or kids use no-login tools. This keeps you compliant with age
    policies and keeps kids' data out of third-party services. See [Safety](safety.md).

### Choosing the Week 2 chat & image tools

Pick tools that (a) allow your use with the kids' ages under your supervision, (b) have a
content filter, and (c) you can drive from a single facilitator account on the projector,
with kids suggesting prompts — or on kid laptops logged into a facilitator-managed account.

> 🔧 **Team decision (see `DESIGN.md`):** standardize on one chat tool and one image tool
> before the pilot, then list them here with exact links and login steps.

Whatever you choose, the *teaching* is tool-agnostic — the handouts talk about "the
chatbot" and "the image generator," not a brand.

### Model access for Week 3 (important)

Week 3's Colab notebook calls a real AI model. Kids must **never** see or paste a raw API
key. Choose one of these brokering patterns:

=== "Option A — Classroom proxy (recommended)"
    Run a small proxy endpoint that holds the key server-side; the notebook calls the
    proxy with no secret. Cleanest and safest — kids only ever see a plain URL.

    > If your organization already runs an OpenAI-compatible proxy (e.g. a LiteLLM
    > gateway), point the notebook's `BASE_URL` at it and use a throwaway classroom token.

=== "Option B — Facilitator-entered key"
    The facilitator opens each kid's notebook and pastes the key into Colab's **Secrets**
    panel (the 🔑 icon), so it's never typed into a code cell or shared on screen. Remove
    it after the session.

=== "Option C — Fully offline fallback"
    If no model access is available, use the notebook's **canned-response mode** (a built-in
    dictionary of replies) so kids still edit the persona and see the loop work. Details in
    [the Colab notebook page](../resources/colab-notebook.md).

## Before each session (5-minute check)

- [ ] All laptops on, charged or plugged in, on wifi.
- [ ] Today's tool opens and works on **one** laptop (your canary).
- [ ] Projector mirrors your screen; volume works if there's audio.
- [ ] Handouts printed and on the tables.
- [ ] Kids' saved work from last week is reachable (see "Saving work" below).

## Saving kids' work between sessions

The capstone builds across four weeks, so work must persist:

- **Week 1 (Teachable Machine):** export the model or screenshot it — but the lasting
  artifact is the **capstone planning sheet** (their assistant's purpose). Keep these.
- **Week 2 (personality + system prompt):** written on the handout **and** typed into a
  shared doc/folder the facilitator controls (one doc per kid).
- **Week 3 (Colab):** each kid saves a **copy** of the notebook to the facilitator's Google
  Drive, named `assistant-<kidname>.ipynb`.
- **Week 4:** kids present from their saved notebook + personality sheet.

!!! tip "Keep a facilitator folder"
    Make one cloud folder for the cohort with a subfolder per kid. Everything lands there.
    It doubles as the showcase material for Week 4 and a portfolio kids can take home.

## If you're short on devices or time

- **Fewer laptops than kids?** Pair them up — pairing actually helps discussion. Make sure
  both kids take a turn driving.
- **Only a projector, no kid laptops?** Run the [unplugged fallbacks](faq.md#when-tech-breaks)
  in each facilitator guide; the capstone planning still works on paper, and Week 3 becomes
  a guided live demo.
