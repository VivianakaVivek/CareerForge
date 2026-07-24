# CareerForge 🎯 — AI-Powered Career War Room

<div align="center">

[![Live App](https://img.shields.io/badge/🌐_Live_App-CareerForge-8B5E3C?style=for-the-badge)](https://careerforge-nfxvxqh8sa4kdmeh9nfcvu.streamlit.app)
[![Built with Streamlit](https://img.shields.io/badge/Built_with-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io)
[![Powered by Gemini](https://img.shields.io/badge/Powered_by-Gemini_AI-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://ai.google.dev)
[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)

**🌍 Try it live → [https://careerforge-nfxvxqh8sa4kdmeh9nfcvu.streamlit.app](https://careerforge-nfxvxqh8sa4kdmeh9nfcvu.streamlit.app)**

</div>

---

## 📌 What is CareerForge?

**CareerForge** is an AI-powered, agentic career readiness platform that bridges the gap between your resume and the actual hiring bar of top-tier companies. Powered by **Google Gemini** (or Groq/OpenAI), CareerForge intelligently analyzes your full profile, scores your readiness across 5 critical dimensions, builds a personalized week-by-week preparation roadmap, and provides an always-on AI Career Coach — all in one place.

> Built for students and early-career professionals preparing for placement season at companies like Bain, Google, Goldman Sachs, Zomato, and more.

---

## ✨ Features

### 📄 Intelligent Resume Parsing
Upload your PDF resume and let the AI do the heavy lifting. CareerForge extracts your complete story — technical skills, soft skills, CGPA, leadership positions, projects, internships, awards, and extracurriculars — not just keywords.

### 🏢 Target Companies & Roles
Select from a curated list of top MNCs (Bain, McKinsey, Google, Zomato, Goldman Sachs, etc.) or type in any custom company or role. The AI calibrates its entire analysis to match that specific hiring bar.

### 📊 5-Axis Readiness Scorecard
Your profile is evaluated holistically and scored (0–100) across five real hiring dimensions:
| Axis | What it Measures |
|---|---|
| 🔧 Technical Depth | Coding, tools, frameworks, projects |
| 🏅 Leadership & Initiative | Clubs, positions of responsibility, social impact |
| 🗣️ Communication & Presentation | Writing, storytelling, articulation |
| 💼 Business Acumen | Strategy, market thinking, domain knowledge |
| 🎯 Role Fit | Overall match to the specific role & company |

### 🗺️ Interactive Preparation Roadmap
Based on your chosen timeline (1 Week → 6 Months), CareerForge generates a structured, phase-by-phase flowchart with specific tasks and curated course recommendations grounded in real data via RAG.

### 🤖 Always-On Career Coach
Chat directly with an AI coach that remembers your entire profile, your target companies, and your gaps. Use it to:
- Run mock case interviews (consulting)
- Practice STAR behavioral stories
- Get skill gap action plans
- Ask any career question, anytime

---

## 🛠️ Tech Stack

| Technology | Role |
|---|---|
| **Python 3.9+** | Core language |
| **Streamlit** | Frontend UI framework |
| **Google Gemini / Groq / OpenAI** | LLM inference engine |
| **RAG (Retrieval-Augmented Generation)** | Grounding AI in real job & course data |
| **Pandas** | Dataset processing |
| **PyPDF** | Resume text extraction |

---

## 🚀 How to Run Locally

### 1. Clone the repository
```bash
git clone https://github.com/VivianakaVivek/CareerForge.git
cd CareerForge
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Set up your API Key
Create a `.env` file in the project root:
```bash
GEMINI_API_KEY="your_api_key_here"
```
> Get a free key at [aistudio.google.com/apikey](https://aistudio.google.com/apikey)

### 4. Run the app
```bash
streamlit run app.py
```
The app opens automatically at `http://localhost:8501`

---

## 🔑 Supported API Keys

| Provider | Key Format | Model Used |
|---|---|---|
| **Google Gemini** (default) | `AIza...` | gemini-2.0-flash |
| **Groq** (recommended for free tier) | `gsk_...` | llama-3.3-70b-versatile |
| **OpenAI** | `sk-...` | gpt-4o-mini |

The app **auto-detects** which provider to use based on your key prefix — no configuration needed!

---

## 📁 Project Structure

```
CareerForge/
├── app.py                  # Main Streamlit application
├── agent_optimizer.py      # 4 AI agents (extract, score, roadmap, coach)
├── resume_parser.py        # PDF text extraction
├── requirements.txt        # Python dependencies
├── .env.example            # API key template
└── data/
    ├── courses.csv         # RAG dataset: online course recommendations
    └── job_postings.csv    # RAG dataset: real job posting context
```

---

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to open an issue or submit a pull request.

---

<div align="center">

**CareerForge** · Built for placement season · Made with ❤️ by Vivek

[![GitHub](https://img.shields.io/badge/GitHub-VivianakaVivek-181717?style=flat&logo=github)](https://github.com/VivianakaVivek)

</div>
