# Integrate document into teach-me

The document skill was planned as a separate skill triggered by `# Document`. This is merged into the teach-me skill, which now handles curriculum building, Socratic tutoring, and diary management in one flow.

Reason: Simplicity and continuity. A single entry point for learning sessions. The diary is a working document from session start, not a post-session artifact.

Trade-off: Reduced modularity. Research remains separate (literature review is its own workflow), but documentation is absorbed. The three-skill PRD architecture is replaced by a two-skill architecture.

Reverting this would mean splitting teach-me back into teach-me and document — possible, but requires rewriting the diary management logic.