# 🩺 HIA (Health Insights Agent)

AI Agent to analyze blood reports and provide detailed health insights.

<p align="center">
  <a href="https://github.com/harshhh28/hia/issues"><img src="https://img.shields.io/github/issues/harshhh28/hia"></a> 
  <a href="https://github.com/harshhh28/hia/stargazers"><img src="https://img.shields.io/github/stars/harshhh28/hia"></a>
  <a href="https://github.com/harshhh28/hia/network/members"><img src="https://img.shields.io/github/forks/harshhh28/hia"></a>
  <a href="https://github.com/harshhh28/hia/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg">
  </a>
</p>

<p align="center">
  <a href="#-features">Features</a> |
  <a href="#%EF%B8%8F-tech-stack">Tech Stack</a> |
  <a href="#-installation">Installation</a> |
  <a href="#-contributing">Contributing</a> |
  <a href="#%EF%B8%8F-author">Author</a>
</p>

<p align="center">
  <a href="https://github.com/harsha-egen/hia"><img src="https://raw.githubusercontent.com/harshhh28/hia/main/public/HIA_demo.gif" alt="Usage Demo"></a>
</p>

## 🌟 Features

- Intelligent agent-based architecture with multi-model cascade system
- In-context learning from previous analyses and knowledge base building
- Medical report analysis with personalized health insights
- PDF upload, validation and text extraction (up to 20MB)
- Secure user authentication and session management
- Session history with report analysis tracking
- Modern, responsive UI with real-time feedback

## 🛠️ Tech Stack

- **Frontend Framework**: Streamlit
- **AI Integration**: Multi-model architecture via Groq
  - Primary: meta-llama/llama-4-maverick-17b-128e-instruct
  - Secondary: llama-3.3-70b-versatile
  - Tertiary: llama-3.1-8b-instant
  - Fallback: llama3-70b-8192
- **Database**: Supabase
- **PDF Processing**: PDFPlumber
- **Authentication**: Supabase Auth

## 🚀 Installation

#### Requirements 📋

- Python 3.8+
- Streamlit 1.30.0+
- Supabase account
- Groq API key
- PDFPlumber
- Python-magic-bin (Windows) or Python-magic (Linux/Mac)

#### Getting Started 📝

1. Clone the repository:

```bash
git clone https://github.com/harsha-egen/hia.git
cd hia
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Required environment variables (in `.streamlit/secrets.toml`):

```toml
SUPABASE_URL = "your-supabase-url"
SUPABASE_KEY = "your-supabase-key"
GROQ_API_KEY = "your-groq-api-key"
```

4. Run the application:

```bash
streamlit run src\main.py
```

## 📁 Project Structure

```
hia/
├── requirements.txt
├── README.md
├── src/
│   ├── main.py                 # Application entry point
│   ├── auth/                   # Authentication related modules
│   │   ├── auth_service.py     # Supabase auth integration
│   │   └── session_manager.py  # Session management
│   ├── components/             # UI Components
│   │   ├── analysis_form.py    # Report analysis form
│   │   ├── auth_pages.py       # Login/Signup pages
│   │   ├── footer.py          # Footer component
│   │   └── sidebar.py         # Sidebar navigation
│   ├── config/                # Configuration files
│   │   ├── app_config.py      # App settings
│   │   └── prompts.py         # AI prompts
│   ├── services/              # Service integrations
│   │   └── ai_service.py      # AI service integration
│   ├── agents/                # Agent-based architecture components
│   │   ├── agent_manager.py   # Agent management
│   │   └── model_fallback.py  # Model fallback logic
│   └── utils/                 # Utility functions
│       ├── validators.py      # Input validation
│       └── pdf_extractor.py   # PDF processing
```

## 👨‍💻 Contributors

Thanks to all the amazing contributors who have helped improve this project!

| Avatar | Name | GitHub | Role | Contributions |
|--------|------|--------|------|---------------|
| <img src="https://github.com/harsha-egen.png" width="50px" height="50px" alt="harsha"/> | Harsha | [harsha-egen](https://github.com/harsha-egen) | Project Creator & Maintainer | Core implementation, Documentation |

<!-- To future contributors: Your profile will be added here when your PR is merged! -->

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙋‍♂️ Author

Created by [Harsha Gubbi Chandrashekar]
