---
date: 2026-02-07
created: 2026-02-07
tags:
  - feedback
  - team-community
  - references
  - ops
  - templates
---

# Operations Templates

Hiring scorecards, automation recipes, daily/weekly checklists, and team structure templates.

---

## Community Manager Job Description

```
## [Community Manager / Senior Community Manager] — [Company Name]

### About the Role

We're looking for a [Community Manager] to build and grow [community
name / our community]. You'll own the member experience from onboarding
to advocacy, design engagement programs, and connect community insights
to business outcomes.

### What You'll Do

- Own the day-to-day community experience ([platform])
- Design and run engagement programs (discussions, events, challenges)
- Onboard new members and ensure first-week activation
- Recruit, train, and manage volunteer moderators and ambassadors
- Track community metrics and report on health and business impact
- Create and distribute community content (newsletter, recaps, spotlights)
- Collaborate with [product/marketing/support] to close the feedback loop
- Build relationships with key members and emerging leaders

### What You Bring

**Must-haves:**
- [X]+ years of community management experience
- Exceptional written communication
- Empathy, patience, and genuine care for people
- Experience with [platform] or similar community platforms
- Self-starter who can work independently
- Comfort with ambiguity and building from scratch

**Nice-to-haves:**
- Experience with [industry/topic]
- Data literacy (can pull and interpret metrics)
- Content creation skills (writing, video, design)
- Event planning experience
- Experience with community analytics tools (Common Room, Orbit)

### Compensation

- Salary: $[X]-$[Y]
- [Benefits, equity, perks]
- [Remote/hybrid/onsite]
```

## Hiring Scorecard

| Criteria | Weight | Score (1-5) | Notes |
|----------|--------|------------|-------|
| Communication skills (writing sample) | 25% | | |
| Community experience (relevant examples) | 20% | | |
| Empathy and member-first mindset | 20% | | |
| Strategic thinking (can connect community to business) | 15% | | |
| Technical skills (platforms, tools, analytics) | 10% | | |
| Culture fit and values alignment | 10% | | |
| **Total (weighted)** | | | |

**Strong hire:** 4.0+
**Proceed with caution:** 3.0-3.9
**Pass:** <3.0

---

## Automation Recipes (Zapier/Make)

### Recipe 1: New Member → Email List + CRM
```
Trigger: New member joins [community platform]
Action 1: Add to email list ([tool]) with tag "community_member"
Action 2: Create/update contact in CRM with community_member = true
Action 3: Set community_join_date = today
```

### Recipe 2: New Member → Welcome DM (Delayed)
```
Trigger: New member joins [community platform]
Delay: 24 hours
Filter: IF member has NOT posted in any channel
Action: Send DM with check-in message template
```

### Recipe 3: Weekly Discussion Auto-Post
```
Trigger: Schedule — Every [Monday] at [9:00 AM]
Action: Post message in #[channel]
Content: [Pull from a list of pre-written prompts, rotating weekly]
```

### Recipe 4: Inactive Member Alert
```
Trigger: Schedule — Every Monday
Action: Query community platform for members inactive 14+ days
Filter: Only members who were active in the previous 30 days
Action: Send list to community team Slack channel
```

### Recipe 5: Event Follow-Up
```
Trigger: Event ends on [Luma/Zoom]
Delay: 2 hours
Action 1: Send thank-you email to attendees
Action 2: Send recording + recap to registered no-shows
Action 3: Send community invite to non-member attendees
```

### Recipe 6: Feedback to Product Team
```
Trigger: New post in #feedback channel
Action 1: Create item in [Canny/Linear/Notion] feedback board
Action 2: Notify product channel in internal Slack
Action 3: React to original post with ✅ (acknowledged)
```

### Recipe 7: Weekly Metrics Compilation
```
Trigger: Schedule — Every Monday at 8:00 AM
Action 1: Pull community metrics from platform API
Action 2: Update Google Sheet with weekly numbers
Action 3: Post weekly pulse summary in #team-community Slack channel
```

---

## Daily Operations Checklist

```
## Daily Community Ops — [Date]

### Morning (30 min)
- [ ] Check moderation queue — resolve any flagged content
- [ ] Respond to new member introductions (within 4 hours)
- [ ] Review overnight discussions — react, reply, or pin as needed
- [ ] Check #feedback for new suggestions

### Midday (15 min)
- [ ] Post or prompt one piece of content (discussion, resource, poll)
- [ ] Check in on any ongoing programs (challenge updates, AMA prep)
- [ ] Respond to DMs from members

### End of Day (15 min)
- [ ] Quick scan of all channels for unresolved questions
- [ ] Note any emerging issues or trends for weekly review
- [ ] Update moderation log if any actions taken
```

## Weekly Operations Checklist

```
## Weekly Community Ops — Week of [Date]

### Monday
- [ ] Run weekly engagement program (post discussion thread)
- [ ] Review last week's metrics
- [ ] Check automation workflows are running

### Tuesday-Thursday
- [ ] Daily ops checklist
- [ ] Prep for weekly event (if applicable)
- [ ] Check in with ambassadors/moderators

### Friday
- [ ] Compile weekly pulse report
- [ ] Send weekly digest/newsletter
- [ ] Plan next week's content and events
- [ ] Update community calendar

### Monthly (first week)
- [ ] Monthly report for stakeholders
- [ ] Ambassador check-in meeting
- [ ] Community guidelines review
- [ ] Platform and tool audit
- [ ] Member feedback collection
```

---

## Team Communication Templates

### Weekly Team Update (Async)
```
## Community Team Update — Week of [Date]

### Key Metrics
- Active members: [X] ([+/-X] vs last week)
- New joins: [X]
- Posts/messages: [X]
- Events: [X] (attendance: [X])

### Wins
- [Win 1]
- [Win 2]

### Issues
- [Issue requiring attention]

### Help Needed
- [Request for other teams]

### Next Week
- [Priority 1]
- [Priority 2]
```

---

## Community Manager Time Allocation Benchmarks

### Solo CM (< 1K members)
| Activity | Hours/Week | % |
|----------|-----------|---|
| Daily engagement (responding, moderating, connecting) | 12-15 | 40% |
| Programming (events, content, challenges) | 6-8 | 20% |
| Growth (outreach, content repurposing, partnerships) | 4-5 | 15% |
| Ops (tools, reporting, automation) | 4-5 | 15% |
| Strategy (planning, stakeholder management) | 3-4 | 10% |

### With Team (1K-10K members)
| Activity | CM Lead | CM | Events/Content |
|----------|---------|-----|---------------|
| Strategy | 40% | 10% | 5% |
| Daily engagement | 15% | 40% | 20% |
| Programming | 15% | 20% | 50% |
| Growth | 15% | 15% | 15% |
| Ops and reporting | 15% | 15% | 10% |
