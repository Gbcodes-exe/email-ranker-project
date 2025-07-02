# Email Ranking Engine: BM25 + Semantic Search

This project simulates an email inbox and ranks emails based on a user query using a hybrid approach: combining BM25 keyword relevance and semantic similarity from sentence embeddings.

Built using Python, this project showcases practical applications of NLP in intelligent search and information retrieval systems.

---

## Features

- Generates a mock inbox with 100 realistic emails
- Combines BM25 scoring with semantic similarity using Sentence Transformers
- Normalizes scores and ranks emails based on user queries
- Prints top-N most relevant emails for any given search term

---

## Technologies Used

- Python 3
- pandas, numpy
- scikit-learn
- rank_bm25
- sentence-transformers (all-MiniLM-L6-v2)

---

## File Overview

```bash
EmailRanking/
├── EmailRankerProject.ipynb   # Jupyter Notebook with full implementation
├── mock_emails.csv            # Simulated inbox data
├── requirements.txt           # Required Python packages
└── README.md                  # Project documentation

Setup Instructions

Clone the repository:
git clone https://github.com/your-username/EmailRanking.git
cd EmailRanking

Create a virtual environment (optional but recommended):
python -m venv env
source env/bin/activate   # or .\env\Scripts\activate on Windows
Install dependencies:
pip install -r requirements.txt

Run the notebook:
jupyter notebook notebook.ipynb

Example Usage
query = "project update"
hybrid_rank(query)

Output:

Top 10 Emails for Query: 'project update'

[Score: 0.984] : Project update | From: alice@company.com | Label: opened
[Score: 0.821] : Urgent deadline | From: bob@company.com | Label: starred
...


Future Work

Integrate with a real email client (e.g., Gmail API)
Deploy as a web app using Flask or Streamlit
Learn user preferences over time to personalize results

