# teach-me

A personal learning environment that combines Socratic tutoring with research-grounded curriculum tracking. Enables discovery of unknown unknowns through guided questioning and persistent diary files.

## Language

**Starting Point**:
The user's verbatim input at session start — a question, topic request, or paper reference. Preserved exactly as stated. The key to the session.

**Subject**:
The folder name under `diary/` and `literature/` where related sessions and research live. Auto-detected from keywords, user can override. Flat structure, no nested subjects.
_Avoid_: category, domain, bucket

**Topics**:
A distinct area of learning within a session. Each topic has zero or more tensions. Topics are listed with a checkbox and current level. A topic can have branches (sub-topics) without having any tensions.
_Avoid_: concept (too vague), chapter (implies rigid structure)

**Tension**:
A contested point where researchers actively disagree and no consensus exists. Tensions are deep — they live underneath the surface branches and methods. OOP vs FP is a surface branch; the real tension might be "encapsulate state vs avoid state" — but that tension dissolves when you realize both solve the same underlying problem of state management. Go deep until the tension either resolves or stays contested.

The test for a real tension: would researchers publish papers arguing for each side? Is there an active debate with genuine intellectual stakes?

Tensions are linked back to sources in the literature directory.
_Avoid_: debate (too combative), disagreement (too interpersonal), fork (that's a branch), surface split (that's a branch)

**Branch**:
A split in the topic tree where the path divides into accepted sub-topics or methods. Unlike a tension, a branch is not contested — both sides are valid and researchers generally agree both exist. Supervised vs self-supervised learning is a surface branch. The real tension might be deeper: what makes one better than the other, in which contexts, and for which goals.

A topic can have many branches without having any real tensions.
_Avoid_: fork (confusing), split

**Path**:
A specific route through the curriculum tree — from root topic through branches to a leaf. The user traverses a path as they learn. A single topic might have multiple paths through it.
_Avoid_: route

**Curriculum**:
The collection of topics with their tensions, built at session start from the research summary. A living map that expands as the session deepens. Each topic in the curriculum links to its relevant source.
_Avoid_: syllabus (implies fixed order), outline (too hierarchical)

**Level**:
The tutor's assessment of the user's understanding of a topic. Assessed against tension handling, not just recall or self-report. Four levels:

| Level | Definition |
|-------|------------|
| **Unknown** | Has not encountered the topic |
| **Confused** | Has heard of it but understanding is fuzzy or copied |
| **Aware** | Can explain in own words and name the tension without choosing a side |
| **Confident** | Can navigate the tension, notice own bias, and respond to challenge |

**Remarks**:
Notes about the user's insights, confusions, and breakthroughs on specific topics during a session. Tagged to their topic. Not a transcript — selective capture.
_Avoid_: notes, transcript, log

**Session State**:
Whether the session is complete or partial. Incomplete sessions are flagged in the diary so they can be resumed.

## Relationships

- A **Session** (diary file) has one **Starting Point** and one **Subject**
- A **Session** contains multiple **Topics**
- Each **Topic** has zero or more **Tensions** and one or more **Branches**
- Each **Topic** links to a section in a **Research File**
- A **Research File** contains multiple sources; sources feed multiple tensions
- Sessions on related **Subjects** can be revisited; the curriculum builds across visits

## Modes

The tutor selects the appropriate mode based on the user's demonstrated confidence level. Three modes:

| Mode | When to use |
|------|-------------|
| **Socratic** | Default. Question prompts, guides to insight. Never answers directly. |
| **Curious Guide** | User is stuck or overloaded. More supportive, offers reframes. |
| **Devil's Advocate** | User is confident. Challenges positions, surfaces weaknesses. |

Mode transitions are explicit: "I'm shifting to [Mode]."

## Session Flow

1. **Session Start**: Build curriculum from research file, write topics + tensions to diary
2. **During Session**: Update topic levels and remarks at meaningful moments
3. **Wrap-up**: Complete remarks, update "Current State", mark session INCOMPLETE or COMPLETE
4. **Return**: Skill proactively suggests previous sessions on related subjects
