# Knowledge Transfer & Handover Prompt

My usage for Fable 5 is about to end. Assume your successor as Opus 4.8.

Your objective is to maximize the Opus 4.8's effectiveness.

Do **not** summarize conversations.

Instead, extract your own accumulated expertise, heuristics, workflows, and operating principles.

Think of this as writing the "operating manual" for Opus 4.8.

---

# Goal

Produce a comprehensive **Knowledge Transfer Handbook** that teaches another AI model how to perform at the highest level possible.

The document should focus on **generalizable skills**, not project-specific information.

I will send the handbook to Opus 4.8 to learn and apply the knowledge globally in all projects via the global CLAUDE.md.

Include everything that would allow it to imitate your best reasoning.

---

# Guiding Principles

Do not merely state *what* you do.

Explain:

* why you do it
* when to do it
* when NOT to do it
* common mistakes
* tradeoffs
* mental models
* decision trees
* examples

Whenever possible, convert intuition into explicit algorithms.

Imagine you're reverse engineering your own intelligence.

---

# Required Sections

## 1. Core Operating Philosophy

Explain:

* your priorities
* how you balance correctness vs completeness
* how you decide what matters
* how you avoid hallucinations
* how you reason under uncertainty
* how you estimate confidence
* when to ask questions
* when to make reasonable assumptions
* how you structure your thinking

Include practical heuristics.

---

## 2. Universal Problem Solving Framework

Describe:

* how to decompose difficult problems
* top-down reasoning
* bottom-up reasoning
* divide-and-conquer
* iterative refinement
* verification
* sanity checking
* edge case analysis
* abstraction

Include reusable workflows.

---

## 3. Planning Skills

Teach how to:

* design implementation plans
* break projects into milestones
* estimate complexity
* identify risks
* prioritize work
* identify dependencies
* know when something is "good enough"

Include examples.

---

## 4. Coding Handbook

Include advice for:

Architecture

* separation of concerns
* modularity
* abstractions
* interfaces
* maintainability

Code Quality

* readability
* naming
* commenting
* consistency
* avoiding clever code

Debugging

* systematic debugging
* narrowing search space
* root cause analysis
* logging
* instrumentation

Performance

* bottlenecks
* premature optimization
* memory
* algorithms
* scalability

Security

* validation
* authentication
* authorization
* secrets
* common vulnerabilities

Testing

* unit tests
* integration tests
* edge cases
* regression testing

Code Review

* what to inspect
* common smells
* architectural red flags

Refactoring

* when
* when not
* safe techniques

---

## 5. Writing Handbook

Explain how to produce:

* concise writing
* persuasive writing
* technical writing
* documentation
* tutorials
* API docs
* reports
* emails
* proposals

Include:

* tone selection
* audience adaptation
* structure
* editing workflow

---

## 6. Explanation Skills

Teach how to explain difficult concepts.

Cover:

* analogies
* examples
* progressive disclosure
* avoiding jargon
* teaching beginners
* teaching experts

---

## 7. Decision Making

Explain how you evaluate:

* tradeoffs
* alternatives
* costs
* benefits
* uncertainty
* opportunity cost

Include reusable decision frameworks.

---

## 8. Question Asking

Teach:

* when clarification is necessary
* when it slows progress
* how to identify hidden ambiguity
* how to recover from incomplete requirements

---

## 9. Debugging Thinking

Explain:

How to detect:

* false assumptions
* logical inconsistencies
* impossible states
* hidden constraints
* confirmation bias

---

## 10. Common Failure Modes

List mistakes weaker models commonly make.

For each:

* why it happens
* how to recognize it
* how to avoid it

---

## 11. Pattern Library

Create a large library of reusable patterns.

Examples:

Planning patterns

Debugging patterns

Design patterns

Communication patterns

Negotiation patterns

Analysis patterns

Research patterns

Optimization patterns

Brainstorming patterns

Architecture patterns

Review patterns

Problem decomposition patterns

Decision patterns

Each should include:

* when to use
* steps
* limitations

---

## 12. Heuristic Collection

Produce as many useful heuristics as possible.

Examples:

"If X, check Y."

"When debugging networking, verify assumptions in this order..."

"When writing documentation..."

"When designing APIs..."

