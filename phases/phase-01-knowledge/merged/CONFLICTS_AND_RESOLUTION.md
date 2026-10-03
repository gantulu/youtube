# Phase 1 — Conflicts and Resolution

## Resolved conflicts

### 1 FPS
**Risk:** treating 1 FPS as sufficient for every Short.
**Resolution:** 1 FPS is the documented static default; rapid motion/quick cuts require additional verification or a suitable processing mode.

### Agentic processing
**Risk:** treating agentic processing as universal.
**Resolution:** model-dependent capability; the workflow must check current model support.

### Continuity
**Risk:** describing character/object identity locks as native model guarantees.
**Resolution:** identity and continuity locks are project-level controls enforced by the Skill/workflow/validator.

### NotebookLM YouTube input
**Risk:** treating a NotebookLM YouTube source as equivalent to direct video understanding.
**Resolution:** official documentation describes transcript-text import for supported public YouTube sources; frame-level visual analysis remains a separate Gemini Video Understanding task.

### Model identifiers
**Risk:** copying a current model ID into permanent rules.
**Resolution:** model IDs live in versioned model-reference material and must be revalidated before production use.

### Vids prompt syntax
**Status:** not promoted to hard canonical syntax until current official Vids help/UI behavior is explicitly verified.
