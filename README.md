# AI Young Builders Club 🤖

A **4-weekend, one-hour-a-week** hands-on AI literacy program for kids aged **11–13**.
Small groups (≤8), each kid on a laptop, using real AI tools under supervision. Over four
sessions every kid designs, builds, and presents **their own AI assistant**.

> 🌐 **Live site:** https://sreenivas-sadhu-prabhakara.github.io/ai-young-builders-club/

This repository holds the full curriculum and all reference materials: facilitator
run-sheets, slide outlines, printable kid handouts, a glossary, prompting cheat sheet,
ethics primer, a ready-to-run Colab notebook, plus setup, safety, and consent docs.

## What's inside

| Week | Theme | The "wow" activity | Capstone step |
|------|-------|--------------------|----------------|
| 1 | What even *is* AI? | Train a model in the browser (Teachable Machine) | Pick your assistant's purpose |
| 2 | Talking machines | Prompt a chatbot & generate images | Design its personality + system prompt |
| 3 | A taste of real code | Run Python in Colab that calls an AI | Get your assistant running in code |
| 4 | Smart & safe AI citizen | Red-team your bot, add a guardrail | **Showcase** to the group & parents |

- **Curriculum** → `docs/week-1` … `docs/week-4` (overview, facilitator guide, slides, handout)
- **Reference materials** → `docs/resources` (glossary, prompt cheat sheet, ethics primer, Colab notebook)
- **For facilitators** → `docs/for-facilitators` (setup, safety & consent, FAQ, rubric)
- **Program design / pitch** → [`DESIGN.md`](./DESIGN.md) — the doc for co-founder discussion

## Run the site locally

```bash
python3 -m venv .venv
./.venv/bin/pip install -r requirements.txt
./.venv/bin/python -m mkdocs serve
# open http://127.0.0.1:8000
```

## How it's published

Every push to `main` triggers `.github/workflows/deploy.yml`, which builds the MkDocs site
(`--strict`) and deploys it to GitHub Pages. Content is plain Markdown under `docs/` — edit a
file, push, and the site updates automatically.

## License

Curriculum content is released under **[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)** —
free to use, adapt, and share with attribution. See [`LICENSE`](./LICENSE).
