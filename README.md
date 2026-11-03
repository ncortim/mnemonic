# Mnemo

A local-first retrieval-augmented generation (RAG) service for personal notes and
journal entries. Ask questions like "What did I decide about moving to Berlin?" or
"How has my sleep been over the last month?" and get answers grounded in your own
writing, with citations to the specific entries and dates they came from. If your
notes don't contain the answer, Mnemo says so instead of guessing.

**Stack:** Python 3.11 · uv · FastAPI · ChromaDB · multilingual-e5 embeddings ·
Ollama / Claude API (swappable) · Docker · GitLab CI/CD

**Design goals**
- Privacy-first: embeddings run locally, and a fully offline mode is supported
- Markdown-aware chunking with date metadata for time-based questions
- Retrieval quality measured on a custom evaluation set
- Demo runs on synthetic data, so no personal content is ever in the repo
