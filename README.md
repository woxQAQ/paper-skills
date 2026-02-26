# paper-skills

A repository of reusable writing skills for thesis and project documentation workflows.

## Structure

- `skills/` — all skill packages
  - `*/SKILL.md` — workflow and usage instructions
  - `*/agents/openai.yaml` — agent metadata and default prompt
  - `*/references/*.md` — SOPs, templates, and quality checklists
- `AGENTS.md` — contributor guidelines for this repository

## Available Skill Domains

Current skills cover:
- thesis introduction writing
- requirements analysis writing
- system overview design writing
- detailed design and implementation writing
- system testing writing
- project technology section writing

## Quick Checks

Run these before submitting changes:

```bash
rg --files skills
find skills -maxdepth 3 -type f | sort
python -c "import yaml, pathlib; [yaml.safe_load(p.read_text()) for p in pathlib.Path(skills).glob(*/agents/*.yaml)]"
```

## Contributing

Please follow `AGENTS.md` for naming, style, testing, and pull request expectations.
