---
date: 2026-02-07
created: 2026-02-07
tags:
  - integrations
  - discourse
---

# Discourse Integration Guide

## Overview
Discourse is an open-source forum platform ideal for long-form discussion, knowledge bases, and technical communities. SEO-friendly by default with a trust level system that scales moderation naturally.

## Community Setup

### Categories
```
General
├── Introductions
├── Announcements

Topics
├── Category 1
├── Category 2

Support
├── Help & Questions
├── Bug Reports

Meta
├── Community Feedback
├── Site Feedback
```

### Trust Levels
Discourse has a built-in trust system (0-4) that automatically grants permissions based on participation:
- Level 0: New user (limited posting)
- Level 1: Basic (read enough, can post freely)
- Level 2: Member (regular participant, can invite)
- Level 3: Regular (trusted, can recategorize, close topics)
- Level 4: Leader (community moderator)

### Hosting Options
- Self-hosted: Free, requires server management
- Discourse Cloud: $50-300+/month depending on scale

## Best Practices
- Let the trust level system do the heavy lifting for moderation
- Use tags in addition to categories for cross-cutting topics
- Enable solved plugin for Q&A-style support
- Make key content wiki posts that multiple members can edit
- Use the API for integrations with your product
