Email Ranking Engine: BM25 + Semantic Search (NLP)

This project demonstrates a hybrid ranking system for emails using both BM25 keyword matching and semantic similarity with sentence embeddings. Built with Python, pandas, scikit-learn, rank_bm25, and SentenceTransformers, it simulates a realistic email inbox and ranks messages based on a user query.

What It Does

Generates a mock inbox with 100 simulated emails across categories like Work, Promo, Newsletter, Social, and Updates.
Stores emails in a CSV format using pandas.
Combines traditional BM25 scoring (for keyword relevance) with semantic similarity (for contextual understanding) to rank emails.
Outputs the top emails most relevant to a natural language query, useful for intelligent inbox triage or automated email assistants.

Features

🔁 Simulated email data with realistic timestamps, labels, and actions (reply, archive, etc.)
🧠 BM25-based retrieval using rank_bm25 for fast keyword matching.
🤖 Semantic similarity using SentenceTransformers (all-MiniLM-L6-v2) for contextual ranking.
⚖️ Hybrid scoring mechanism with tunable weight (alpha) to balance BM25 vs. semantic relevance.
📈 Normalized ranking scores using MinMaxScaler for fair comparison across methods.
