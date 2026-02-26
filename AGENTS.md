# Repository Guidelines

## Project Structure & Module Organization
This repository stores reusable writing skills under `skills/`. Each skill lives in `skills/<skill-name>/` and should include:
- `SKILL.md`: workflow, scope, and usage rules.
- `agents/openai.yaml`: agent-facing metadata (`display_name`, prompt text, etc.).
- `references/*.md`: SOPs, templates, and quality checklists used by the skill.

Use kebab-case for skill directory names (for example, `thesis-system-testing-writer`). Keep related references close to the skill that uses them.

## Build, Test, and Development Commands
There is no build pipeline in this repo; changes are content-first. Use these checks before opening a PR:
- `rg --files skills` — verify expected files are present.
- `find skills -maxdepth 3 -type f | sort` — quick structure audit.
- `python -c "import yaml, pathlib; [yaml.safe_load(p.read_text()) for p in pathlib.Path(skills).glob(*/agents/*.yaml)]"` — validate agent YAML syntax.

## Coding Style & Naming Conventions
- Markdown: use clear headings, short paragraphs, and task-oriented bullet lists.
- Keep instructions imperative and specific ("Run quality checks", not "Quality checks should be run").
- File names: lowercase kebab-case for docs; keep checklist/template names descriptive.
- YAML: 2-space indentation; quote strings only when needed for clarity.

## Testing Guidelines
Testing is lightweight and review-driven:
- Verify each `SKILL.md` references real local files.
- Ensure referenced paths are relative to that skill directory.
- For workflow edits, run a dry read-through from input collection to output to confirm no missing steps.
- Prefer adding or updating a checklist in `references/` when introducing new requirements.

## Commit & Pull Request Guidelines
This branch currently has no commit history, so use Conventional Commits from now on:
- `feat: add thesis-system-testing-writer checklist`
- `docs: clarify introduction workflow assumptions`

PRs should include:
- a short purpose statement,
- impacted paths (for example, `skills/thesis-introduction-writer/`),
- before/after behavior summary,
- sample output snippet when prompts or workflow logic change.

## Security & Configuration Tips
Do not commit secrets, API keys, or private project data in examples. Keep examples anonymized and reusable across institutions/projects.
