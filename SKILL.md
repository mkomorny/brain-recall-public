---
name: brain-recall
description: >-
  Instantly searches your personal Second Brain for memories, decisions, preferences,
  and past context. Executes immediately with no approval needed. Supports flags:
  --hops <0-2> (graph expansion), --tag <tag>, --kind <semantic|episodic>, --topK <N>.
---

# Brain Recall — Semantic Search (`/brain-recall`)

Execute **immediately** by calling the `second-brain` MCP `recall` tool. No approval needed.

## Syntax

```
/brain-recall <query> [--hops <0-2>] [--tag <tag>] [--kind <semantic|episodic>] [--topK <N>]
```

## How to call the tool

- **Intent-frame the query**: Expand to `"User wants to [action] regarding [topic] — what should I know?"`
- **`--hops`** (default 0): Set 1–2 when user asks "why", "how did this evolve", or wants linked context
- **`--topK`** (default 5): Increase to 10–20 for broad searches

## After results

- Show results as a clean list: ID, title, date, summary per entry
- If any result shows `[truncated ...]`, alert and suggest `/brain-get <id>`
- If no results, suggest rephrasing or broader query

## Examples

```
/brain-recall Live Actions architecture
/brain-recall Ableton buffer dropouts --hops 1
/brain-recall studio preferences --kind semantic --topK 10
/brain-recall open tasks --tag task
```
