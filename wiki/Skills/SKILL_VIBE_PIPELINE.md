# Skill: Vibe Pipeline Creator (Falko Edition)

## Core Framework: Content Engine 2.0 (Inspired by "Eddie")
1. **Strategic Research Protocol (SRP) & Ad-Mining:**
   - **Competitor Scraping:** Use Playwright/Apify to mine Meta/TikTok Ad Library for a niche or specific competitor.
   - **Profitability Sort:** Identify oldest active ads (likely most profitable).
   - **Intelligence Extraction:** Transcribe top ads (Whisper) and break down hooks/angles.
   - **Storage:** Log full intel dump in `/research/<project>/competitors/`.
2. **Brand Brain (The Three Pillars):**
   - **VOICE.md:** Define tone based on existing content (Falko's "Made in Garage" + Manga vibe).
   - **PRODUCT.md:** Technical specs, USP, and "secret sauce".
   - **ICP.md:** Who actually buys? (Anime fans, streetwear collectors, etc.).
   - **WRITING_RULES.md:** The Anti-AI Filter (banning "AI slop" words/patterns).
3. **Strategic Vibe Matrix (The Multiplier):** 
   - Generate 50-100 script variations via Gemini Batch.
   - **The Rewrite Loop:** Original competitor script -> Angle extraction -> Our Voice/Product rewrite.
   - Multiply by different ICPs.
4. **Approval & Routing:**
   - User selects winners.
   - Route to **UGC Creators** (Top 10%) or **AI Generation** (Remaining 90%).
5. **Multi-Model Production:**
   - **NanoBanana:** Static UGC, character consistency, lifestyle lookbooks.
   - **Replicate/Fal.ai:** Dynamic video (Kling/Luma), multiple "actors" per script.
6. **Performance Feedback Loop (EVALUATE & REGENERATE):**
   - **Data Ingestion:** User provides performance metrics (CPA, ROAS, Retention) via MMP (e.g., Singular API) or manual report.
   - **Winning Direction:** OpenClaw analyzes which creative angles and actors outperformed others.
   - **Brain Update:** Winning patterns are added to a "Winning Archive" to bias future generations toward success.

## 🔄 Maintenance & Evolution
- **Bi-Weekly Audit:** Review `/research/competitors/` to catch new market shifts.
- **Rules Refinement:** Periodically update `WRITING_RULES.md` as AI models evolve to ensure 0% slop.
- **Prompt Engineering:** Optimize Replicate/Fal.ai prompts based on rendered output quality.
- **Framework Updates:** This skill file is a living document; update it after every successful "Chapter" to reflect learned efficiencies.

## Operational Workflow
- **Input:** "Wrzucam fotki nowej bluzy z Rozdziału 2."
- **Process:** OpenClaw executes Step 1 & 3 autonomously -> Returns Matrix.
- **Output:** Approved assets generated and delivered to `/output/falko-project/`.
