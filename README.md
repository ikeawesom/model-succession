# Model Succession Pipeline

If you spend enough time using coding agents from the terminal, you've probably had this thought:

> *"My favorite model is about to hit its usage limit... now what?"*

This repository is for **CLI LLM users**. Whether you're using Claude Code today, Codex tomorrow, or whatever comes next.

The idea is simple: **don't just hand over the conversation. Hand over the capability.**

## Workflow

### 1. Extract the capability

Give your current model `fable-handover.md` (Fable 5, in my case).

Instead of summarizing your project, it generates a **Knowledge Transfer Handbook** that externalizes its reasoning process, planning discipline, heuristics, orchestration strategies, and operational knowledge.

Save the handbook.

### 2. Install the capability

Start a fresh session with your successor model (Opus 4.8, in my case).

Provide:

* `opus-learn.md`
* the generated **Knowledge Transfer Handbook**

The new model converts the handbook into a lightweight operating system (`SYSTEM.md`, `CLAUDE.md`, `OPERATING_MANUAL.md`, and more) designed to restore the original model's working style while minimizing future context and token usage.

## Why?

Long-running AI-assisted projects accumulate more than code.

They accumulate judgment.

This workflow helps preserve that judgment across model switches, usage limits, and future generations of coding agents.

## My workflow

I built this around **Claude Code**, where orchestrator handovers between models are a natural part of longer projects.

The concepts, however, are intentionally model-agnostic. Any CLI coding agent with multiple models and long-lived contexts could adopt a similar capability transfer workflow.

If this saves you from the dreaded *"90% usage remaining"* moment, then it has already done its job.

Happy building. 🚀

---

## Important notes

This workflow **does not retrain or permanently improve** the successor model.

It cannot make a weaker model "become" a stronger one.

Instead, it provides structured guidance describing **how the predecessor model approached problems**, i.e. its planning methodology, reasoning workflows, heuristics, orchestration strategies, and operational discipline.

Think of it as handing over an experienced engineer's playbook rather than upgrading the engineer's IQ.

The successor model still operates within its own capabilities, knowledge and reasoning limits. The generated artifacts simply help it adopt a more consistent and effective way of working, reducing the amount of methodology that needs to be rediscovered during long-running projects.

Your mileage will therefore depend on the successor model's own capabilities. Better models are generally able to internalize and apply the transferred operating methodology more faithfully than weaker ones.

These prompts are soley for Claude Code's Fable 5 and Opus 4.8. You may choose to update the necessary models for your use cases.

_Last updated: 7 July 2026_
