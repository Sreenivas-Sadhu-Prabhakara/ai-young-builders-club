# Capstone code (Colab notebook)

*This is the Week 3 notebook — the one that brings each kid's assistant to life in real
Python. It's written as **fill-in-the-blanks**: kids change a few clearly-marked lines and
run it.*

!!! tip "Download the ready-to-run notebook"
    📓 **[Download `assistant_starter.ipynb`](assistant_starter.ipynb)** and upload it to
    [Google Colab](https://colab.research.google.com) (File → Upload notebook), or open it
    from the facilitator's Drive. The code below is the same thing, shown for reference.

## How the notebook is structured

It has just **four cells**, each with a clear job. Kids only ever edit **Cell 2**.

| Cell | What it does | Kids edit it? |
|------|--------------|----------------|
| 1 | Setup — connects to the AI model (facilitator handles the key) | No |
| 2 | **Your assistant's personality** — the part kids customize | **Yes!** |
| 3 | The "brain loop" — sends messages to the AI and prints replies | No (but they can read it) |
| 4 | Chat with your assistant! | They run it & talk to their bot |

This mirrors the mental model from Week 2: the **system prompt** (Cell 2) shapes a general
AI into *their* assistant.

## The code (for reference)

### Cell 1 — Setup *(facilitator-managed; kids don't change this)*

```python
# --- Cell 1: Setup. The facilitator handles the key; you don't need to touch this. ---
# This connects our notebook to a real AI model using an OpenAI-compatible API.
!pip -q install openai

import os
from openai import OpenAI

# The facilitator provides these (e.g. via Colab Secrets 🔑 or a classroom proxy URL).
# Kids never see or type a raw key.
BASE_URL = os.environ.get("ABC_BASE_URL", "https://api.openai.com/v1")
API_KEY  = os.environ.get("ABC_API_KEY",  "set-by-facilitator")
MODEL    = os.environ.get("ABC_MODEL",    "gpt-4o-mini")

client = OpenAI(base_url=BASE_URL, api_key=API_KEY)
print("✅ Connected! Your assistant is ready to be brought to life.")
```

### Cell 2 — Your assistant's personality 🎨 *(THIS is the part you change!)*

```python
# --- Cell 2: YOUR ASSISTANT. Change the lines marked with 👉 ---

# 👉 1. Give your assistant a NAME:
ASSISTANT_NAME = "Sparky"

# 👉 2. Describe its PERSONALITY (cheerful? grumpy? super-formal? a pirate?):
PERSONALITY = "cheerful, patient, and a little bit silly"

# 👉 3. What does it HELP with? (its purpose from Week 1):
PURPOSE = "helping kids practice their times tables"

# 👉 4. One RULE it must always follow (your guardrail!):
RULE = "give a friendly hint before the answer, and never be mean"

# This builds your assistant's "system prompt" from your choices above.
SYSTEM_PROMPT = f"""
You are {ASSISTANT_NAME}, an assistant whose personality is {PERSONALITY}.
Your job is {PURPOSE}.
Important rule: {RULE}.
Keep your answers short and easy for an 11-year-old to read.
If you don't know something, say so instead of making it up.
"""

print(f"🤖 Meet {ASSISTANT_NAME}!")
print(SYSTEM_PROMPT)
```

### Cell 3 — The brain loop *(read it if you're curious!)*

```python
# --- Cell 3: The "brain". This sends your message to the AI and gets a reply. ---
def ask_assistant(user_message, history):
    # We send the personality (system prompt) + the conversation so far.
    messages = [{"role": "system", "content": SYSTEM_PROMPT}] + history
    messages.append({"role": "user", "content": user_message})

    response = client.chat.completions.create(model=MODEL, messages=messages)
    reply = response.choices[0].message.content

    # Remember this exchange so the assistant has memory of the chat.
    history.append({"role": "user", "content": user_message})
    history.append({"role": "assistant", "content": reply})
    return reply
```

### Cell 4 — Chat with your assistant! 💬

```python
# --- Cell 4: Talk to your creation! Type 'bye' to stop. ---
chat_history = []
print(f"Say hi to {ASSISTANT_NAME}! (type 'bye' to stop)\n")

while True:
    you = input("You: ")
    if you.strip().lower() in ("bye", "quit", "exit"):
        print(f"\n{ASSISTANT_NAME}: Bye! 👋")
        break
    answer = ask_assistant(you, chat_history)
    print(f"{ASSISTANT_NAME}: {answer}\n")
```

## Offline / no-key fallback mode

If there's no model access (wifi down, no key, quota hit), the downloadable notebook
includes a **canned-response mode** so kids can still edit Cell 2 and see the loop work.
Replace the body of `ask_assistant` with this version, which fakes replies using the
personality the kid set:

```python
# --- FALLBACK: no internet/key needed. Replies are faked, but the loop is real. ---
import random
def ask_assistant(user_message, history):
    openers = [
        f"As {ASSISTANT_NAME}, here's a hint:",
        f"{ASSISTANT_NAME} thinks...",
        "Great question! Let's see —",
    ]
    history.append({"role": "user", "content": user_message})
    reply = f"{random.choice(openers)} (pretend answer about {PURPOSE}!)"
    history.append({"role": "assistant", "content": reply})
    return reply
```

Kids still experience the key idea: **the same code becomes a different assistant when you
change the personality.** Swap to the real model when you can.

## Go Further challenges (for keen kids)

- **Change the greeting** in Cell 4 to something in your assistant's voice.
- **Add a second rule** to `SYSTEM_PROMPT` and see how the bot's behavior changes.
- **Make a "mood"** — add `MOOD = "excited"` in Cell 2 and weave it into the system prompt.
- **Give it a catchphrase** it has to use in every reply.

!!! warning "Key safety (facilitators)"
    Kids must never see or paste a raw API key. Use Colab **Secrets** (the 🔑 icon) or a
    classroom proxy URL. See [Setup → Model access](../for-facilitators/setup.md#model-access-for-week-3-important).
