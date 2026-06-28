# Chapter 3

## Build Contracts, Not Chaos

### Mission Brief

Every engineering project begins with an objective.

Very few begin with a contract.

The difference appears small.

It is not.

Objectives describe what we hope to achieve.

Contracts define what is allowed while trying to achieve it.

Artificial intelligence dramatically increases the number of possible solutions that can be proposed during development. Without explicit boundaries, every conversation introduces new alternatives, new optimizations, and new directions.

The challenge is no longer generating ideas.

The challenge is deciding which ideas are permitted to influence the project.

Engineering contracts exist to answer that question.

Objectives establish direction, but direction alone rarely produces consistent engineering outcomes. Different engineers may interpret the same objective differently, and an AI system can generate dozens of equally plausible paths toward it. Without an explicit agreement on boundaries, implementation becomes an exercise in continuous interpretation rather than disciplined execution.

A contract reduces that uncertainty before the first change is made. It captures the decisions that should remain stable throughout implementation, allowing subsequent work to focus on execution rather than repeatedly renegotiating intent. In that sense, the contract is not documentation produced after engineering. It is the first engineering artifact created before engineering truly begins.

---

## Core Principle

A contract is not legal language.

It is engineering language.

It defines the operating boundaries of a task before implementation begins.

A good engineering contract answers questions that should never be negotiated in the middle of execution.

What is the objective?

What is outside the scope?

What must not change?

How will success be measured?

What evidence will prove completion?

What evidence will reject the proposed solution?

Once these questions have been answered, implementation becomes significantly calmer.

The conversation stops debating purpose.

It begins executing purpose.

Writing a contract is not merely an act of communication. It is an act of engineering in its own right. The effort required to define objectives, scope, constraints, and verification often exposes questions that remained invisible while the project existed only as an idea. Assumptions that appeared obvious suddenly require explicit decisions. Ambiguities that would have surfaced during implementation become visible while they are still inexpensive to resolve.

This discipline benefits both the engineer and the AI. The assistant receives clearer boundaries for execution, while the engineer gains a more precise understanding of the work itself. Many implementation problems are ultimately specification problems that simply remained hidden until construction had already begun. A contract brings those problems forward, where they can be addressed deliberately instead of reactively.

---

## Real Engineering Experience

One of the most important discoveries during long-running AI-assisted development was that ambiguity compounds.

A task would begin with a clear intention.

Halfway through the discussion, an adjacent improvement would appear.

Then another.

Then another.

Each suggestion was individually reasonable.

Collectively they transformed a focused engineering task into an architectural redesign.

Nothing malicious had happened.

Nothing irrational had happened.

The assistant was doing exactly what it had been designed to do.

It was generating useful possibilities.

The engineering process, however, had failed to distinguish between possibilities and permission.

That distinction eventually became the turning point.

Before implementation began, every significant task was preceded by an explicit engineering contract.

The conversation immediately became shorter.

More focused.

More predictable.

Most importantly, it became recoverable.

Weeks later, it remained obvious why the work had been performed and equally obvious why other ideas had deliberately been postponed.

The contract had preserved the decision.

Not the conversation.

---

## Objectives Before Solutions

One of the easiest ways to lose control of an engineering project is to begin discussing solutions before agreeing on the objective.

Solutions multiply naturally.

Objectives should remain remarkably stable.

A contract therefore begins with a single sentence.

Objective:

<Describe exactly what success looks like.>

Everything that follows exists to support that objective.

Nothing exists to compete with it.

## Scope Is an Engineering Tool

Every project has more work available than it has time.

Artificial intelligence magnifies this imbalance by continuously producing additional possibilities.

Some of those possibilities are valuable.

Most are simply outside the current objective.

Scope exists to protect engineering effort from engineering enthusiasm.

A contract therefore defines not only what will be done, but what will deliberately remain untouched.

Typical scope statements include:

- Components that may be modified.
- Components that are read-only.
- Architectural layers excluded from the task.
- Behaviour that must remain unchanged.
- Features explicitly postponed.
- Risks accepted for this implementation.

Without scope, every improvement competes equally for attention.

With scope, engineering becomes selective.

Selection is one of the highest forms of engineering discipline.

---

## Constraints

Constraints are often misunderstood.

Many engineers treat constraints as obstacles.

In reality they are design tools.

Every meaningful engineering solution exists inside constraints.

Time.

Resources.

Architecture.

Compatibility.

Performance.

Maintainability.

Human understanding.

Removing all constraints rarely produces a better solution.

It usually produces an uncontrolled one.

Well-defined constraints reduce unnecessary creativity.

They allow creativity to focus where it matters.

