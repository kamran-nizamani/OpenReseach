# OpenResearch

**OpenResearch** is an AI-native research workspace for discovering papers, reading evidence, comparing studies, and maintaining a research trail.

## What is included
- 🔎 Research discovery with relevance scoring
- 📚 Personal paper library
- 📖 Focused paper reader with an AI research brief
- 🧠 Structured research signals: problem, approach, open question
- 🔗 Evidence-map concept for claims and relationships
- ⚖️ Side-by-side paper comparison
- 📝 Persistent in-session research notes
- 📱 Responsive dark research UI

## Run locally

```bash
npm install
npm run dev
```

Then open the Vite URL shown in the terminal.

## Architecture

The current version is a frontend-first foundation. Paper data is isolated in `src/main.jsx` so it can be replaced with live providers later.

Recommended production integrations:
- Semantic Scholar / OpenAlex for paper metadata
- arXiv for preprints
- Supabase/Postgres for accounts, libraries and notes
- pgvector for semantic search
- An LLM gateway for summaries, evidence extraction and research questions
- DOI/Crossref metadata for citation normalization

## Product direction

OpenResearch should evolve from a paper browser into a **research operating system**: every paper, claim, note, citation and research question becomes a connected evidence object with provenance.

> Important: AI-generated summaries should always expose their source paper and should not be treated as primary evidence without verification.
