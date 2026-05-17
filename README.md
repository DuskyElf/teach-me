# teach-me

> [!NOTE]
> Recent updates brought major improvements in surfacing pitfalls. To get the latest version, run:
> ```bash
> npx skills update duskyelf/teach-me
> ```
> Literature reivew template got updates, please re-generate your literature-reviews

[![skills.sh](https://skills.sh/b/duskyelf/teach-me)](https://skills.sh/duskyelf/teach-me)

A personal learning environment that questions your answers, not just answers your questions. It helps you find your **unknown unknowns**, by tacking what you've mastered, what you're fuzzy on, and comparing it with discussions of experts.

Inspired by the [/grill-me](https://github.com/mattpocock/skills/blob/main/skills/productivity/grill-me/SKILL.md) and [/grill-with-docs](https://github.com/mattpocock/skills/blob/main/skills/engineering/grill-with-docs/SKILL.md) skill by Matt Pocock.

## It's just Two skills

```
/literature-review [topic|question|subject]
```
Builds a source-backed literature review with consensus, tensions, and gaps. Use when you want academic grounding, or needs a high-quality source map before a learning session.

```
/teach-me [topic|question] [research-paper|article|literature-review-file]
```
Starts a Socratic session which grills you through your own understanding and knowledge gaps and forces you to think the answers yourself.

## Quickstart

```bash
npx skills add duskyelf/teach-me
```
**Or Manually:**
```bash
git clone https://github.com/DuskyElf/teach-me.git
cd teach-me
```

## It's for; tldr
- Finding what's the state of consensus at the moment and where the tensions are
- Understanding a specific research paper or a broad concept intuitively
- Probing your knowledge gaps before an exam

## How it works

Everything here runs on one idea: you don't learn by being told. You learn by being questioned.

The skill starts with research — it finds what's actually contested in your topic, not just what's settled. Those contested points are called tensions. Then it asks you questions that sit right inside those tensions. It watches how you respond, tracks your level, and keeps a diary so you can continue later.

The interesting part is how it measures progress. It's not about recall. It's about whether you can hold the tension without picking a side too early. Whether you notice when you're fuzzy. Whether you can notice your own bias when the questions press on it.

[Read more...](docs/how-it-works.md)
