# AGENTS Guide for `dddsa`

> This repository is intentionally minimal. Use this guide to stay aligned when documenting, extending, or auditing it.

## 📘 Project Overview
- **Purpose:** Placeholder project maintained to demonstrate documentation workflows.
- **Current State:** Only `README.md` exists with the single heading `# dddsa`.
- **Key Implication:** Every modification is high-visibility—changes should be explicit, well-documented, and justified in pull requests.

## 🗂️ Repository Structure
```
.
├── README.md   # Stub description of the project
└── (you)       # Add new files only when absolutely necessary, with docs
```
- No source directories, configuration files, or dependencies are present.
- Creating any new path (e.g., `src/`, `docs/`) must be accompanied by rationale in commit messages and documentation updates.

## 🛠️ Development Guidelines
1. **Start with documentation.** Update `README.md` and this `AGENTS.md` before adding code.
2. **Keep history linear.** Rebase onto `main` before opening a PR.
3. **Isolate experiments.** Use feature branches named `feature/<short-description>`.
4. **Explain new assets.** When adding files, include a short purpose note at the top of the file or in accompanying docs.
5. **Prefer Markdown.** Until real code exists, communicate designs, specs, or plans as Markdown documents.

## ✅ Quality Standards
- **Clarity:** Every change must describe *why* it exists. Vague commits will be rejected.
- **Consistency:** Follow existing Markdown style—sentence case headings, concise bullet lists.
- **Traceability:** Reference issue IDs or task names when applicable.
- **Minimalism:** Avoid adding tooling or dependencies unless a documented use case demands them.

## 🚨 Critical Rules
- **Do not fabricate structure.** Only describe or reference files that actually exist.
- **Document before code.** Any new implementation requires an accompanying design note in `README.md` or a new Markdown file linked from it.
- **No binaries.** Store artifacts outside the repo; use links if needed.
- **Security hygiene:** Even though empty, treat secrets cautiously—never commit credentials, tokens, or sample secrets.

## 🧾 Common Tasks
| Task | Steps |
| --- | --- |
| Update README title/description | Edit `README.md`, ensure heading remains `# dddsa` unless renaming project, describe purpose underneath. |
| Propose new structure | Draft a section in `README.md` describing the planned structure; optionally include a tree diagram. |
| Add initial code file | Create a new directory (e.g., `src/`), add file with header comment explaining scope, update both `README.md` and `AGENTS.md`. |
| Document workflow | Add a new Markdown file under `docs/` (if created), reference it from `README.md`, summarize intent in PR body. |

## 🧩 Reference Examples
- **Repository tree snippet:** (above) shows expected formatting for future expansions.
- **Commit message template:**
  ```
  feat: describe change in <=50 chars
  
  - context for the change
  - summary of files touched
  - link to issue/task
  ```
- **PR checklist:**
  - [ ] README updated
  - [ ] AGENTS.md updated (if instructions changed)
  - [ ] Tests planned (if code introduced)
  - [ ] Rationale documented

## 📚 Additional Resources
- No external dependencies or tooling are defined yet.
- If you introduce tooling (e.g., Node.js, Python), document installation steps and version constraints immediately in `README.md`.
- Coordinate with repository owners via the main issue tracker (see workflow ticket) before large changes.

---
Need clarification? Start by opening an issue or draft PR outlining your questions and proposed next steps.
