# Content Creator Skill

## Workflow
1. User sends a topic, voice note, or a list of topics.
2. For single topics:
   - Generate `<slug>.pl.md` and `<slug>.en.md` based on `portfolio/blog/_template.*.md`.
   - 3 LinkedIn post versions.
   - Prompt for an image.
3. For bulk topics (Batch API - 50% cheaper):
   - Prepare `batch_requests.jsonl`.
   - Run `python3 gemini_batch_worker.py create batch_requests.jsonl`.
   - Poll with `python3 gemini_batch_worker.py check <job_id>`.
   - Process results once finished.
4. User approves.
5. I:
   - Commit/Push MD files to `portfolio/blog/`.
   - Generate image via API (NanoBanana).
   - Post to LinkedIn via Playwright.

## Style Guidelines
- **Target:** Clients (results-oriented, business value).
- **Tone:** Professional yet loose, technical authority but no "secret sauce" leaks.
- **SEO:** Always fill `seoTitle` and `seoDescription`.
- **Translations:** `slug` and `translationKey` must match between PL and EN files.
- **Assets:** Always use `/blog/<slug>/cover.webp` for cover images.
