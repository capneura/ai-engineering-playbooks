# Evidence Map

## Purpose

This file maps real engineering experience to the general principles used in the manuscript.

The manuscript must not name the source project.

The purpose is not to document the original project.

The purpose is to extract durable engineering principles from it.

## Evidence Rule

Every principle used in the manuscript must answer four questions:

1. What happened?
2. What did we learn?
3. What engineering rule emerged?
4. How can another builder apply it?

## Evidence Authority

Evidence should be handled in this order:

1. Repository artifacts
2. Runtime outputs and diagnostics
3. Written contracts and phase documents
4. Collaboration summaries
5. Conversation-derived patterns
6. Memory and interpretation

Memory may suggest a hypothesis.

Repository evidence and documented collaboration patterns decide whether it belongs in the manuscript.

## Category 1 - Project Drift

### What Happened

Long-running AI-assisted work repeatedly risked drifting away from its original purpose.

Each local decision often looked reasonable in isolation.

The larger system became harder to reason about when the original mission, architectural decisions, and authority boundaries were not continuously preserved.

### What We Learned

AI can help move quickly, but speed without continuity creates confusion.

The problem is rarely one bad answer.

The problem is accumulated local decisions without a stable control structure.

### Engineering Rule

AI does not remove the need for architectural continuity.

It increases the need for it.

### Application

A builder should maintain stable project summaries, frozen objectives, milestone records, and decision logs.

If the project cannot be restarted from its own documentation, the project is under-documented.

### Manuscript Relevance

- Chapter 1 - The Illusion
- Chapter 5 - Preventing AI Drift
- Chapter 6 - Long-Term Project Survival

---

## Category 2 - Mixed Operating Modes

### What Happened

Exploration, planning, and implementation were sometimes mixed into one motion.

This caused confusion.

A diagnostic conversation would become a patch.

A planning discussion would become a redesign.

A verification step would accidentally become a new theory.

### What We Learned

Different kinds of work require different permissions.

Exploration should discover.

Planning should decide.

Implementation should change.

Verification should test.

When these modes are mixed, the work becomes hard to audit.

### Engineering Rule

Do not explore, plan, implement, and verify at the same time.

### Application

Before starting a work session, declare the operating mode:

- Explore
- Plan
- Implement
- Verify

Do not allow the AI assistant to leave the mode without explicit permission.

### Manuscript Relevance

- Chapter 2 - The Three Operating Modes
- Chapter 3 - Build Contracts, Not Chaos
- Chapter 7 - Putting Everything Together

---

## Category 3 - Contracts as Control Surfaces

### What Happened

Progress improved when vague intentions were converted into explicit contracts.

The most useful contracts defined:

- Objective
- Scope
- Constraints
- Success criteria
- Forbidden changes
- Verification requirements
- Next allowed action

### What We Learned

A contract gives the AI assistant boundaries.

It also gives the human operator a way to catch drift.

The contract is not bureaucracy.

It is a control surface.

### Engineering Rule

A contract turns intention into engineering control.

### Application

Before implementation, create a short written contract.

The contract should say what is allowed, what is forbidden, and what counts as success.

Do not begin implementation until the contract is stable.

### Manuscript Relevance

- Chapter 3 - Build Contracts, Not Chaos
- Chapter 5 - Preventing AI Drift
- Chapter 6 - Long-Term Project Survival

---

## Category 4 - Evidence Over Opinion

### What Happened

At several points, theories about system behavior became less useful than direct evidence.

The work improved when opinions were replaced by diagnostics, telemetry, runtime reports, file inspection, and reproducible verification.

### What We Learned

AI can produce confident explanations before the evidence is complete.

Human operators can do the same.

Confidence is not verification.

### Engineering Rule

Opinion is useful for forming hypotheses.

Evidence is required for decisions.

### Application

When a system behaves unexpectedly, do not redesign immediately.

First collect evidence.

Then identify the source of truth.

Then decide.

### Manuscript Relevance

- Chapter 4 - Evidence Beats Opinion
- Chapter 7 - Putting Everything Together

---

## Category 5 - Canonical Sources of Truth

### What Happened

Multiple artifacts appeared to describe the same reality.

Some reflected intention.

Some reflected configuration.

Some reflected historical behavior.

Some reflected runtime behavior.

Some reflected broker-level or external reality.

Progress required deciding which source had authority for each kind of truth.

### What We Learned

A system can contain many truths.

Not all truths have the same authority.

