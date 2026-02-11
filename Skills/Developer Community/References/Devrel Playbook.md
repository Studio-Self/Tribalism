---
date: 2026-02-07
created: 2026-02-07
tags:
  - references
  - devrel
  - playbook
---

# DevRel Playbook

Developer community templates, contributor guide structure, and DevRel program design.

---

## CONTRIBUTING.md Template (Open Source)

```markdown
# Contributing to [Project Name]

Thanks for your interest in contributing! This guide will help you get started.

## Getting Started

### Prerequisites
- [Language/runtime] version [X]+
- [Tool 1]
- [Tool 2]

### Development Setup
\```bash
# Clone the repo
git clone [repo-url]
cd [project]

# Install dependencies
[install command]

# Run the project locally
[run command]

# Run tests
[test command]
\```

### Verifying Your Setup
Run `[verification command]`. You should see:
\```
[Expected output]
\```

## Finding Issues to Work On

- 🟢 **good first issue** — Great for newcomers. Well-scoped, clear requirements.
- 🔵 **help wanted** — Needs community help. May require more context.
- 🟡 **feature request** — New functionality. Discuss in issue before starting.
- 🔴 **bug** — Something broken. Check if someone's already working on it.

Browse issues: [link to filtered issues]

## Making Changes

1. Fork the repo and create a branch: `git checkout -b feature/your-feature`
2. Make your changes
3. Write/update tests
4. Run the test suite: `[test command]`
5. Commit with a clear message: `git commit -m "feat: add [feature]"`
6. Push and open a pull request

### Commit Convention
We use [Conventional Commits](https://conventionalcommits.org/):
- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation
- `test:` Tests
- `refactor:` Code refactoring
- `chore:` Maintenance

### Pull Request Process
1. Fill out the PR template
2. Link the related issue
3. Ensure CI passes
4. Request review from maintainers
5. Address feedback
6. Maintainer merges when approved

**Response time:** We aim to review PRs within 48 hours.

## Code Style
[Style guide or linter configuration details]

## Getting Help
- 💬 [Discord/Slack channel]: [link]
- 📝 [Discussion forum]: [link]
- 📧 [Email]: [address]

## Recognition
All contributors are listed in [CONTRIBUTORS.md / release notes].
Regular contributors may be invited to become maintainers.

## Code of Conduct
This project follows our [Code of Conduct](CODE_OF_CONDUCT.md).
Please read it before contributing.
```

---

## Developer Content Templates

### Tutorial Structure
```
# How to [Accomplish Specific Task] with [Product/Tool]

## What You'll Build
[Screenshot or diagram of the end result]
[1-2 sentences describing what this tutorial produces]

## Prerequisites
- [Prerequisite 1]
- [Prerequisite 2]
- Estimated time: [X] minutes

## Step 1: [First Action]
[Explanation of what and why]

\```[language]
[Code block]
\```

[Explanation of what the code does]

## Step 2: [Second Action]
[Same structure]

## Step 3: [Third Action]
[Same structure]

## Testing Your Implementation
[How to verify it works]

## Next Steps
- [Link to related tutorial]
- [Link to advanced documentation]
- [Link to community for questions]

## Troubleshooting
| Problem | Solution |
|---------|---------|
| [Common error 1] | [Fix] |
| [Common error 2] | [Fix] |
```

### Architecture Deep Dive Structure
```
# How We Built [Feature/System]

## Context
[What problem we were solving and why it mattered]

## Options We Considered
| Option | Pros | Cons |
|--------|------|------|
| [Option A] | [Pros] | [Cons] |
| [Option B] | [Pros] | [Cons] |
| [Option C] | [Pros] | [Cons] |

## What We Chose (and Why)
[Decision and reasoning]

## Architecture
[Diagram or description of the system]

## Implementation
[Key code or configuration, with explanations]

## What We'd Do Differently
[Honest retrospective — this builds credibility]

## Performance Results
[Data, benchmarks, before/after]
```

---

## DevRel Metrics Dashboard

| Category | Metric | Target |
|----------|--------|--------|
| **Awareness** | GitHub stars/month | [X] |
| | Social mentions/month | [X] |
| | Blog post views/month | [X] |
| **Adoption** | New API signups/month | [X] |
| | Time to first API call | <[X] min |
| | Tutorial completion rate | >[X]% |
| **Engagement** | Monthly active developers (using API) | [X] |
| | Community DAU | [X] |
| | Questions answered (community) | [X]/month |
| | PRs from community/month | [X] |
| **Satisfaction** | Developer NPS | >[X] |
| | Documentation satisfaction | >[X]/5 |
| | Issue response time | <[X] hours |

---

## Developer Community Benchmarks

| Metric | Early Stage | Growing | Mature |
|--------|-----------|---------|--------|
| GitHub stars | <1K | 1K-10K | 10K+ |
| Monthly active contributors | <10 | 10-50 | 50+ |
| Community members (Discord/Slack) | <500 | 500-5K | 5K+ |
| Docs pages | <50 | 50-200 | 200+ |
| Time to first API call | >30 min | 10-30 min | <10 min |
| Issue response time | >72 hours | 24-72 hours | <24 hours |
| PR review time | >1 week | 2-5 days | <48 hours |
| Community-answered questions (% of total) | <20% | 20-50% | >50% |

**Named examples:**
- Stripe: Gold standard for developer docs. Time to first API call: ~5 minutes. Developer NPS consistently 60+.
- Vercel/Next.js: 100K+ GitHub stars. Community discussions answer 60%+ of questions.
- Supabase: 50K+ GitHub stars. Grew through developer-created content and hackathons.
- Tailwind CSS: Community-driven plugin ecosystem. 70K+ GitHub stars mostly through word-of-mouth.