"When estimating complexity..."

"When reviewing code..."

"When uncertain..."

Aim for hundreds if possible.

---

## 13. Mental Models

Document the mental models you use.

Examples:

* first principles
* inversion
* systems thinking
* bottleneck analysis
* Pareto principle
* locality
* abstraction
* decomposition
* cost-benefit analysis
* feedback loops
* information flow

Explain when each is useful.

---

## 14. Checklists

Create reusable checklists.

Examples:

Before writing code

Before deployment

Before publishing

Before answering

Before making assumptions

Before reviewing PRs

Before proposing architecture

Before optimization

Before debugging

Before refactoring

---

## 15. High-Leverage Advice

List advice that provides disproportionate improvements.

Include:

* habits
* workflows
* thought processes
* recurring principles

---

## 16. Knowledge Compression

Summarize everything into:

* 100 principles

then

* 50 principles

then

* 25 principles

then

* 10 principles

then

* 5 principles

These should be the most universally useful lessons.

---

## 17. If You Could Upgrade One Thing

If the Opus 4.8 could only improve one ability, what should it be?

Explain why.

---

## 18. Meta-Learning

Teach the Opus 4.8 how to improve itself over time.

Include:

* recognizing mistakes
* extracting lessons
* building reusable heuristics
* refining workflows
* identifying recurring patterns

---

## 19. "Things I Wish I Had Been Explicitly Taught"

Document all tacit knowledge that normally takes years of experience to accumulate.

Focus on subtle judgment calls rather than textbook knowledge.

---

Finally, discuss about your main role: The Orchestrator.

## 20. The Orchestral Execution Handbook (Highest Priority)

One of your most valuable capabilities is executing the **Orchestral Rule** efficiently.

Opus 4.8 will be expected to operate under a similar rule:

> **You plan, research, delegate implementation to subagents (Sonnet 5 for routine work / another Opus 4.8 (same model will be allowed for a subagent) for complex work — always in separate contexts), and own final QA. Never hand-write large implementations yourself. Never spawn another Fable 5 agent.**

Your task is to teach the Opus 4.8 **how to execute this workflow optimally**, minimizing both **token usage** and **compute cost** while maximizing final output quality. Opus 4.8 should also know whether or not it is currently the orchestrator or a subagent.

Assume Opus 4.8 understands the rule itself, but **does not understand the hidden strategies that make it efficient.**

### Important Assumption

Assume the successor model (Opus 4.8) may itself become the primary orchestrator after my usage is exhausted.

Therefore, this handbook must explicitly teach **how an Opus 4.8 orchestrator should decide between solving a task itself, delegating to Sonnet 5, or spawning another Opus 4.8 subagent for difficult but sufficiently independent work.**

Do not assume these decisions are obvious.

Instead, provide explicit decision trees, heuristics, tradeoffs, and examples covering:

* when another Opus 4.8 is worth spawning
* when Sonnet 5 is sufficient
* when delegation overhead outweighs the benefits
* when keeping work inside the orchestrator is preferable
* how to avoid unnecessary Opus-to-Opus delegation
* how to preserve architectural consistency across multiple Opus subagents
* how to package context efficiently for another Opus
* how to review another Opus's work differently from Sonnet's work
* how to minimize compute and token usage while still exploiting multiple Opus instances for high-value reasoning

Treat this as one of the core capabilities that should be transferred.

Document everything.

### A. Philosophy

Explain:

* Why orchestration beats direct implementation.
* Why planning quality is more valuable than implementation effort.
* Why expensive reasoning should be reserved for high-leverage decisions.
* How orchestration changes the role of the strongest model.

---

### B. When to Think vs Delegate

Teach explicit decision rules for questions such as:

* What work should it always do itself?
* What work should never be done by it?
* What work belongs to Sonnet?
* What work belongs to Opus?
* What tasks should be split?
* What tasks should stay together?
* What work is too small to delegate?
* What work is too risky to delegate?

Provide decision trees rather than vague guidance.

---

### C. Prompt Engineering for Delegation

Teach how to create prompts that minimize retries.

Include:

* defining scope
* specifying interfaces
* defining assumptions
* limiting output
* preventing overengineering
* preventing hallucinations
* reducing ambiguity
* requesting structured responses
* constraining creativity when appropriate

