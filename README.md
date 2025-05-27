# 🧠 QuerySensei

QuerySensei is your personal data analysis assistant, powered by AI.  
Upload a CSV file or connect to BigQuery, ask questions in natural language, and get smart, visual, and actionable answers.

---

## ✨ Features

- 🔍 Ask questions in plain English (or other languages) about your data
- 📊 Get instant answers as:
  - Text summaries
  - SQL queries
  - Charts and graphs
  - Machine Learning insights (e.g. forecasting, clustering)
- 🧠 Powered by Vertex AI LLM and Python
- 🚀 Deployable to GCP (Cloud Run + Docker)
- 🗃️ Works with local CSVs and (soon) BigQuery / CloudSQL

---

## 🛠️ Tech Stack

| Layer | Tech |
|-------|------|
| Interface | Streamlit |
| AI | Vertex AI LLM (Gemini/PaLM) |
| Data | Pandas (CSV), BigQuery (later CloudSQL) |
| ML | Scikit-learn, Prophet, matplotlib |
| DevOps | Docker, Cloud Run |
| Utils | Google Cloud SDK, Python dotenv |

---

## 🚀 Quick Start

```bash
git clone https://github.com/yourusername/querysensei.git
cd querysensei
pip install -r requirements.txt
streamlit run app/main.py
