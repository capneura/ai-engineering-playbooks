# Chapter 2

# The Three Operating Modes

## Explore. Plan. Verify.

### Mission Brief

AI-assisted engineering becomes unstable when different kinds of work are mixed together.

Exploration is not planning.

Planning is not implementation.

Implementation is not verification.

Verification is not redesign.

When these modes collapse into one conversation, the project begins to drift. The assistant may still sound useful, but the engineering process becomes progressively harder to control.

The first practical discipline of AI-assisted engineering is therefore simple:

**Declare the operating mode before the work begins.**

---

## Core Principle

Most failures during AI collaboration begin because the human and the assistant are silently performing different kinds of work.

The human believes the discussion is exploratory.

The assistant begins planning.

The human requests analysis.

The assistant proposes implementation.

The human asks for verification.

The assistant introduces an entirely new theory.

None of these responses are necessarily wrong.

They simply belong to different engineering activities.

When those activities become mixed together, engineering loses structure.

The solution is not to limit AI.

The solution is to structure the collaboration.

This manual defines three primary operating modes:

- Explore
- Plan
- Verify

Implementation exists as a separate activity, but it must never begin until planning has been completed and deliberately frozen.

---

## Real Engineering Experience

One recurring pattern became impossible to ignore during long-running AI-assisted development.

Conversations almost always began correctly.

A problem appeared.

The goal was to understand it.

Ideas were explored.

Possible causes were discussed.

Evidence was collected.

Then something subtle happened.

Without anybody explicitly deciding to change modes, exploration quietly became planning.

Planning then became implementation.

Implementation became redesign.

By the end of the session, modifications had been proposed or even completed before the original problem had been fully understood.

The visible failure appeared to be inconsistent AI behaviour.

The real failure was the absence of operating discipline.

The engineering process had never established what kind of work was actually being performed.

---

## Mode 1 - Explore

Explore mode exists for one purpose:

**Understanding.**

Nothing more.

It does not authorize implementation.

It does not authorize redesign.

It does not authorize architectural change.

Its responsibility is to expand understanding.

Typical outputs include:

- observations
- possible causes
- unanswered questions
- required evidence
- competing hypotheses
- uncertainty lists
- system maps
- risk identification

Explore mode is intentionally permissive.

Ideas are allowed.

Speculation is allowed.

Questions are encouraged.

Decisions are not.

The most common mistake during exploration is confusing discovery with permission.

Finding a promising explanation does not justify changing the system.

Exploration earns the right to plan.

Nothing more.

---

## Mode 2 - Plan

Planning transforms understanding into controlled action.

Every engineering decision should become explicit before implementation begins.

A proper plan identifies:

- objective
- scope
- constraints
- success criteria
- forbidden changes
- implementation order
- verification strategy
- rollback conditions

A good engineering plan is rarely exciting.

Its purpose is not inspiration.

Its purpose is reducing uncertainty.

One of the most valuable functions of planning is protecting scope.

AI naturally generates adjacent improvements.

Many are useful.

Few belong inside the current task.

Planning prevents today's objective from quietly becoming tomorrow's redesign.

---

## Mode 3 - Verify

Verification answers one question.

**Did reality behave as expected?**

Nothing else.

Verification does not begin with explanation.

It begins with observation.

Typical verification outputs include:

- command results
- runtime behaviour
- logs
- telemetry
- diagnostics
- pass/fail evaluation
- comparison against success criteria
- remaining uncertainty

Verification protects engineering from belief.

Confidence may justify investigation.

Only evidence justifies conclusion.

---

## The Forbidden Mixture

The most dangerous AI response is not an incorrect answer.

It is a correct answer delivered at the wrong time.

Implementation during exploration.

Redesign during verification.

New theories during implementation.

Every one of these may be technically sound.

Every one of them introduces unnecessary instability.

The important question is not merely:

"Is this a good idea?"

It is:

"Does this belong in the current operating mode?"

That single question prevents an extraordinary amount of engineering drift.

---

## Engineering Rule

Every AI-assisted engineering session begins by declaring its operating mode.

If the session is exploratory, implementation is forbidden.

If the session is planning, code remains unchanged.

If the session is verification, redesign is postponed unless evidence proves it necessary.

Changing modes is allowed.

Changing modes silently is not.

---

## Failure Pattern

The same pattern appears repeatedly.

A problem emerges.

Investigation begins.

One explanation appears convincing.

Planning starts before investigation ends.

Implementation begins before planning stabilizes.

Verification becomes superficial.

Unexpected behaviour appears.

The original diagnosis is forgotten.

The team now debates symptoms instead of causes.

This is not a model failure.

It is a process failure.

---

## Field Notes

Declaring the operating mode creates productive resistance.

It becomes acceptable to interrupt the conversation.

"We are still exploring."

"That belongs in planning."

"We have not reached verification yet."

These interruptions slow individual conversations.

They accelerate long-term engineering.

Momentum alone is not progress.

Direction matters.

---

## Practical Checklist

Before every engineering session, ask:

- What operating mode are we entering?
- What outcomes are expected?
- What actions are forbidden?
- What evidence is required before moving forward?
- How will success be verified?
- Who decides when the operating mode changes?

If these questions remain unanswered, the project is already vulnerable to drift.

---

## Common Mistakes

Treating exploration as planning.

Treating planning as implementation.

Treating implementation as verification.

Accepting convincing explanations without evidence.

Changing objectives while solving the current problem.

Assuming the assistant automatically understands the current operating mode.

It does not.

The mode must always be explicit.

---

## Engineering Laws

**Law 1**

A session without an operating mode eventually becomes every operating mode.

**Law 2**

Exploration discovers possibilities.

It never authorizes change.

**Law 3**

Planning freezes intention before implementation begins.

**Law 4**

Verification tests reality, not confidence.

**Law 5**

A correct answer delivered in the wrong mode is still a process failure.

**Law 6**

Silent mode changes are engineering drift.

---

## Chapter Summary

Operating modes are not bureaucracy.

They are engineering control.

Explore protects understanding.

Plan protects intention.

Verify protects reality.

Artificial intelligence becomes significantly easier to manage once each activity occupies its proper place.

Before deciding what work should be done, engineers must first decide what kind of work is being performed.

That distinction becomes the foundation for every remaining chapter in this manual.

---

## Field Reflection

> "A prince ought to have no other aim or thought, nor select anything else for his study, than war and its rules and discipline."

> - Niccolò Machiavelli, *The Prince*

The point is not war.

The point is discipline.

Artificial intelligence grants engineers remarkable capability.

Discipline determines whether that capability produces coherent systems or increasingly sophisticated confusion.

Power without discipline creates instability.

Engineering without operating modes does the same.