The contract should therefore identify every significant constraint before implementation begins.

When later decisions appear difficult, the constraints already provide much of the answer.

---

## Success Criteria

A surprising number of engineering tasks begin without defining success.

The result is predictable.

Implementation continues until everyone becomes tired.

A contract prevents this.

Success must become observable.

Not emotional.

Not intuitive.

Observable.

Good success criteria are measurable.

For example:

- The defect no longer appears.
- Existing behaviour remains unchanged.
- All tests pass.
- Runtime telemetry confirms the expected outcome.
- No regressions are introduced.
- Verification completes successfully.

Notice that none of these depend upon opinion.

Engineering finishes when reality satisfies the contract.

Not when the discussion feels complete.

---

## Frozen Scope

Once planning has finished, the contract becomes temporarily frozen.

This does not prevent better ideas.

It simply postpones them.

Every project accumulates improvements faster than it can safely implement them.

The disciplined engineer writes those ideas down.

Then returns to the contract.

The current task deserves completion before the next task begins.

A frozen scope is not resistance to improvement.

It is respect for continuity.

Projects that constantly redefine themselves rarely finish anything well.

Projects that finish one disciplined step at a time accumulate remarkable progress.

## Engineering Rule

Every significant engineering task deserves its own contract before implementation begins.

The contract does not need to be lengthy.

It needs to be unambiguous.

At a minimum, it should answer five questions.

1. What is the objective?

2. What is the scope?

3. What constraints exist?

4. How will success be verified?

5. What is explicitly forbidden?

Once those questions have been answered, implementation becomes execution rather than discovery.

Discovery belongs in exploration.

Execution belongs in implementation.

The contract separates the two.

---

## Failure Pattern

A project begins with a simple objective.

An improvement is suggested.

Then another.

The discussion shifts toward architecture.

Someone notices a different optimization.

A related defect is discovered.

The implementation grows.

Verification becomes difficult.

The original objective quietly disappears.

Weeks later the team has produced a large amount of work.

Very little of it solves the original problem.

Nothing catastrophic occurred.

The project simply lacked a contract.

Chaos rarely announces itself.

It accumulates.

---

## Field Notes

The shortest engineering contracts often become the most valuable.

One page is usually enough.

The goal is not documentation.

The goal is preserving intent.

If an engineer returns six months later and immediately understands why a change exists, the contract has succeeded.

If they must reconstruct the reasoning from commit history and memory, the contract was incomplete.

The contract is not written for today's implementation.

It is written for tomorrow's engineer.

Often, that engineer is you.

---

## Practical Checklist

Before implementation begins, confirm:

- Is the objective written in one sentence?
- Is the scope clearly defined?
- Are forbidden changes listed?
- Are constraints identified?
- Are success criteria measurable?
- Is the verification method defined?
- Has the implementation sequence been decided?
- Is there a rollback strategy if the change fails?

If several of these questions remain unanswered, planning is incomplete.

Continue planning.

Do not begin implementation.

---

## Common Mistakes

Beginning implementation while the objective is still evolving.

Treating every suggestion as part of the current task.

Allowing adjacent improvements to expand the scope.

Changing architectural decisions during implementation.

Defining success after implementation has already begun.

Assuming everyone understands the objective without writing it down.

Confusing productive discussion with engineering progress.

---

## Engineering Laws

**Law 1**

Objectives inspire.

Contracts govern.

**Law 2**

Every undefined boundary eventually becomes a source of drift.

**Law 3**

A frozen scope protects engineering effort.

**Law 4**

Constraints improve engineering more often than they restrict it.

**Law 5**

Implementation should execute decisions, not discover them.

**Law 6**

A contract preserves intent long after conversations have been forgotten.

---

## Chapter Summary

Engineering succeeds when decisions become explicit before work begins.

Contracts transform intention into structure.

They preserve objectives.

They define boundaries.

They reduce ambiguity.

They protect continuity.

Artificial intelligence increases the number of possible solutions.

Engineering contracts determine which of those solutions are permitted to become reality.

The stronger the contract, the calmer the implementation.

The next chapter builds upon this foundation by replacing opinion with evidence, showing why telemetry, diagnostics, verification, and canonical sources of truth consistently outperform intuition during long-running engineering work.

---

## Field Reflection

> "Men in general judge more by the eye than by the hand, because everyone can see, but few can truly understand."

> - Niccolo Machiavelli, *The Prince*

Engineering suffers from the same temptation.

A convincing explanation is easy to see.

A disciplined process requires deeper understanding.

Contracts force engineering to move beyond appearances.

They replace assumption with explicit agreement.

That discipline becomes one of the strongest defenses against drift in AI-assisted engineering.
