# LLM Wiki Schema (Karpathy Pattern)

## Directory Structure
- `raw/`: Immutable source documents (clippings, transcripts, raw notes). I read from here but never modify.
- `wiki/`: The persistent knowledge base. I own this layer. It contains summaries, entity pages, and cross-references.
  - `wiki/Skills/`: Documentation for all active agents and workflows.
  - `wiki/Projects/`: Status and context for ongoing projects (e.g., Portfolio, Falko).
  - `wiki/Memory/`: Long-term memory, decisions, and user preferences.
- `index.md`: A catalog of everything in the `wiki/` folder with one-line summaries.
- `log.md`: An append-only record of our interactions (ingests, queries, updates).

## Workflows

### 1. Ingest (New Information)
When you provide a new source (URL, file, or long text):
1. I read the source from `raw/` or the chat.
2. I discuss key takeaways with you.
3. I create or update pages in `wiki/` to reflect this new knowledge.
4. I update `index.md` and append an entry to `log.md`.

### 2. Query (Asking Questions)
When you ask a question:
1. I consult `index.md` to find relevant wiki pages.
2. I read those pages and synthesize an answer.
3. If the answer is complex, I create a new page in `wiki/` to save the synthesis for later.

### 3. Lint (Maintenance)
Periodically, I will:
- Check `wiki/` for contradictions or stale info.
- Look for "orphan" pages (no inbound links).
- Suggest new sources to fill gaps in our knowledge.

## Conventions
- **Markdown:** All files are `.md`.
- **Links:** Use `[[Internal Links]]` for Obsidian compatibility.
- **Frontmatter:** Use YAML frontmatter for tags and dates where helpful.
- **Tone:** Professional, concise, and action-oriented.
