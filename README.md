# paper-skills

A Claude Code plugin with reusable writing skills for Chinese technical papers
and graduation projects.

## Installation

### From Marketplace

```bash
# Add the marketplace
/plugin marketplace add woxQAQ/paper-skills

# Install the plugin
/plugin install paper-skills@paper-skills-marketplace
```

### From Git URL

```bash
/plugin install https://github.com/woxQAQ/paper-skills.git
```

### Local Development

```bash
# Clone the repository
git clone https://github.com/woxQAQ/paper-skills.git

# Use with Claude Code
claude --plugin-dir /path/to/paper-skills
```

### Using in codex

You can install this skills with Open your codex and call codex to install for
you

```
$skill-installer install all the skills under https://github.com/woxQAQ/paper-skills/tree/main/skills
```

## Available Skills

| Skill                                                 | Trigger Phrases                                         | Description                                                    |
| ----------------------------------------------------- | ------------------------------------------------------- | -------------------------------------------------------------- |
| `thesis-introduction-writer`                          | "write introduction", "绪论", "第一章"                  | Write and optimize the Introduction chapter (sections 1.1-1.5) |
| `thesis-requirements-analysis-writer`                 | "requirements analysis", "需求分析", "第三章"           | Write system requirements analysis with UML artifacts          |
| `thesis-system-overview-design-writer`                | "system design", "系统设计", "总体设计"                 | Write system overview design chapter                           |
| `thesis-system-detailed-design-implementation-writer` | "detailed design", "详细设计", "implementation", "实现" | Write detailed design and implementation                       |
| `thesis-system-testing-writer`                        | "system testing", "系统测试", "测试"                    | Write system testing chapter                                   |
| `project-technology-section-writer`                   | "technology selection", "技术选型", "相关技术"          | Write technology selection rationale                           |

## Structure

```
paper-skills/
├── .claude-plugin/
│   └── plugin.json          # Plugin manifest
├── skills/                  # All skill packages
│   └── <skill-name>/
│       ├── SKILL.md         # Workflow and usage instructions
│       ├── references/      # SOPs, templates, quality checklists
│       └── agents/          # Legacy agent metadata (optional)
├── marketplace.json         # Marketplace configuration
├── AGENTS.md               # Contributor guidelines
└── README.md               # This file
```

## Usage

Once installed, the skills are automatically available in Claude Code. Simply
describe what you need:

- "Help me write the introduction chapter for my graduation project about..."
- "Write the requirements analysis for a student management system..."
- "Review and improve my system testing section..."

Claude will automatically load the appropriate skill based on your request.

## Quick Checks

Run these before submitting changes:

```bash
rg --files skills
find skills -maxdepth 3 -type f | sort
python -c "import yaml, pathlib; [yaml.safe_load(p.read_text()) for p in pathlib.Path('skills').glob('*/agents/*.yaml')]"
```

## Contributing

Please follow `AGENTS.md` for naming, style, testing, and pull request
expectations.

## License

MIT
