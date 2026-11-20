# Full Stack Academy RAG Chatbot (Streamlit)

## What I built

Built a document question-answering chatbot using Streamlit. It uses retrieval-augmented generation (RAG) to find relevant information in PDFs stored in the project’s pdfs/ folder and answer users’ questions.

## Setup
```bash
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
cp .streamlit/secrets.toml.example .streamlit/secrets.toml   # then paste your Groq key
```

Put your PDFs (what was `/content/fsa_pds` in Colab) into the `pdfs/` folder.

## Run
```bash
streamlit run app.py
```

## Deploy to Streamlit Community Cloud
1. Push this folder to GitHub (secrets.toml is git-ignored).
2. Create an app at share.streamlit.io pointing to `app.py`.
3. In the app's **Settings → Secrets**, paste: `GROQ_API_KEY = "gsk_..."`

## Project summary

This project combines PDF retrieval with a language model to answer questions grounded in the provided documents. The README includes setup and run instructions, and explains how to configure the Groq API key for local use or deployment.
