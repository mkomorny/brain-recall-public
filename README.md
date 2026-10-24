# Brain Recall

> **Tri-Platform Agent Skill** for Claude Desktop / Code, Grok CLI, and Google Antigravity / Gemini.  
> Semantic Search and Associative Retrieval with Hops — Instantly searches personal Second Brain for memories, decisions, preferences, and past context using semantic embeddings, tag filters, and graph hops.

---

## Overview

`brain-recall` provides standardized capabilities across conversational AI platforms:
- Semantic vector search with user intent framing.
- Multi-hop graph expansion (--hops 0-2).
- Tag filtering (--tag <tag>) and memory kind filtering (--kind semantic|episodic).
- Top-K result limiting with relevance scoring.
- Tri-platform NTFS junctions connecting Claude, Grok, and Antigravity.
- Standard documentation suite: SKILL.md, HOW_TO_USE.txt, IMPLEMENTATION_PLAN.md, and README.md.

---

## Tri-Platform Architecture

Zero duplicate code across platforms. Canonical source resides in `.agents`:
- **Canonical Source**: `C:\Users\<you>\.agents\skills\brain-recall`
- **Claude**: `C:\Users\<you>\.claude\skills\brain-recall` (NTFS Junction)
- **Grok**: `C:\Users\<you>\.grok\skills\brain-recall` (NTFS Junction)
- **Antigravity**: `C:\Users\<you>\.gemini\config\skills\brain-recall` (NTFS Junction)

---

## Documentation Suite

- [`HOW_TO_USE.txt`](HOW_TO_USE.txt): Standardized user guide and prompt templates.
- [`IMPLEMENTATION_PLAN.md`](IMPLEMENTATION_PLAN.md): Feature checklist and roadmap.
- [`App Changes Tracker.html`](App%20Changes%20Tracker.html): Interactive visual version log.
- [`SKILL.md`](SKILL.md): Agent system instructions and triggers.
