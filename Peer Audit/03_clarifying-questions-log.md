# Phase 3 — Clarifying questions log: Platform Risk Research Agent

Information requested from client (Nelly) on 2026-08-18. Per lab ground rules, these were logged before any self-audit findings were exchanged.

---

### Question 1 — Basis for the "compliance posture" score
**What I need to know:** What specific regulations, standards, or frameworks does the compliance-posture risk score actually check against (e.g., GDPR, SOC 2, ISO 27001, sector-specific rules), and how is that different from the general web-search-based risk scoring the system also does?
**Why it matters:** "Checks compliance signals" is undefined in the brief. Without knowing the reference standard, it's hard to assess whether a "not recommended" compliance-posture score is well-founded or just an inference from limited web signal — which matters a lot given there's no human review before the buyer sees it.
**Provisional assumption:** I'm assuming this is currently based on publicly available signals found via web search (e.g., a vendor's published certifications or policy pages) rather than a formal audit against a named standard, since no named framework appears in the brief.

### Question 2 — Whether the verdict functions as a real sign-off
**What I need to know:** In practice, does a buyer treat a "not recommended" verdict as final — i.e., do they stop evaluating that vendor — or do they independently verify before acting on it?
**Why it matters:** The brief says the system is self-serve with no human review by design. If buyers, in practice, treat the verdict as decisive rather than as one input among several, that's the real-world stakes of Finding 1 in the audit report, regardless of the AI Act tier.
**Provisional assumption:** I'm assuming buyers currently do treat "not recommended" as effectively decisive, since the system is explicitly designed to be self-serve and fast, which is the whole point of not having a review step.

### Question 3 — Data retention and storage
**What I need to know:** How long are submitted company details and generated vendor reports retained, where are they stored, and who (if anyone) can access past reports — including reports about a given vendor generated for other buyers?
**Why it matters:** The brief confirms the inputs may include company data, even though not personal data about individuals. Retention and access matter for confidentiality between buyer companies, and for whether a vendor could ever see what's been said about them.
**Provisional assumption:** I'm assuming no formal retention policy exists yet, given this is a course-stage project.

### Question 4 — Disclosure of the AI-generated, unreviewed nature of the report
**What I need to know:** Does the report itself state clearly that it was generated automatically with no human review, and that confidence tags should be read as an indicator of evidence strength rather than certainty?
**Why it matters:** Even though I don't think this is legally required by Article 50 given the non-conversational, non-public nature of the tool, it seems like important good practice given how consequential the verdict is and how it directly names competing vendors.
**Provisional assumption:** I'm assuming this isn't yet explicitly stated in the report itself, since the brief describes the confidence tags but not a disclosure statement.
