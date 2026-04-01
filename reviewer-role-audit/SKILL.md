---
name: reviewer-role-audit
description: Audit any interface — existing or in design — through the lens of the reviewing role. Use when someone wants to evaluate whether their AI-assisted interface supports a human reviewer coming in to assess, approve, and act on agent-produced output. Invoke with /reviewer-role-audit.
---

# Reviewer Role Audit

Audit question: **If an agent did all the work and a human is reviewing — can they orient, assess, and decide in 5 seconds?**

Work through the five audit areas. Be specific. Flag what works, what doesn't, what to fix.

---

## Step 1 — Understand the context

Ask if not provided:

1. What does the agent produce? (draft, summary, briefing, recommendation?)
2. What does the reviewer need to decide? (Approve / edit / redirect / send?)
3. What's the time pressure?
4. Who is the reviewer? (Role, expertise level)
5. Did the reviewer encounter the underlying information before seeing the artifact, or does it arrive cold?
   *(Cold = interface must surface evidence harder. Prior context = anchoring to the AI's framing is the bigger risk.)*

---

## Step 2 — Five audit areas

### 2.1 — Artifact prominence
Is the artifact front and center, or buried next to the chat?

- **Good:** Artifact is dominant. Chat is secondary infrastructure.
- **Bad:** Chat panel dominates. Artifact is a side panel or afterthought.
- **Fix:** Flip the hierarchy. The artifact is the product; the conversation is the tool that made it.

---

### 2.2 — Five-second test
Can a reviewer orient, assess, and decide in 5 seconds — and does the artifact visually signal where scrutiny is needed?

- **Good:** Clear structure, headers, key claim visible immediately. Uncertain or low-confidence sections are visually flagged — not just mentioned — so the reviewer's eye is drawn to what needs scrutiny.
- **Bad:** Prose blocks, buried key points. Or: uniformly polished output where a hallucinated statistic and a verified fact look identical. Uniform polish suppresses critical review regardless of layout.
- **Fix:** Bullets over sentences. Key claim at top. Mark uncertain claims at the claim level — not a single aggregate confidence score. Size of uncertainty markers matters more than color.

---

### 2.3 — Iterability
Are Approve, Edit, and Reject structurally equal — or is approval the path of least resistance?

- **Good:** Three-state model (Approve / Request Changes / Comment). All equally accessible — same visual weight, same number of steps. Unresolved concerns can block the output from proceeding.
- **Bad:** One prominent approve button; edit or feedback requires extra steps. The interface treats approval as the expected outcome.
- **Fix:** Equal visual weight. Equal steps. Consider whether unresolved concerns should block — not just note — the output.

---

### 2.4 — Evidence quality
Does the artifact show *where* information comes from, or does it explain *why* it's correct?

This distinction matters: explanations increase acceptance of both correct *and* incorrect AI outputs. Sources (verifiable evidence) reduce overreliance on incorrect outputs. An artifact that explains its reasoning is less safe to review than one that links to its evidence.

- **Good:** Claims link to specific sources, data points, or passages. The reviewer can verify independently. Inline citations at the claim level. Provenance is traceable, not just summarised.
- **Bad:** The artifact explains its own reasoning ("Based on the client's situation, I recommend X because..."). Confident narrative throughout, no source links. Every section reads as a conclusion rather than a claim to check.
- **Warning sign:** If the artifact reads as a polished argument for its own conclusions, the reviewer is being asked to trust, not verify.
- **Fix:** Replace rationale paragraphs with evidence linkage. Inline citations at the claim level. The reviewer checks the source — not the AI's interpretation of it.

---

### 2.5 — Approve-to-send flow
Is the path to "send" clear and direct — and does the approval moment feel consequential?

- **Good:** One clear action from reviewed → approved → sent. The approve action surfaces a brief summary of what is being endorsed — so approval is deliberate, not casual.
- **Bad:** Multi-step or requires leaving the artifact view. Or the opposite: a single frictionless click with no confirmation — possible to approve without demonstrating anything was reviewed.
- **Fix:** Collapse the flow to minimal steps. But introduce a deliberate moment at approval: a summary, checklist, or confirmation that names what is being sent. Not friction for its own sake — making approval feel like a decision, not a default.

---

## Step 3 — Output format

**What's working:** (1–3 things the interface gets right for the reviewing role)

**Critical gaps:** (The 1–2 things that most undermine the reviewing role — fix these first)

**Quick wins:** (Small changes that would meaningfully improve reviewer experience)

**One question to keep asking:** (A design principle tailored to this interface that the team should use as a recurring test)

---

## Underlying principle

> "Design the artifact, not the interface."

The agent's output is what the human actually uses. The interface is infrastructure. Start with what a great artifact looks like. Then build the interface to support it.

Sources reduce overreliance on wrong answers. Explanations increase it. Prioritise evidence linkage over AI-generated rationale.
