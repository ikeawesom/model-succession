# Model Succession Pipeline

A lightweight prompt pipeline for preserving an AI coding agent's **reasoning methodology** across model handovers.

Designed primarily for **CLI LLM workflows** (such as Claude Code, Codex CLI, and similar agentic coding environments), where long-running projects often outlive a single model session.

While this repository was built around my own **Claude Code** workflow, the underlying ideas are intentionally model-agnostic and can be adapted to other coding agents.

The goal isn't to preserve conversations, but to preserve **capability**.

## Workflow

### 1. Generate the handbook

Start a conversation with your source model.

Provide it with `fable-handover.md`.

The model generates a **Knowledge Transfer Handbook** describing its reasoning process, planning methodology, heuristics, orchestration strategies, and operational principles.

Save the generated handbook.

### 2. Install the capabilities

Start a new conversation with your successor model.

Provide:

* `opus-learn.md`
* the generated **Knowledge Transfer Handbook**

The successor model transforms the handbook into a compact operating system, including artifacts such as:

* `OPERATING_MANUAL.md`
* `SYSTEM.md`
* `CLAUDE.md`

These compressed layers preserve the original handbook's capabilities while minimizing future context size and token usage.

## Philosophy

The **Knowledge Transfer Handbook** remains the canonical source of truth.

The generated operating system distills that knowledge into reusable layers that can be efficiently loaded into future projects and sessions.

Although the examples in this repository are based on **Claude Code**, the workflow is applicable to any CLI-based LLM that supports long-running, agentic software development.

Happy building! 🚀
