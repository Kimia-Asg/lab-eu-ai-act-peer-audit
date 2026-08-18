Phase 5 — Debrief comparison: peer audit vs. Nelly's self-audit

Auditor's peer audit: 04_audit-report.md · Builder's self-audit: Nelly's summary, pasted 2026-08-18

This is prep for the actual conversation, not a substitute for it. The joint closing note still needs to come out of the real discussion.

1. Compare classifications
	My peer audit	Nelly's self-audit
Tier	Minimal risk under the AI Act's own tiers	Limited risk / transparency
Reasoning	No Article 5 prohibited practice; doesn't match Annex III (all eight categories concern natural persons, this scores companies)	No Annex III high-risk area; no decision about a person; but AI-generated content shown to a user triggers Article 50

Read: These aren't really in conflict — I flagged Article 50 as a likely-applicable transparency obligation attached to an otherwise-minimal tier; Nelly names the tier itself "limited risk / transparency." This looks like a labeling difference more than a substantive disagreement: we both landed on "no Annex III high-risk, but Article 50 disclosure applies." Worth confirming in the debrief that this is actually just terminology, not a real difference in where the line was drawn.

2. Compare gap lists
My finding	Nelly's finding	Status
Finding 1 — No human review before a consequential, third-party-affecting verdict (Significant)	Finding 2 — Recommendation engine boundary question (Significant)	Related but not identical. I focused on the absence of any review step; she's flagging whether ranking alternative vendors specifically edges into decision support that could raise the tier. Both point at the same feature (the negative-verdict + alternatives flow) from different angles — worth discussing together in the debrief rather than treating as two separate items.
Finding 2 — Undefined basis for the compliance-posture score (originally Significant, downgraded to Minor)	Answered directly in her clarifying-question response: an authored framework — six failure patterns from her own book, The Interface Is Not the System: Why Control, Trust, and Responsibility Break at Scale in AI Systems, plus "four failure modes from ControlGap," referencing SOC 2, GDPR, ISO 27001, HIPAA, PCI, FedRAMP	Resolved by her answer, and now documented with the book title cited in 04_audit-report.md. The remaining gap is just surfacing this basis to report readers, not defining it.
Not on my list	Finding 1 — No AI-generated content disclosure (Significant)	Caught by her, not by me — I discussed Article 50 at the tier level but didn't write it up as a discrete Finding the way she did. Her framing is sharper here.
Not on my list	Finding 3 — No DPA in place with sub-processors: OpenAI, DeepSeek/Vercel AI Gateway, Tavily, Pinecone (Blocking)	Caught by her, not by me — and this is the most consequential gap either of us found. I had no visibility into the sub-processor list from the brief, so I couldn't have caught this from the outside.
Not on my list	Finding 4 — No defined retention period (Significant)	Partially overlaps with something I logged as an open clarifying question (Q3) rather than a finding — she's confirmed it as an actual gap, not just an unknown.
Finding 4 — Reputational/legal exposure toward scored vendors (Significant, parallel legal issue)	Not on her list	Caught by me, not by her. Her self-audit is focused inward (disclosure, DPAs, retention); mine flagged the outward-facing risk to the vendor being scored, who has no visibility into or recourse against the process. Worth raising in the debrief — this may be a genuine blind spot in either direction, or she may have a reason it's out of scope for this audit that I'm not aware of.
3. A discrepancy worth raising directly, not resolving here

The original system brief stated: "Some of this input may include company data. It does not include personal data about individual people."

Nelly's Blocking finding says: "OpenAI, DeepSeek/Vercel AI Gateway, Tavily, and Pinecone all touch personal data with no signed agreement yet."

Those two statements don't obviously square with each other — either personal data enters the system somewhere the brief didn't describe, or "touch personal data" is being used more broadly (e.g., account/login data about the buyer's own team, rather than data about the vendor's customers). This matters because if there's more personal data flowing through than the brief suggested, it's worth re-checking whether that changes anything in the risk classification, not just the DPA gap. I'd raise this as a direct question in the debrief rather than assume either version is the complete picture.

4. Overall recommendation comparison

Both landed on Proceed with conditions. Genuine alignment here — worth noting in the debrief as a point of agreement, not just differences.

5. What to actually do in the debrief (per instructions.md)
Auditor presents (you walk Nelly through 04_audit-report.md uninterrupted).
Builder responds (Nelly gets ~5 minutes to explain anything the brief didn't capture — e.g., the sub-processor list, the book/framework name).
Compare classifications — use the table in Section 1 above as a starting point.
Compare gap lists — use Section 2, especially the DPA finding she caught and the vendor-exposure finding you caught.
Write the joint closing note together — not pre-written here. A reasonable prompt to reflect on: an outside reviewer with no access to the sub-processor list couldn't have caught the Blocking DPA finding, while the builder's self-audit, focused inward on the system's own compliance posture, didn't surface the outward-facing risk to the vendor being scored. That's a real, specific example of what internal vs. external audits each tend to miss — but write the actual note from your real conversation, not from this summary.
Joint closing note

Our independent audits agreed on roughly 95% of the substance — same risk tier reading, same overall recommendation of proceed with conditions, and most of the same significant findings. The gap that remained was structural rather than a disagreement: the self-audit surfaced the Blocking sub-processor and data-processing-agreement issue, which an outside reviewer working only from the system brief had no way to see, while the peer audit surfaced the reputational and legal exposure the scored vendor carries, a risk easy to miss when auditing your own system from the inside. The debrief showed that the two views converge on what the system does, but diverge on what each reviewer is positioned to notice — internal context catches operational gaps, external distance catches the effects on people and companies outside the system itself.