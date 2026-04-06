---
title: Content Creator Skill
tags: []
keywords: []
importance: 55
recency: 1
maturity: draft
updateCount: 1
createdAt: '2026-03-10T18:31:41.976Z'
updatedAt: '2026-03-10T18:39:55.729Z'
---
## Raw Concept
**Task:**
Automate content creation and LinkedIn posting

**Files:**
- SKILL_CONTENT_CREATOR.md
- gemini_batch_worker.py

**Flow:**
User input -> Generate MD (PL/EN) -> Batch API for bulk -> User approval -> Commit/Push -> NanoBanana Image Gen -> LinkedIn Post via Playwright

**Timestamp:** 2026-03-10

## Narrative
### Structure
Workflow for single and bulk topics using Next.js/Medusa.js stack.

### Dependencies
Gemini Batch API, NanoBanana API, LinkedIn (Playwright), GitHub API.

### Highlights
Batch API reduces costs by 50%. Automated LinkedIn posting.

### Rules
Always fill seoTitle/seoDescription. Slug/translationKey must align. Cover images at /blog/<slug>/cover.webp.

## Facts
- **batch_api_savings**: Batch API saves 50% on Gemini-2.0-flash costs [project]
- **image_path_convention**: Cover images must be located at /blog/<slug>/cover.webp [convention]
