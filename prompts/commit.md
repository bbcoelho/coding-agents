---
description: Create a git commit with staged changes
agent: build
subtask: true
---

- Consider only this session changes
- Follow the repository's commit message style by checking recent commits.

*Important*: Do NOT push to remote repository.

Analyze the changes and create a commit message:
    - First line: concise summary (under 50 chars) using Conventional Commits pattern.
    - If the summary is self-explanatory use single-line commit
    - For complex changes, add empty line and brief objective description with bullet points starting with "-"
