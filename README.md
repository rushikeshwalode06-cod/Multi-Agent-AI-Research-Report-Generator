# NEXUS AI — Multi-Agent Research & Report Generator

A Streamlit research assistant using LangChain, LangGraph, and Google Gemini API (not OpenAI API).

## Features
- Researcher, Analyst, and Report Writer agents
- DuckDuckGo web search results with source URLs
- Dark purple RGB/neon dashboard
- Markdown, TXT, and PDF report downloads
- Basic error handling for missing keys and API/quota issues

## Setup (Windows / VS Code)

1. Install Python 3.10 or newer and VS Code.
2. Open this folder in VS Code.
3. Create a virtual environment in the VS Code terminal:

   ```powershell
   python -m venv .venv
   .venv\Scripts\activate
   ```

4. Install dependencies:

   ```powershell
   python -m pip install --upgrade pip
   pip install -r requirements.txt
   ```

5. Copy `.env.example` to `.env`. Get a key at https://aistudio.google.com/apikey and replace the placeholder with your key. Never upload `.env` to GitHub.
6. Run the app:

   ```powershell
   streamlit run app.py
   ```

## Notes
- Web search requires internet access and may be rate-limited or unavailable sometimes.
- Gemini model access and quotas depend on your Google AI Studio account. If a model is unavailable, choose another model offered in the app.
- Search snippets are leads, not proof. Verify important claims on original pages.
