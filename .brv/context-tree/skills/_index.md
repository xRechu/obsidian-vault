---
children_hash: 3ec2517d9e5b69a6f441601faa97b1c6d60ffa47ec1552f9e89f3b8a4d2950a3
compression_ratio: 0.7535545023696683
condensation_order: 2
covers: [content_creator/_index.md]
covers_token_total: 211
summary_level: d2
token_count: 159
type: summary
---
### Content Creator Skill (d2 Summary)

**Core Function:** Automates multi-language content generation and LinkedIn distribution.

**Workflow Path:**
Input → Gemini Batch API (50% cost reduction) → Approval → GitHub Commit → NanoBanana Image Gen → Playwright LinkedIn Post.

**Technical Stack & Files:**
- **Stack:** Next.js, Medusa.js.
- **Key Assets:** `SKILL_CONTENT_CREATOR.md`, `gemini_batch_worker.py`.

**Mandatory Conventions:**
- SEO metadata (title/description) required.
- Slug/translationKey alignment enforced.
- Image Path: `/blog/<slug>/cover.webp`.

**Integrations:** Gemini Batch API, NanoBanana, Playwright, GitHub API.