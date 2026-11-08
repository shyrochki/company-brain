# How to contribute

> **Owner:** Oleksandra Riabtseva · **Backup:** unassigned · **Last reviewed:** 2026-11-08

These rules are the same for humans and AI agents.

## Hard rules

- All changes go only through a Pull Request, never directly into `main`.
- No passwords, API keys, access tokens. Instead of a secret, we write where it is stored (1Password).
- About customers we record only the customer company's name and the name of the contact person at that company; no contact details (phones, emails, addresses).
- No salaries, private employee data, personal notes or reflections.
- Only recorded information. We do not make up unknowns — we add them to `open-questions.md`.
- When answering a question, cite the source file.
- Every page starts with the `Owner · Backup · Last reviewed` block.
- If a question has been asked twice — add the answer to the Brain.
- If a change adds, renames or deletes a document, update the 'Start here' table in `README.md` in the same PR so that it points only to files that exist.
- Brain is written in English — Fernway's working language (see team rules). All new pages and edits must be in English, even if the request is in another language.

## How to make a change

1. One branch per logical change, i.e. per PR. If you are already working not in `main` but in a branch for the current task, keep working in it. Create a new branch only from `main` and only for a new, separate task. Never create separate folders or worktrees.
2. Make the edit.
3. Update the `Last reviewed` date in the block at the top of the page.
4. Open a PR and write in one line what changed and why.
5. The PR is approved by the page owner (Owner).

## Exceptions

- `docs/team.md` and `docs/runbooks/hiring.md` — a PR is required, owner approval is not.
