# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

Company Brain is the company's single source of truth in docs-as-code format: Markdown in Git, reviewed through Pull Requests. It is a knowledge base, not a codebase, so there is no build, linter or tests here.

Other tools (Slack, Notion, Drive, Gmail) feed this repository, but it is the source of truth. If data conflicts, what is written here is considered correct; the discrepancy should be shown to a human, not fixed silently.

## Structure

- `docs/about-company.md` — company, product, positioning
- `docs/team.md` — roles, responsibilities, onboarding new hires
- `docs/tools.md` — tools and admins (credentials are in 1Password)
- `docs/runbooks/` — step-by-step procedures: customer-onboarding, inbound-lead, support-escalation, billing, releases, hiring
- `docs/agents/` — registry of AI agents and automations
- `docs/team-rules/` — team rules: decisions, questions, customer-data, passwords, friday, language, claude
- `docs/info/` — reference information: out-of-office, kaffee-nord
- `README.md` — what this is, how it is organized, who is responsible for what
- `CONTRIBUTING.md` — hard rules and how to make changes
- `maintaining.md` — who maintains the Brain and how it stays up to date
- `GLOSSARY.md` — terms and abbreviations
- `open-questions.md` — unanswered questions
- `CODEOWNERS` — page owners for review

## Rules

Before any change, read `CONTRIBUTING.md` (full rules) and `maintaining.md` (who is responsible for the Brain and how it is maintained) and follow them.

### Answering questions about the company

First look for the answer in `docs/` (and in `GLOSSARY.md`, if relevant), and only then answer. Do not make things up: if there is no answer, say so directly. Cite the file the answer comes from.

### Changes

New information gets here only through a Pull Request, never directly into `main`.

One branch per logical change, i.e. per PR. If you are already working not in `main` but in a branch for the current task, keep working in it. Create a new branch only from `main` and only for a new, separate task. Never create separate folders or worktrees.

If a change adds, renames or deletes a document, update the 'Start here' table in README.md in the same PR so that it points only to files that exist.

In the same PR:

- update "Last reviewed" on all changed pages;
- if the change adds a page or changes its Owner/Backup, update `CODEOWNERS`.

### How to write pages

- Brain is written in English — Fernway's working language (see team rules). All new pages and edits must be in English, even if the request is in another language.
- Every new file starts with a `# ...` heading, followed directly by the block: `Owner: … · Backup: … · Last reviewed: YYYY-MM-DD`.
- Use only facts provided by a human. Do not make anything up.
- If there are no facts for a section, write `_To be filled._`.
- Record unknowns in `open-questions.md`.

### What must not be added

No file, example or commit message may contain:

- passwords, access keys, API keys, tokens — only state that they are in 1Password;
- customer contact details (phones, emails, addresses) — about customers we record only the customer company's name and the name of the contact person at that company;
- financial details;
- highly sensitive internal data (for example, salaries);
- personal notes and reflections of a specific person.

If such data appears in material that needs to be added, do not carry it over and tell the human about it.
