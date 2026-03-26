# AGENTS

## Purpose

Build a minimal coding agent example for an engineering audience with Python skills.

- Primary use case: educational walkthrough in Jupyter.
- Python environment: `uv`.
- Dependency policy: keep dependencies minimal and easy to explain.
- Version control: use `git`.

## Working Style

- Prefer small, readable steps over clever abstractions.
- Keep the example easy to inspect in a notebook.
- Favor standard library code unless a dependency clearly improves the teaching value.
- Document tradeoffs briefly and directly.

## Memory System

Use a simple file-based memory system under `memory/`.

- `memory/project.md`: stable project context, goals, and constraints.
- `memory/decisions.md`: short design decisions and why they were made.
- `memory/next.md`: current next steps, open questions, and handoff notes.

Rules:

- Update memory only when something worth preserving changes.
- Keep entries short and append-only when possible.
- Store facts and decisions, not long transcripts.
- Before starting new work, read the memory files if they exist.
- After finishing meaningful work, update the relevant memory file.

## Environment

Use `uv` for local setup.


Keep additional packages to a minimum.

## Git Rules

- Commit only changes that have been tested.
- Prefer small, focused commits.
- Commit after each small completed chunk.
- Do not mix unrelated changes in one commit.
- If tests do not exist yet, run the smallest useful verification and note it.

## Jupyter Guidance

- Keep notebook cells short and sequential.
- Prefer examples that can be understood without framework knowledge.
