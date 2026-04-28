---
description: Create a git commit with staged changes
agent: build
subtask: true
---

Analyze the changes since the last commit and create a comprehensive new commit. Follow the repository's commit message style by checking recent commits.

*Important*: Do NOT push to remote repository.

Steps:

1. Gather all git information in one command: git status; echo "=== RECENT COMMITS ==="; git log --oneline -10; echo "=== STAGED CHANGES ==="; git diff --staged
2. If there are staged files in the status output, consider only those files and jump directly to step 4
3. If there are NO staged files but there are unstaged changes, stage everything using "git add ."
4. Analyze the staged changes and create a commit message:
    - First line: concise summary (under 50 chars)
    - If the summary is self-explanatory use single-line commit
    - For complex changes, add empty line and brief objective description with bullet points starting with "-"
5. Create the commit with the appropriate message format (single-line for simple changes, multi-line for complex changes)
6. Confirm that the commit was successful and display its hash and message, following the example format below:

✅ Successful!
Hash: 4f73c78b
Full message: Replace sl-input with bkper-amount in account balance adjuster

- Remove manual input sanitization logic
- Leverage built-in amount parsing and formatting
- Simplify amount change handling

7. Only return the final output as shown above, without any additional explanations or comments. And do NOT use the term "commit" at all.