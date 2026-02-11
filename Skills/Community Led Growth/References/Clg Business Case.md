---
date: 2026-02-07
created: 2026-02-07
tags:
  - references
  - clg
  - business
  - case
---

# CLG Business Case Template

Templates for building a business case for community investment and measuring CLG impact.

---

## Business Case Template

```
# Community Investment Business Case

## Executive Summary
[2-3 sentences: We propose investing [amount] in community to drive
[specific business outcomes]. Based on [Data/benchmarks], we project
[ROI/impact] within [timeline].]

## The Opportunity
- [X]% of our customers who engage in community have [Y]% higher retention
  (or: industry benchmarks show community members retain 15-30% better)
- Community-answered questions cost $2-5 vs. $15-25 per support ticket
- Community members expand at [X]% higher rate than non-members
- Top competitors [name 1, name 2] have invested in community and are seeing [results]

## Investment Required

| Item | Monthly Cost | Annual Cost |
|------|-------------|-------------|
| Community Manager (1 FTE) | $[X] | $[X] |
| Platform costs | $[X] | $[X] |
| Tools (analytics, automation) | $[X] | $[X] |
| Events and programs | $[X] | $[X] |
| Ambassador program perks | $[X] | $[X] |
| **Total** | **$[X]** | **$[X]** |

## Projected Returns (12-Month)

| Value Driver | Calculation | Annual Value |
|-------------|------------|-------------|
| Support deflection | [X] tickets/mo × $20/ticket × 12 | $[X] |
| Retention lift | [X] customers × [Y]% lift × $[Z] ARPU | $[X] |
| Acquisition influence | [X] community-sourced signups × $[Z] ACV | $[X] |
| Content value | [X] community posts × $[Y] equivalent cost | $[X] |
| **Total projected value** | | **$[X]** |

## ROI Projection
- Year 1 ROI: [X]%
- Break-even: Month [X]
- 3-year NPV: $[X]

## Risks and Mitigations
| Risk | Probability | Mitigation |
|------|------------|-----------|
| Low adoption | Medium | Phased launch, founding member approach |
| Can't prove attribution | Medium | Instrument before launch, cohort tracking |
| Community team turnover | Low | Document processes, cross-train |

## Success Metrics (First 6 Months)
1. [X] active community members
2. [X] support tickets deflected per month
3. [X]% activation rate for new members
4. Community members show [X]% higher retention
5. [X] product feedback items surfaced

## Ask
Approve $[X] annual investment in community with [X]-month checkpoint.
```

---

## CLG Attribution Setup Guide

### Step 1: Tag Community Members in CRM

Create a field in your CRM (HubSpot, Salesforce, etc.):
- Field name: `community_member`
- Type: Boolean (Yes/No)
- Populated by: Community platform webhook, Zapier, or manual

Also track:
- `community_join_date`
- `community_engagement_level` (low/medium/high)
- `community_source` (how they found the community)

### Step 2: Create Comparison Cohorts

| Cohort | Definition | What You'll Compare |
|--------|-----------|-------------------|
| Community members | community_member = Yes | All metrics below |
| Non-community customers | community_member = No, is customer | Same metrics |
| Community → Customer | Joined community before becoming customer | Attribution |
| Customer → Community | Became customer before joining community | Retention lift |

### Step 3: Metrics to Track Per Cohort

| Metric | Community Members | Non-Community | Delta |
|--------|------------------|--------------|-------|
| 30-day retention | | | |
| 90-day retention | | | |
| Annual retention | | | |
| NPS score | | | |
| Support tickets per user | | | |
| Feature adoption rate | | | |
| Expansion rate (upsell) | | | |
| LTV | | | |
| Referral rate | | | |

### Step 4: Track Community-Influenced Pipeline

For sales-assisted deals:
- Did the prospect engage in the community before the deal?
- Did a community member make a referral or introduction?
- Did the prospect cite community content in the sales process?

Tag opportunities in CRM:
- `community_influenced` = Yes/No
- `community_sourced` = Yes/No (community was the original acquisition source)

---

## CLG Dashboard Template

### Overview Metrics
```
┌─────────────────────────────────────────────┐
│ COMMUNITY-LED GROWTH DASHBOARD              │
├─────────────┬───────────┬───────────────────┤
│ Active      │ Community │ Community         │
│ Members     │ Revenue   │ ROI               │
│ [X]         │ $[X]      │ [X]%              │
│ ↑[X]% MoM  │ ↑[X]% MoM│                   │
├─────────────┴───────────┴───────────────────┤
│                                             │
│ RETENTION LIFT                              │
│ Community: [X]%  |  Non-community: [X]%     │
│ Delta: +[X]%                                │
│                                             │
│ SUPPORT DEFLECTION                          │
│ Tickets deflected: [X]/month                │
│ Savings: $[X]/month                         │
│                                             │
│ ACQUISITION                                 │
│ Community-sourced signups: [X]              │
│ Community-influenced pipeline: $[X]         │
│                                             │
│ ENGAGEMENT                                  │
│ DAU/MAU: [X]% | Posts/week: [X]             │
│ Active contributors: [X]                    │
│                                             │
└─────────────────────────────────────────────┘
```

---

## Named CLG Examples

**Figma:** Community-created templates became the primary discovery channel. Users find templates → try Figma → become users. Community drove virality without traditional marketing spend.

**Notion:** Community-driven template gallery and YouTube ecosystem created by power users. The community IS the marketing engine — user-generated content ranks for thousands of keywords.

**HubSpot:** Community forums answer 40%+ of support questions. Community members have 25% higher NPS and 30% higher expansion rate.

**Atlassian:** Atlassian Community answers 60%+ of support questions, saving millions in support costs. Community answers are often faster and more detailed than official support.

**Salesforce Trailblazer Community:** 3M+ members. Community-certified "Rangers" and "MVPs" drive product adoption, provide peer support, and create content that Salesforce couldn't produce internally at scale.

**MongoDB:** Developer community answers 40% of support volume. Community-sourced documentation and tutorials rank in search, driving organic acquisition.
