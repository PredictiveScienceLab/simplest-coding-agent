# Decisions

- 2026-03-25: Use a notebook-first walkthrough instead of hiding logic in modules. Reason: easier to inspect step by step in Jupyter.
- 2026-03-25: Use the OpenAI Responses API over raw HTTP with `urllib.request`. Reason: keeps dependencies at standard-library only while matching current OpenAI guidance for new projects.
- 2026-03-25: Use a fenced `bash` block as the agent protocol instead of formal tool calling. Reason: smallest possible control loop for teaching.
- 2026-03-25: Keep the API key as an explicit notebook variable that the reader pastes locally. Reason: makes the credential flow obvious in a teaching notebook and avoids hidden environment setup in the walkthrough.
- 2026-03-25: Add `matplotlib` as a project dependency for the Lorenz-attractor example. Reason: plotting is the one case where a small extra dependency materially improves the teaching value.
