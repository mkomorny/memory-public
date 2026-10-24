# Memory & State Management

> **Tri-Platform Agent Skill** for Claude Desktop / Code, Grok CLI, and Google Antigravity / Gemini.  
> Persistent Bot Memory and Task Ledger Synchronization — Standardizes persistent bot memory, session synchronization, and decision logging via the structured Task Ledger, Hypothesis Ledger, and rolling window pruning.

---

## Overview

`memory` provides standardized capabilities across conversational AI platforms:
- Structured Task Ledger and Hypothesis Ledger format (lessons-learned.md).
- Rolling window pruning (keep latest 50 tasks, 20 decisions).
- Append-only decision logging ritual.
- Worker subagent read-only memory enforcement.
- Tri-platform NTFS junctions connecting Claude, Grok, and Antigravity.
- Standard documentation suite: SKILL.md, HOW_TO_USE.txt, IMPLEMENTATION_PLAN.md, and README.md.

---

## Tri-Platform Architecture

Zero duplicate code across platforms. Canonical source resides in `.agents`:
- **Canonical Source**: `C:\Users\<you>\.agents\skills\memory`
- **Claude**: `C:\Users\<you>\.claude\skills\memory` (NTFS Junction)
- **Grok**: `C:\Users\<you>\.grok\skills\memory` (NTFS Junction)
- **Antigravity**: `C:\Users\<you>\.gemini\config\skills\memory` (NTFS Junction)

---

## Documentation Suite

- [`HOW_TO_USE.txt`](HOW_TO_USE.txt): Standardized user guide and prompt templates.
- [`IMPLEMENTATION_PLAN.md`](IMPLEMENTATION_PLAN.md): Feature checklist and roadmap.
- [`App Changes Tracker.html`](App%20Changes%20Tracker.html): Interactive visual version log.
- [`SKILL.md`](SKILL.md): Agent system instructions and triggers.
