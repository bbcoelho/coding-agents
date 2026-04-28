---
description: Suggest AGENTS.md updates based on session learnings
agent: plan
---

Review the conversation history since the last time this command (`/updt_agtmd`) was run. If it has not been run before, review the full session.

Identify knowledge that should be added to AGENTS.md — specifically knowledge that an agent could NOT discover by reading the codebase alone or fetching from the web. Focus on:

1. **Key decisions made** — architectural, design, or workflow decisions and the reasoning behind them
2. **Failed attempts** — approaches that were tried and rejected, and why they failed (so future agents don't repeat them)
3. **User-provided context** — preferences, constraints, domain knowledge, or corrections introduced by the user
4. **New conventions agreed upon** — patterns, naming, structure, or process decisions established during the session

Then read the current AGENTS.md to understand what is already documented and what needs to be changed or adapted. Do not suggest anything already covered.

For each finding, output a **ready-to-paste markdown block** followed by a one-line note indicating where in AGENTS.md it belongs.

Do NOT modify any files.
