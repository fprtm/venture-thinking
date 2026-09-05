# Domain grounding via Atlas Domain Knowledge

Vague FRAME answers are usually a vocabulary problem, not a thinking problem — "clinic owners" and "manual workflow" are placeholders, not a domain. Before accepting a FRAME or naming an assumption, ground the idea in **Atlas Domain Knowledge** — [github.com/fprtm/atlas-domain-knowledge](https://github.com/fprtm/atlas-domain-knowledge) (raw file: [`atlas-domain-knowledge.md`](https://raw.githubusercontent.com/fprtm/atlas-domain-knowledge/main/atlas-domain-knowledge.md)) — instead of inventing roles, processes, or systems from general knowledge. Fetch it with a web-fetch tool when available. This is optional grounding, not a hard dependency — if it can't be fetched, run the loop as normal.

**Scope: vocabulary only, never a substitute for real-world validation.** Atlas is a static ontology — it tells you the real role names, process steps, and system types a domain uses, nothing about whether *this specific* pain is felt today, how competitors currently price it, or whether this customer will pay. Use it only when the loop needs domain/business vocabulary it doesn't already have. It never answers a TEST-stage question and it must never be cited as evidence of market reality — that always requires the mandatory internet research in [`research.md`](research.md).

## What to pull from it, and when

**During FRAME** — locate the idea's industry in Atlas §8 (Major Industry Map, 45 industries A–AS, e.g. `B. Healthcare & Life Sciences`, `AK. Laundry & Cleaning Services`, `AN. Wedding & Event Organizer`). Each industry entry lists real subindustries, roles, processes, systems, data, and AI opportunities. Use these to sharpen "who exactly" and "what problem" instead of a generic guess — a clinic-queue idea should name the actual role (front-desk admin vs. triage nurse) and the actual process step from §8's Healthcare entry, not an assumed one.

**During ASSUME** — cross-check candidate assumptions against Atlas §55 Master Meta-Model (`DOMAIN → INDUSTRY → ORGANIZATION → ROLE → TASK → PROCESS → SYSTEM/DATA/DECISION → OUTCOME → KPI → BUSINESS VALUE`). An assumption that skips a layer (e.g. jumps from "role" straight to "business value" without naming the process or decision in between) is usually the unexamined one — that gap is often the riskiest assumption, not a minor detail.

**When the FRAME still feels thin after one pass** — run Atlas §56 The 12 Questions (domain, who's involved, their job, their goal, the process, the decisions made, the rules that apply, the data needed, the systems used, the output, how success is measured, how tech could improve it). Answering these against the real industry entry usually surfaces the pain point and the willingness-to-pay driver directly.

**Anti-patterns to avoid** — Atlas §54 lists common domain-modeling mistakes (treating a role as a system, confusing a process with a decision, inventing data entities no real system holds). Skim it before finalizing FRAME/ASSUME wording so the hypothesis doesn't rest on a fabricated system or dataset.

## How to use this without breaking the loop

This is grounding, not homework for the person — do the Atlas lookup yourself, in the same turn, the same way desk research and social listening happen in TEST. Don't quote large verbatim blocks of Atlas back at the person; extract the two or three facts (the real role name, the real process step, the real system) that sharpen the FRAME, and cite the section (e.g. "per Atlas §8 Healthcare") so it's traceable.
