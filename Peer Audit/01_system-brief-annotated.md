# Phase 1 — Read and annotate: Platform Risk Research Agent (Nelly's project)

Annotation key: **[TIER]** = affects risk tier classification · **[?]** = unclear, needs clarifying question · **[OBL]** = suggests a specific obligation applies

---

## What the system does

The system checks if an AI vendor is safe to use. A user gives it a vendor name and a use case. The system searches the web, checks compliance signals, and scores the vendor on six risk areas. **[?: "compliance signals" against what standard — see clarifying questions]** It gives a final verdict: recommended, or not recommended. **[TIER: a binary verdict with real consequences for a third party (the vendor), generated with no human check — relevant to both the tier discussion and to non-AI-Act liability exposure]** If not recommended, it suggests other vendors instead.

## Inputs

The user gives three things:
- The vendor name
- What they plan to use the vendor for
- Basic context about their own company

Some of this input may include company data. It does not include personal data about individual people. **[TIER: this is a meaningful point in favor of a lower tier — no natural person is being profiled by the inputs]**

## Outputs

The system gives one report. The report has:
- A trust score
- Six risk scores (data handling, vendor stability, incident history, community signal, compliance posture, integration risk)
- A confidence tag for each finding (strong evidence, limited evidence, inferred, or no signal found) **[OBL: good practice for uncertainty communication — relevant to Finding 3]**
- A final verdict
- If the verdict is negative, two or three alternative vendors with a comparison table **[?: steering the buyer toward named competitors is a meaningful action with commercial consequences for the rejected vendor]**

## Who is affected

The buyer company gets the report and acts on it. The vendor being checked is affected too, since the report can recommend against them. **[TIER: the "affected" party here is a company/vendor, not a natural person — this is the key reason I don't think Annex III's people-focused high-risk categories apply, but it's still worth flagging as a real-world stakes issue in Section 4]**

## Human review

No human reviews the report before the user sees it. This is on purpose. The system is self-serve. Nobody checks the output first. **[TIER/OBL: strongest single fact in this brief. Fully autonomous, no human-in-the-loop at all — opposite design choice from a system like RegGuard-Mini. Even though this doesn't push the system into a high-risk AI Act tier by itself, it is the central fact for Section 4 findings]** This makes the confidence tags important. If the system is not sure about something, it has to say so in the report itself. **[TIER: mitigates but doesn't eliminate the no-human-review risk — see Finding 3 on how "no signal found" actually gets handled in the final verdict]**

## Who built it

Built alone, using an existing LangGraph agent repo as a starting point, with research, scoring, and reporting logic built on top. **[?: brief doesn't name a specific commercial LLM provider the way a comparable project might — worth clarifying for the role map, since it affects who the "third-party vendor" role actually is]**

## Who uses it in production

A company deciding whether to adopt an AI vendor or no-code platform — either a small team doing its own vendor check, or a consultant running it before advising a client. The current build targets the first case: the buyer runs it directly. **[?: no company/employer is named as the intended commercial provider (unlike a scenario where a named company builds and sells it) — worth asking whether there's a planned production owner]**