Without explicit authority, the loudest artifact wins.

That is dangerous.

### Engineering Rule

Every engineering system needs an explicit source of truth for each decision category.

### Application

Define which artifact owns:

- Configuration truth
- Runtime truth
- Historical truth
- External truth
- Decision truth
- Verification truth

Do not allow one source to answer every question.

### Manuscript Relevance

- Chapter 4 - Evidence Beats Opinion
- Chapter 7 - Putting Everything Together

---

## Category 6 - Authority Debugging

### What Happened

Visible symptoms were often misleading.

The real issue was frequently hidden in the layer that owned the decision.

A system could appear broken at the surface while the real cause was an upstream gate, downstream filter, stale authority rule, or mismatched interpretation.

### What We Learned

Debugging symptoms wastes time when the decision path is unclear.

The first task is not to fix the symptom.

The first task is to identify who had authority to create the symptom.

### Engineering Rule

Do not debug symptoms before identifying which layer owns the decision.

### Application

When a system fails, trace the decision path:

1. Who produced the signal?
2. Who transformed it?
3. Who admitted it?
4. Who rejected it?
5. Who executed it?
6. Who verified it?

Repair the owning layer, not the visible surface.

### Manuscript Relevance

- Chapter 4 - Evidence Beats Opinion
- Chapter 7 - Putting Everything Together

---

## Category 7 - Summaries as Continuity Infrastructure

### What Happened

Long-running work required durable summaries.

Without summaries, previous decisions were repeatedly rediscovered, misunderstood, or overwritten.

Summaries became necessary for continuity across sessions.

### What We Learned

A summary is not administrative decoration.

It is part of the engineering system.

It preserves decisions, scope, evidence, unresolved questions, and next actions.

### Engineering Rule

A summary is continuity infrastructure.

### Application

End every major phase with a summary containing:

- What changed
- What was proven
- What remains uncertain
- What must not be repeated
- What the next action is

### Manuscript Relevance

- Chapter 5 - Preventing AI Drift
- Chapter 6 - Long-Term Project Survival

---

## Category 8 - Incremental Repair

### What Happened

Large redesigns were tempting during failure periods.

They often increased uncertainty.

Progress improved when repair happened in small stages, with verification after each stage.

### What We Learned

When too many things change at once, success cannot be attributed and failure cannot be isolated.

Small repairs create observable cause and effect.

### Engineering Rule

Repair one authority boundary at a time.

### Application

Change one meaningful thing.

Verify it.

Record the result.

Only then continue.

### Manuscript Relevance

- Chapter 3 - Build Contracts, Not Chaos
- Chapter 6 - Long-Term Project Survival
- Chapter 7 - Putting Everything Together

---

## Category 9 - Verification Before Redesign

### What Happened

Confusion often created pressure to redesign.

But redesign without verification risked replacing an unknown problem with a larger unknown system.

The work improved when verification came first.

### What We Learned

A system should not be redesigned until the failure mode is known.

Otherwise, redesign becomes emotional relief disguised as engineering.

### Engineering Rule

Redesign is not the first response to confusion.

Verification is.

### Application

Before redesigning, answer:

- What exactly failed?
- Where did it fail?
- Which evidence proves it?
- Which layer owns the failure?
- What is the smallest repair?

### Manuscript Relevance

- Chapter 1 - The Illusion
- Chapter 4 - Evidence Beats Opinion
- Chapter 7 - Putting Everything Together

---

## Category 10 - Collaboration With AI

### What Happened

AI was most useful when treated as a constrained engineering collaborator.

It became less reliable when allowed to improvise across unclear goals, unstable context, or vague authority.

### What We Learned

AI collaboration requires operating discipline.

The assistant needs clear mode, context, evidence, boundaries, and verification.

Without that, it may produce plausible work that moves in the wrong direction.

### Engineering Rule

AI collaboration requires control, not blind trust.

### Application

Use AI with:

- Stable objectives
- Explicit operating modes
- Written contracts
- Evidence requirements
- Verification steps
- Session summaries
- Human authority over scope

### Manuscript Relevance

- Introduction
- Chapter 1 - The Illusion
- Chapter 2 - The Three Operating Modes
- Chapter 5 - Preventing AI Drift
- Chapter 6 - Long-Term Project Survival

---

## Current Evidence Status

This evidence map is the first control layer.

It will be expanded as manuscript chapters are drafted.

No manuscript section should introduce a major principle that does not map back to this file or to a later evidence note.