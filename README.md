<div align="center">

<br/>

```
███╗   ██╗███████╗██╗    ██╗███████╗    ███████╗██████╗ ██╗  ██╗███████╗██████╗ ███████╗
████╗  ██║██╔════╝██║    ██║██╔════╝    ██╔════╝██╔══██╗██║  ██║██╔════╝██╔══██╗██╔════╝
██╔██╗ ██║█████╗  ██║ █╗ ██║███████╗    ███████╗██████╔╝███████║█████╗  ██████╔╝█████╗  
██║╚██╗██║██╔══╝  ██║███╗██║╚════██║    ╚════██║██╔═══╝ ██╔══██║██╔══╝  ██╔══██╗██╔══╝  
██║ ╚████║███████╗╚███╔███╔╝███████║    ███████║██║     ██║  ██║███████╗██║  ██║███████╗
╚═╝  ╚═══╝╚══════╝ ╚══╝╚══╝ ╚══════╝    ╚══════╝╚═╝     ╚═╝  ╚═╝╚══════╝╚═╝  ╚═╝╚══════╝
```

# 🌍 AI Smart News Sphere

**A dual-mode intelligent news aggregator powered by NLP, Machine Learning & Generative AI.**

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![HTML5](https://img.shields.io/badge/HTML5-Web%20Dashboard-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-Styled-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com)
[![Gemini](https://img.shields.io/badge/Google%20Gemini-Pro-8E24AA?style=for-the-badge&logo=google&logoColor=white)](https://ai.google.dev)
[![License](https://img.shields.io/badge/License-MIT-22C55E?style=for-the-badge)](LICENSE)

<br/>

> *Don't just read the news — understand it.*

<br/>

</div>

---

## ✨ What is AI Smart News Sphere?

**AI Smart News Sphere** is a dual-mode intelligent news aggregator that goes beyond simple headlines. It combines advanced **Natural Language Processing (NLP)** with **Generative AI** to cluster, analyze, and surface deep insights from news stories — so you don't just know *what* happened, you understand *why* it matters.

The project ships in two distinct but complementary forms:

| Mode | Component | Purpose |
|------|-----------|---------|
| 🖥️ **Web Dashboard** | `news_aggregator.html` | Responsive Thistle-themed UI with Gemini Pro AI analysis |
| 🐍 **Python CLI Engine** | `smart_newssphere.py` | Live data fetching, TF-IDF clustering, terminal reports |

---

## 🚀 Features

### 🖥️ Web Dashboard — `news_aggregator.html`

> Powered by **Google Gemini Pro** for rich, multi-layered analysis.

- **🤖 AI-Powered Analysis** — Generates summaries, sentiment scores, and contextual insights per article
- **🔍 Root Cause Analysis** — Explains the *why* behind every story, not just the *what*
- **📜 Historical Context** — Connects current events to relevant past occurrences
- **❓ Follow-up Questions** — Auto-generates thought-provoking questions for deeper reading
- **🎨 Modern Thistle UI** — Polished purple/white responsive grid layout
- **🔎 Smart Filtering** — Filter articles by **Category**, **Location** (USA/India), and **Type**

---

### 🐍 Python CLI Engine — `smart_newssphere.py`

> A robust ML-backed backend that runs entirely in your terminal.

- **📡 Live Data Fetching** — Pulls real-time articles from **NewsData.io API** and **BBC RSS feeds**
- **🧠 TF-IDF Vectorization** — Converts raw text into machine-readable feature vectors
- **🗂️ Agglomerative Clustering** — Groups semantically related stories into meaningful topic clusters automatically
- **📊 Console Reporting** — Structured text summaries and clustering stats printed in your terminal

---

## 📂 Project Structure

```
news_aggregator_project/
│
├── 📁 news_aggregator_project/     # Django project config
│   ├── __init__.py
│   ├── asgi.py                     # ASGI entry point
│   ├── settings.py                 # Project settings & configuration
│   ├── urls.py                     # Root URL routing
│   └── wsgi.py                     # WSGI entry point
│
├── 📁 news_collector/              # Main Django app
│   ├── 📁 migrations/              # Database migrations
│   ├── __init__.py
│   ├── admin.py                    # Django admin configuration
│   ├── apps.py                     # App configuration
│   ├── models.py                   # Database models (Article, etc.)
│   ├── scraper.py                  # News scraping & fetching logic
│   ├── tests.py                    # Unit tests
│   └── views.py                    # Request handlers & API views
│
├── 📄 outcome                      # Sample output / results
├── 🐍 manage.py                    # Django management CLI
├── 🔧 .gitattributes
└── 📖 README.md                    # Project Documentation
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Frontend** | HTML5, Tailwind CSS, Vanilla JavaScript |
| **AI / LLM** | Google Gemini Pro API |
| **Backend** | Python 3.8+, Django |
| **ML / NLP** | Scikit-Learn (TF-IDF, Agglomerative Clustering), NumPy |
| **Data Sources** | NewsData.io API, BBC RSS Feeds |
| **Database** | Django ORM (SQLite by default) |

---

## 📦 Prerequisites

Before you begin, make sure you have:

- ✅ **Python 3.8+** installed
- ✅ A **Google Gemini API Key** — [Get one here](https://ai.google.dev)
- ✅ A **NewsData.io API Key** — [Get one here](https://newsdata.io)

---

## ⚙️ Installation

**1. Clone or download the project:**
```bash
git clone https://github.com/akshatxn/news-aggregator-project.git
cd news-aggregator-project
```

**2. Install Python dependencies:**
```bash
pip install django requests feedparser scikit-learn numpy
```

**3. Apply database migrations:**
```bash
python manage.py migrate
```

---

## 🖥️ Running the Web Dashboard

The web dashboard requires a local server to avoid browser CORS security blocks.

**Step 1 — Start a local server:**
```bash
cd path/to/NewsSphere
python -m http.server 8000
```

**Step 2 — Open in your browser:**
```
http://localhost:8000/news_aggregator.html
```

**Step 3 — Configure your Gemini API Key:**

Open `news_aggregator.html` in any code editor and find line ~380:
```javascript
const apiKey = "";  // 👈 Paste your Google Gemini API Key here
```

---

## 🐍 Running the Python CLI Engine

The CLI engine fetches live news and runs ML clustering directly in your terminal.

**Step 1 — Set your NewsData.io API Key:**

Open `fetcher.py` and set:
```python
NEWSDATA_API_KEY = "your_api_key_here"
```

**Step 2 — Run the main script:**
```bash
python smart_newssphere.py
```

The script will:
1. 📡 Fetch live articles from NewsData.io and BBC RSS
2. 🧠 Run TF-IDF vectorization on article content
3. 🗂️ Cluster related stories using Agglomerative Clustering
4. 📊 Print grouped topic summaries to your console

---

## 🔑 API Keys — Quick Reference

| Key | Used In | Where to Get |
|-----|---------|-------------|
| `Google Gemini API Key` | Web Dashboard (`news_aggregator.html`) | [ai.google.dev](https://ai.google.dev) |
| `NewsData.io API Key` | Python CLI (`fetcher.py`) | [newsdata.io](https://newsdata.io) |

> ⚠️ **Never commit your API keys to version control.** Consider using environment variables or a `.env` file in production.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Make your changes and commit: `git commit -m "Add some feature"`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<div align="center">

Made with ❤️ by [akshatxn](https://github.com/akshatxn)

⭐ If you found this project useful, consider giving it a star!

</div>
