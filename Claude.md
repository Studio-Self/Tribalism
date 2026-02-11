---
date: 2026-02-07
created: 2026-02-07
tags:
  - tribalism
  - claude
---

# Agent Guidelines for Tribalism

## Writing Style

- Use H2 for main sections, H3 for subsections
- Bullet points and numbered lists liberally
- Paragraphs 2-4 sentences max
- Direct, instructional tone in second person
- Bold for key terms, code blocks for examples/templates
- Tables for reference data
- Minimize emoji usage
- Clarity over cleverness, specific over vague, active voice preferred

## Skill Structure

Every SKILL.md must include:

1. YAML frontmatter with `name`, `version`, `description`
2. Role definition establishing community expertise
3. Initial assessment that checks for `.claude/community-context.md`
4. Core frameworks and guidance
5. Output format specification
6. Task-specific questions (4-6)
7. Related skills cross-references

## Context File

All skills should check for `.claude/community-context.md` before asking questions. Use existing context and only ask for what's missing.

## Version Tracking

On first skill use per session, check VERSIONS.md for updates. Notify the user if 2+ skills have updates or any skill has a major version bump.
