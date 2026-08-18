# Lab process log: Lesson alignment, Kick-off, and Debrief record

This file documents the process steps that the audit report itself doesn't cover — the setup, exchange rules, and the actual debrief conversation — so they're traceable for grading against `rubric.md`.

---

## Lesson alignment

Per `instructions.md`, this lab requires:
- A completed self-audit (`02_lab_self-audit.md`) done **before** the peer audit.
- Review of `01_eu-ai-act-fundamentals.md` (risk tiers and obligations).
- Review of the compliance/legal framing in `00_compliance-and-legal.md`.

**Note:** I'm not able to confirm from this conversation whether the self-audit lab was completed before this peer audit began — that's something only Kimia can confirm. If it was completed beforehand, add a line here confirming it (e.g., "Self-audit for [Kimia's project] completed on [date], prior to starting this peer audit"). If it wasn't, that's worth flagging honestly rather than asserting it happened, since the lab explicitly frames the peer audit as a test of whether an independent review reaches the same conclusions as a completed self-audit.

## Kick-off

**What was exchanged:** Only Nelly's Phase 1 system brief (the "Platform Risk Research Agent" system brief, ~350 words) was exchanged before the peer audit began. No self-audit findings, risk tier, gap analysis, or compliance memo were shared or seen in advance — the audit in `04_audit-report.md` was written from the brief alone, and Nelly's self-audit tier and findings were only received afterward (see `06_debrief-comparison.md`).

**Ground rules followed:**
- Work independently until the debrief — the peer audit (`01`–`04`) was completed and finalized *before* Nelly's self-audit was requested or received.
- Clarifying questions were asked in writing and logged — see `03_clarifying-questions-log.md`, with each question's rationale and a provisional assumption stated for the case where no answer came back in time.
- Ambiguity was noted rather than resolved by guessing — see the annotations marked **[?]** in `01_system-brief-annotated.md`, and the "Where I'm least confident" section in `02_classification.md`.

## Debrief conversation record

Per `instructions.md`, the debrief runs in five steps. Steps 1–2 aren't otherwise documented in the other files, so recorded here:

**1. Auditor presents:** The audit report (`04_audit-report.md`) was walked through with Nelly — risk tier, role map, all four findings, and the overall "proceed with conditions" recommendation.

**2. Builder responds:** Nelly explained context the brief hadn't captured, most notably: the specific sub-processors in use (OpenAI, DeepSeek/Vercel AI Gateway, Tavily, Pinecone) and the fact that DPAs weren't yet signed with them; and the source of the compliance-posture scoring — her own book, *The Interface Is Not the System: Why Control, Trust, and Responsibility Break at Scale in AI Systems*, plus four ControlGap failure modes.

**3–5. Compare classifications, compare gap lists, joint closing note:** Documented in full in `06_debrief-comparison.md`.

## Reinforce (optional stretch reflection)

The lab's Reinforce prompts, briefly addressed:

- *Reviewing the clarifying questions asked of you about your own system:* Not applicable to this submission — no self-audit or peer audit of Kimia's own project is included here; this file covers only the audit of Nelly's project.
- *A finding you initially disagreed with, and whether you still disagree after the debrief:* The clearest candidate is Finding 4 (reputational/legal exposure toward scored vendors) versus Nelly's Finding 3 (the DPA gap) — these came from different vantage points rather than a disagreement, and the debrief didn't surface an actual dispute so much as two findings that only became visible from where each person was standing. That asymmetry is what the joint closing note in `06_debrief-comparison.md` is built around.
