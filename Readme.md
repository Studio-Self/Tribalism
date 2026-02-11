---
date: 2026-02-07
created: 2026-02-07
tags:
  - tribalism
  - readme
---

# Tribalism: Community Building Skills for Claude Code

A comprehensive skill set for community managers, builders, and growth hackers. Everything you need to build, grow, and sustain thriving communities — from zero to scale.

## What This Is

Tribalism is a collection of 21 interconnected skills that give Claude deep expertise in community building. Each skill covers a specific domain and cross-references related skills, so you get expert guidance whether you're launching a Discord server, designing an ambassador program, or scaling community-led growth.

## Skills

### Foundation
| Skill | What It Does |
|-------|-------------|
| **community-context** | Shared context document about your community (read by all other skills) |
| **community-strategy** | Overall community planning, architecture, and positioning |
| **platform-selection** | Choosing the right platform (Discord, Slack, Circle, forum, etc.) |
| **community-culture** | Values, norms, identity, and belonging |

### Launch & Growth
| Skill | What It Does |
|-------|-------------|
| **community-launch** | Launching a new community from scratch |
| **community-growth** | Acquisition, viral loops, and member-led growth |
| **community-led-growth** | CLG strategy — community as a business growth engine |
| **community-partnerships** | Cross-community collabs, co-marketing, ecosystem building |

### Engagement & Retention
| Skill | What It Does |
|-------|-------------|
| **member-onboarding** | New member activation and first experiences |
| **engagement-programs** | Rituals, events, challenges, and content programs |
| **community-events** | AMAs, meetups, hackathons, summits |
| **community-content** | Content strategy for community channels |
| **retention-reactivation** | Churn prevention, win-back, re-engagement |

### Programs & Operations
| Skill | What It Does |
|-------|-------------|
| **ambassador-program** | Champions, ambassadors, and power user programs |
| **moderation-governance** | Rules, moderation, conflict resolution, trust & safety |
| **community-ops** | Tooling, automation, workflows, and team structure |
| **community-metrics** | Health metrics, dashboards, and reporting |

### Advanced
| Skill | What It Does |
|-------|-------------|
| **community-monetization** | Paid communities, sponsorships, premium tiers |
| **community-feedback** | Feedback loops, product input, voice of community |
| **developer-community** | DevRel, docs community, open source community |
| **crisis-management** | Handling community crises, PR issues, trust repair |

## Installation

### CLI Install (Recommended)

```bash
npx skills add Studio-Self/Tribalism
```

Install a single skill:

```bash
npx skills add Studio-Self/Tribalism --skill community-strategy
```

List available skills:

```bash
npx skills add Studio-Self/Tribalism --list
```

### Clone and Copy

```bash
git clone https://github.com/Studio-Self/Tribalism.git
cp -r Tribalism/Skills/* .claude/skills/
```

### Git Submodule

```bash
git submodule add https://github.com/Studio-Self/Tribalism.git .claude/tribalism
```

## How Skills Work

Skills activate automatically when your conversation matches their trigger phrases, or you can invoke them directly with slash commands:

```
/community-strategy
/community-launch
/member-onboarding
```

### Shared Context

Create `.claude/community-context.md` (using the **community-context** skill) to store your community's details. Every other skill reads this file first, so you don't repeat yourself.

## Skill Structure

Each skill follows a consistent format:

```
skills/skill-name/
├── SKILL.md          # Main skill definition
└── references/       # Optional detailed frameworks and examples
```

Every SKILL.md contains:
1. **YAML frontmatter** — name, version, description with trigger phrases
2. **Role definition** — expert persona
3. **Initial assessment** — context gathering (reads community-context first)
4. **Core frameworks** — domain-specific guidance
5. **Output format** — how to structure deliverables
6. **Task-specific questions** — what to ask when context is missing
7. **Related skills** — cross-references

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on adding or improving skills.

## License

MIT — see [LICENSE](LICENSE).