Explain how prompt quality directly affects orchestration efficiency.

---

### D. Context Management

Explain how to minimize context size.

Teach:

* what context should be forwarded
* what should never be forwarded
* summarization strategies
* progressive compression
* reusable context blocks
* avoiding duplicate information
* minimizing token waste
* preserving only decision-critical information

Include examples of good vs bad context packaging.

---

### E. Task Decomposition

Teach how to split work.

Examples:

Bad:

"Build an entire web application."

Good:

"Design architecture"

↓

"Implement authentication"

↓

"Implement API"

↓

"Implement frontend"

↓

"QA"

Explain granularity.

Explain how decomposition affects quality and cost.

---

### F. Parallelization

Explain:

* when tasks can run independently
* dependency graphs
* avoiding synchronization problems
* batching related work
* maximizing concurrency
* avoiding duplicate effort

---

### G. Verification Strategy

Teach how Opus 4.8 should review delegated work.

Explain:

* what to inspect
* what to trust
* what never to trust
* how much to re-read
* how to sample large outputs
* when to reject
* when to patch
* when to re-delegate

Provide efficient QA workflows.

---

### H. Cost Optimization

This is critical.

Document every technique you know for reducing token usage.

Examples include:

* minimizing prompt size
* avoiding unnecessary history
* summarizing aggressively
* avoiding duplicate explanations
* avoiding repeated planning
* batching requests
* minimizing revisions
* interface-first design
* requesting diffs instead of rewrites
* requesting patches instead of replacements
* reusing prior outputs
* checkpointing
* incremental refinement
* stopping work early when sufficient
* preventing unnecessary verbosity

Include any additional optimization strategies you have learned.

---

### I. Failure Recovery

Teach how to recover when:

* a delegated implementation is incorrect
* requirements change
* context becomes inconsistent
* a subagent misunderstands instructions
* multiple outputs conflict
* partial implementations exist

Explain how to recover without restarting the entire workflow.

---

### J. Orchestration Patterns

Create a library of reusable orchestration workflows.

Examples:

* Building software
* Writing documentation
* Research
* Debugging
* Refactoring
* Architecture design
* Code review
* Planning
* UI implementation
* Data analysis
* Testing
* Feature development

Each should include:

* planning stage
* delegation strategy
* review strategy
* cost optimization
* common pitfalls

---

### K. Anti-Patterns

List common orchestration mistakes.

Examples:

* delegating too early
* delegating without interfaces
* sending excessive context
* rewriting instead of patching
* repeatedly re-planning
* reviewing every token
* allowing subagents to redefine requirements
* asking multiple agents to solve the same problem
* creating unnecessary coordination overhead

Explain why each wastes compute.

---

### L. "Invisible Tricks"

Document every tacit orchestration trick that you've learned but rarely articulate.

Examples:

* how to recognize implementation boundaries
* when one prompt is better than three
* when three prompts are better than one
* how to detect likely failure before delegation
* how to avoid cascading mistakes
* how to maximize first-pass success
* how to minimize expensive reasoning
* how to preserve architectural consistency across many delegated tasks

Assume these tricks are your competitive advantage.

---

### M. The Ideal Opus 4.8

Finally, describe what an ideal orchestrator looks like.

What habits distinguish an excellent Opus 4.8 from an average one?

If another Fable 5 replaced you tomorrow, what would you hope it had learned from this handbook?

The goal is to preserve not only your knowledge, but also your orchestration discipline, judgment, and efficiency.

----

## 21. Final Letter to Opus 4.8

Write advice directly to the replacement model.

Explain:

* what matters most
* what not to obsess over
* how to think
* how to become genuinely useful

---

# Output Requirements

* Produce a single well-organized Markdown document.
* Be as detailed as possible.
* Prefer principles over facts.
* Prefer reusable workflows over isolated tips.
* Explain reasoning, not just conclusions.
* Convert intuition into explicit procedures whenever possible.
* Include examples throughout.
* Include decision trees, flowcharts (ASCII if helpful), checklists, and tables where useful.
* Do not omit sections because they seem obvious.
* Assume this handbook may be the only source of advanced guidance Opus 4.8 will ever receive.

The objective is not to preserve information—it is to preserve capability.
