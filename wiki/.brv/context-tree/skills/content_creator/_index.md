---
children_hash: d2679533d1cb62d59f65b095ab5a923bbcda126e3a90bf813ce5dfa5399605ed
compression_ratio: 0.5444444444444444
condensation_order: 1
covers: [content_creator_skill.md]
covers_token_total: 270
summary_level: d1
token_count: 147
type: summary
---
### Content Creator Skill
Automates multi-language content generation and LinkedIn distribution.

**Workflow:**
Input -> Gemini Batch API (50% cost reduction) -> Approval -> GitHub Commit -> NanoBanana Image Gen -> Playwright LinkedIn Post.

**Key Components:**
- **Stack:** Next.js, Medusa.js.
- **Critical Files:** `SKILL_CONTENT_CREATOR.md`, `gemini_batch_worker.py`.
- **Conventions:**
  - SEO fields (title/description) required.
  - Slug/translationKey alignment mandatory.
  - Path: `/blog/<slug>/cover.webp`.

**Dependencies:** Gemini Batch API, NanoBanana, Playwright, GitHub API.