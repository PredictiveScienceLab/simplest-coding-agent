# Simplest Coding Agent in a Jupyter Notebook

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PredictiveScienceLab/simplest-coding-agent/blob/main/notebooks/minimal_coding_agent.ipynb)

This repo is a small, notebook-first walkthrough of how to build a
minimal coding agent.

It is aimed at engineers who already know Python and want to see the
core idea without a framework:

1. send a conversation to a model
2. detect a fenced `bash` block in the reply
3. run the command
4. feed the result back
5. ask the human for input when there is no command

The main teaching artifact is `notebooks/minimal_coding_agent.ipynb`.

## Setup

This project uses `uv`.

```bash
uv sync
```

Then start Jupyter:

```bash
uv run jupyter notebook
```

Open `notebooks/minimal_coding_agent.ipynb`.

## What The Notebook Covers

- a minimal agent loop using the Python standard library
- direct HTTP calls to the OpenAI Responses API
- shell execution with `subprocess`
- a C++ hello-world example
- a Lorenz attractor example
- a Fortran example that generates logistic-map bifurcation data and
  plots it

## API Key

The notebook is designed to use only `OPENAI_API_KEY`.

- Early examples use a pasted `api_key` variable in the notebook.
- Do not save a real key into the notebook file.

## Repo Layout

- `notebooks/minimal_coding_agent.ipynb`: main walkthrough
- `memory/project.md`: stable project context
- `memory/decisions.md`: short design decisions
- `memory/next.md`: next steps and handoff notes

## Inspiration

- Geoffrey Huntley: https://ghuntley.com/agent/
- `mini-swe-agent`: https://github.com/SWE-agent/mini-swe-agent

## Development Harness

I include `AGENTS.md` and the `memory/` folder to demonstrate the
harness I used while developing this project.

- `AGENTS.md` captures the working rules and development constraints I
  gave the coding agent.
- `memory/project.md`, `memory/decisions.md`, and `memory/next.md`
  form a simple file-based memory system for project context, design
  decisions, and handoff notes.

These files are not part of the minimal agent itself. They are part of
the process used to build the notebook and keep the work organized.
