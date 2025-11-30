# GitHub Copilot Instructions for `arkenidar`

This is the special profile repository for `@arkenidar`.
Its `README.md` appears on the public GitHub profile; treat the root as profile-facing and subfolders as experiments.

## General Principles
- Prefer **small, focused changes** over large refactors.
- Avoid introducing heavy dependencies or tools unless explicitly requested.
- When adding files, keep names clear and descriptive; avoid deep nesting unless there’s an obvious need.
- Default to **plain, well‑commented code** that is easy to learn from.

## Communication & Style
- Treat `README.md` as user-facing profile content; avoid large rewrites unless explicitly requested.
- Prefer small, composable edits (new sections, bullets, links) over full rewrites.
- Explain non‑obvious design choices in a few comments or in the most relevant `README.md`.
- Use clear, explicit naming over brevity (`total_count` instead of `cnt`).
- Keep responses and generated docs concise; avoid boilerplate text.

## Languages & Tooling
- Assume a **Linux + bash** environment.
- When suggesting commands, use bash‑compatible syntax and keep them copy‑pasteable.
- If you introduce a new language or framework, also add a short section to `README.md` explaining how to run or build it.

## Project Organization
- Keep the repository root tidy so the profile `README.md` stays focused on how the user presents themselves.
- When adding new work:
  - Group related code in folders (`src/`, `scripts/`, `experiments/`, etc.) instead of the repo root.
  - Prefer **one folder per experiment** with its own mini `README.md`.
  - In the root `README.md`, at most add a short bullet or link to notable experiments or tools.

## Tests & Verification
- If you add non‑trivial code, provide at least a minimal way to verify it:
  - For scripts: an example command in `README.md` or a `--help` option.
  - For libraries: a tiny demo script or example usage block.
- Use simple, standard tooling (e.g., `pytest` for Python, `npm test` for Node) only when clearly needed; document any new test command you introduce.

## Working With AI Agents
- Before creating larger features, **summarize your proposed structure** in the conversation so the user can adjust it.
- When editing existing files, preserve the current style and do not reformat unrelated code.
- Avoid adding license or copyright headers; the repo already has a `LICENSE`.
- Do not create git branches or commits unless the user asks.

## Examples of Good Contributions
- Add a small, self‑contained tool or script in a new directory (e.g., `tools/word_counter/`) with:
  - Source code
  - A short `README.md` describing usage
- Improve profile documentation by adding or refining concise sections in the root `README.md` (e.g., bio, links, selected projects), without overloading it with technical detail.

---
If the repository later gains a more defined structure (apps, libraries, docs), update this file to document:
- Main components and their directories
- Build / run / test commands
- Any project‑specific patterns or conventions.
