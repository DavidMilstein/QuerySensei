# 🧠 QuerySensei

QuerySensei is your personal data analysis assistant, powered by AI.  
Upload a CSV file or connect to BigQuery, ask questions in natural language, and get smart, visual, and actionable answers.

---

## 🚧 Development Status

QuerySensei is currently in early development (MVP stage).

⚠️  *QuerySensei is actively under development. Features, structure, and priorities may shift as the project grows.*

The goal is to build a smart, production-ready AI assistant for exploring data using natural language.  
Core functionality is being implemented first, including:

- Uploading CSV files  
- Interpreting natural language questions with Vertex AI  
- Running data analysis and visualizations with Python  

As the project progresses, features may be added, removed, or changed based on insights and technical constraints.

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

bash
git clone https://github.com/yourusername/querysensei.git
cd querysensei
pip install -r requirements.txt
streamlit run app/main.py

---

## 🧠 Sample Prompt

> "Analyze sales.csv and predict the revenue for next month."  
> "Which products have the most complaints?"  
> "Is there a correlation between customer age and purchase amount?"

Try asking:

- What’s the average purchase per customer segment?
- Show me a bar chart of revenue by region.
- Cluster the customers based on behavior.

---

```text
## 📂 Folder Structure

querysensei/
├── app/
│   ├── main.py               # Streamlit entry point
│   ├── ui.py                 # UI components
│   ├── llm_interface.py      # Vertex AI integration
│   ├── query_builder.py      # Translate NL to SQL or logic
│   └── model_handler.py      # ML models (forecasting, clustering)
│
├── data/
│   ├── sample_sales.csv
│   └── sample_customers.csv
│
├── notebooks/
│   ├── ml_experiments.ipynb
│   └── query_testing.ipynb
│
├── utils/
│   ├── config.py
│   └── logger.py
│
├── .env.example              # Template for environment variables
├── requirements.txt
├── Dockerfile
├── README.md
└── .gitignore
```
---

## 🔐 Environment Variables

You'll need to set the following environment variables:

- `GOOGLE_PROJECT_ID`: Your GCP project ID
- `GOOGLE_APPLICATION_CREDENTIALS`: Path to your service account JSON key
- `VERTEX_MODEL_ID`: The specific model you'd like to use (e.g., gemini-pro)

Create a `.env` file based on `.env.example`.

---

## 📌 Roadmap

*Note: This roadmap is tentative and subject to change as the project evolves.*

- [ ] Add support for BigQuery data sources
- [ ] Add CloudSQL integration to store user queries/statistics
- [ ] Add authentication (email-based or Google OAuth)
- [ ] Support Excel (.xlsx) uploads
- [ ] Multilingual support
- [ ] Scheduled insights (email summaries)
- [ ] Deploy public demo to querysensei.com

---

## 🤝 Contributing

Feel free to fork, star, or submit issues and pull requests.

If you have suggestions, ideas, or improvements, contributions are always welcome!

---

## 🧑‍💻 Author

Made by David Milstein 
Powered by [Google Cloud](https://cloud.google.com/) and ❤️

---

## 🌐 Domain

This project is proudly hosted at:  
**[https://www.querysensei.com](https://www.querysensei.com)**
