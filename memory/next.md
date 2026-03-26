# Next

- 2026-03-25: Live-tested the notebook logic against a temporary copy of the repo using the environment `OPENAI_API_KEY`. The agent completed a two-step inspect-and-summarize task successfully.
- 2026-03-25: Updated the notebook so each build step is followed by a small test cell, switched to a pasted `api_key` variable, added function docstrings, and changed the demo task to a compiled C++ hello-world example.
- 2026-03-25: Live-tested the updated notebook logic against a temporary copy of the repo. The agent created `hello.cpp`, compiled `hello`, and the manual `./hello` run printed `Hello World`.
- 2026-03-25: Kept the Lorenz-attractor example and made a Fortran logistic-map workflow the final example. The final example asks the notebook agent to write, compile, and run Fortran code that generates logistic-map bifurcation data for plotting.
- 2026-03-25: Added `matplotlib` to the project with `uv` so the final plotting example can run in the local notebook environment.
- 2026-03-25: Updated the notebook defaults so the agent examples use model `gpt-5.4`, `max_steps=50`, and `timeout=120`.
- 2026-03-25: Updated the notebook agent loop so plain-text assistant replies prompt for human input; the run now stops only when the human submits an empty reply or `max_steps` is reached.
- 2026-03-26: Added a top-level README that explains the repo goal, `uv` setup, notebook contents, and inspiration links.
- 2026-03-26: Updated the README title and added a note explaining that `AGENTS.md` and `memory/` are included to show the development harness used for the project.
- 2026-03-26: Replaced the placeholder `pyproject.toml` description with a short project summary that matches the notebook-first scope.
- 2026-03-26: Added a prominent Google Colab launch link to the top of the README so readers can open the notebook directly from GitHub.
- 2026-03-26: Simplified the README Colab link so only the badge is shown.
- Run the notebook interactively with a pasted real `OPENAI_API_KEY`.
- If needed later, add one follow-up notebook on safety limits and edit validation.
