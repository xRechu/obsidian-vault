# Activity Log

## [2026-04-06] Lint | LLM Wiki Initialization
- **Action:** Restructured the vault according to the Karpathy Pattern.
- **Changes:**
  - Created `raw/` and `wiki/` directories.
  - Moved existing Skills (`CONTENT_CREATOR`, `VIBE_PIPELINE`, `META_AUTONOMOUS_AGENT`) to `wiki/Skills/`.
  - Moved `MEMORY.md` to `wiki/Memory/`.
  - Created `SCHEMA.md` as the guiding document for the agent.
  - Generated initial `index.md` and `log.md`.
- **Status:** System ready for ingestion and compounding knowledge.

## [2026-04-11] Update | Portfolio Additions
- **Action:** Added `paraboo.pl` to the `Realizations` section of `jakubreszka.pl` portfolio.
- **Details:** 
  - Extracted details from the live `https://paraboo.pl` website (an Asian restaurant in Bydgoszcz with Ristorio ordering system).
  - Wrote PL and EN descriptions matching the portfolio style.
  - Pushed changes directly to the portfolio GitHub repository.

## [2026-04-11] Fix | Blog Layout
- **Action:** Fixed footer behavior on short blog pages.
- **Details:** 
  - Added `min-height: 100vh`, `display: flex`, and `flex-direction: column` to `.blogPage` in `blog.module.css`.
  - Added `flex-grow: 1` to `.blogInner` to push the footer to the bottom of the screen when content is short, preventing the empty space below from making the footer look oversized.

## [2026-04-13] Fix | Dynamic Latest Post Link
- **Action:** Fixed the "Najnowszy wpis" (Latest post) button on the portfolio homepage to dynamically point to the newest blog post instead of a hardcoded article.
- **Details:** 
  - Updated `HomePage.tsx` to accept `latestPostHrefPl` and `latestPostHrefEn` as props.
  - Updated the server components `app/page.tsx` and `app/en/page.tsx` to fetch the latest post via `getAllBlogPosts` and pass the dynamically generated URL to `HomePage`.
