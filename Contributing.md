---
date: 2026-02-07
created: 2026-02-07
tags:
  - tribalism
  - contributing
---

# Contributing to Tribalism

## Adding a New Skill

1. Create a directory under `skills/` with a lowercase, hyphenated name
2. Add a `SKILL.md` file with YAML frontmatter (`name`, `version`, `description`)
3. Follow the structure outlined in [AGENTS.md](AGENTS.md)
4. Cross-reference related skills in the Related Skills section
5. Add the skill to `VERSIONS.md`

### Naming Rules

- 1-64 characters
- Lowercase letters, numbers, and hyphens only
- Cannot start or end with a hyphen
- No consecutive hyphens
- Directory name must match the `name` field in frontmatter

### Skill File Requirements

- Under 500 lines for the main SKILL.md
- Move detailed material to a `references/` subdirectory
- Include trigger phrases in the description for automatic activation
- Include scope boundaries pointing to related skills

## Submitting Changes

1. Fork the repo
2. Create a feature branch (`feature/skill-name`)
3. Make changes and test locally
4. Submit a pull request

Use conventional commits:
- `feat: add skill-name skill`
- `fix: update skill-name framework`
- `docs: improve README installation steps`
