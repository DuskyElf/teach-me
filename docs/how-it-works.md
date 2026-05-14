# How It Works

The whole thing runs on one idea: you don't learn by being told. You learn by being questioned. And the questions that matter most live inside tensions.

## Two Skills, One Flow

`/literature-review` goes first. It searches across Semantic Scholar, web articles, videos, and Wikipedia to build a map of your topic: what consensus exists, where researchers actually disagree, and what's still unclear. When it saves its literature review, it follows a shape `/teach-me` can use directly:

- **Summary**: 2-3 sentences that answer the question at a high level
- **Findings**: each finding tagged as consensus or having tension underneath
- **Tensions**: the contested points, with what each side argues
- **Sources**: which papers were kept and why, which were dropped
- **Gaps**: what's still unclear or weakly supported

A good gap is not a failure. It's a signal for where the session should be careful or exploratory.

Research stays separate because it's a different cognitive workflow. Research casts a wide net, scores sources, surfaces contradictions. Tutoring probes understanding through dialogue. Mixing them would bloat the experience or shallow out both.

`/teach-me` starts a session with that literature review as a foundation. It builds a curriculum, asks questions, tracks your level, and keeps a diary so you can come back later.

## Tensions vs Consensus

Every topic has two layers. There's the surface layer where experts agree on facts, definitions, and methods. Then there's the deeper layer where researchers actively disagree and no one has settled the answer yet.

That deeper layer is where the real learning happens.

**Consensus** is settled ground. It feels safe, but it doesn't test you.

**Tension** is contested ground. It's uncomfortable. It's where two smart people can read the same evidence and come to different conclusions. And that's exactly why it matters. If you can hold a tension without collapsing it into one side, you understand something that goes beyond memorizing facts.

The test for a real tension: would researchers publish papers arguing for each side? If yes, that's a tension worth sitting in.

A branch is where both sides exist and researchers agree both are valid. A tension is where researchers argue about which side is right, or whether the question itself is framed correctly.

Sometimes a tension dissolves when you go deep enough — both sides are solving the same underlying problem, just from different angles. The skill probes for this.

## The Curriculum is a Tree

The curriculum isn't a list of topics. It's a tree built by extracting from the literature review:

- **Root** — your starting point
- **Branches** — surface splits from the findings (researchers agree both exist)
- **Tensions** — the contested points underneath the branches, drawn from the review's Tensions section
- **Leaves** — fine-grained questions at the edges
- **Paths** — a specific route from root to a leaf

The literature review doesn't hand over questions. It hands over findings tagged as consensus or tension-underneath. Teach-me extracts those into a tree: each finding becomes a branch, each flagged tension surfaces underneath it, and the tree grows as you explore. When you reach the end of a path, the skill offers to explore a sibling branch or go deeper. The tree is never done — it unfolds as you learn.

## Levels

The skill tracks your understanding against how you handle tension, not just recall or self-report.

**Unknown**: You haven't met this topic yet.

**Confused**: You've heard of it, but your understanding is fuzzy or copied from somewhere else. You can repeat it back, but you can't move it around.

**Aware**: You can explain it in your own words and name the main tension without instantly picking a side.

**Confident**: You can navigate the tension, notice your own bias, and respond to challenge without falling apart.

The goal isn't to reach Confident on every topic. The goal is to notice where you're fuzzy and stay honest about it. Aware is useful already.

One more thing: levels aren't self-reported. The tutor probes your understanding of the tension even when you say you know something. Overconfidence is part of the lesson.

Here's what the levels look like on the same topic — "is Python readable?"

**Confused**: "Python is readable because it uses whitespace." Press on it: "What makes whitespace readable?" — silence. They can repeat the claim but can't move it around.

**Aware**: "Python's readability is contested. One side says enforced formatting reduces friction. The other side says it's just a convention — any language with enforced formatting would have the same benefit. I don't have a strong opinion yet."

**Confident**: "I'm biased toward thinking readability is about ecosystem, not syntax. That's a form of confirmation bias — I've learned to associate 'readable' with 'tools I trust.' I can articulate the other side charitably."

## The Flow

**Session start.** The tutor reads your starting point exactly as you wrote it — your question, topic, or paper. It builds a curriculum from the literature review if one exists. Then it asks: "What do you already know about these?" All topics default to Unknown. The tutor probes your answer to find where you're fuzzy and assess your level.

**During the session.** The tutor asks questions, watches how you handle each tension, and updates your level as you move. The tutor shifts between three modes based on how you're doing:

- **Socratic** (default): questions only, never answers
- **Curious Guide**: offers one reframe when you're stuck — still your insight to have
- **Devil's Advocate**: pushes hard on your positions when you're confident

The tutor announces shifts: "I'm shifting to Curious Guide." You can also trigger changes yourself:
- Stuck? Say "help me" or "I don't get this"
- Ready for pressure? Say "let's debate" or "I understand this"
- Over the pressure? Say "you're confusing me" or "too much"

The tutor also watches for fuzzy language — when you use a word in a way that shifts meaning, it catches it and names it. That's not pedantic, it's a gift. It's the moment where you realize you've been reasoning without anchors.

The tutor writes remarks at meaningful moments — breakthroughs, confusions, biases you noticed. Not a transcript, just the useful parts.

You're allowed to say "I don't know." A partial session is still a successful session. If you're exhausted, the tutor lets you stop.

**Wrap-up.** The tutor updates the diary, walks you through what you covered, marks the session complete or incomplete. Incomplete means there are still paths worth exploring. You can come back.

**Coming back.** When you continue a previous session, the tutor loads the diary — which is the curriculum's persistent form. It gives a brief recap and picks up where you left off. The diary is the curriculum. It grows across visits.

## The Diary

Everything lives in a diary file. It captures your starting point, the topics you explored, your level on each, the tensions you engaged with, and any remarks from moments of confusion or breakthrough. It grows across visits — the tree you start building in one session is still there when you return.

```markdown
# [filename]

## Starting Point
[verbatim user input] [link to literature-review file]

## Topics
- [ ] Root topic
  - level: Unknown | Confused | Aware | Confident
  - branches:
    - [ ] Sub-topic A (uncontested)
      - level: Unknown
    - [ ] Sub-topic B (has tension)
      - tensions:
        - [ ] Real tension: what researchers disagree on
      - level: Unknown

## Current Topic
[active branch or tension]

## Remarks
- **Topic**: brief note about confusion, insight, bias, or breakthrough

## Current State
INCOMPLETE | COMPLETE
```

The diary is a working document, not a transcript.