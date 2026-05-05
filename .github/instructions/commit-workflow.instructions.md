---
applyTo: "**"
description: "When user asks to commit, use the commit-workflow skill and confirm required points with ask tool before committing."
---

# Commit Request Workflow

When the user asks to create a commit:

1. Load and follow `.github/skills/commit-workflow/SKILL.md`.
2. Use ask tool to confirm required points before committing.
3. Respect conventional commit format and 50-char header max.
4. Do not commit without explicit user confirmation.
