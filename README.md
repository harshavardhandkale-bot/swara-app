# Swara — Expense Tracker
### Kale Pharma Pvt Ltd

A simple expense tracking app built with Python and Streamlit.

## Features
- 📷 Upload bill photos — AI reads date, vendor, amount, category automatically
- 📋 Expense statement with date & category filters
- 📥 Download expenses as Excel (ready for Marg ERP import)
- 📊 Summary with category and payment mode breakdown
- 📈 Daily spend chart

## Setup

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

### 2. Add your Gemini API key
Create `.streamlit/secrets.toml`:
```toml
GEMINI_API_KEY = "your-gemini-api-key-here"
```
Get your free API key at: https://aistudio.google.com/app/apikey

### 3. Run locally
```bash
streamlit run app.py
```

## Deploy on Streamlit Cloud (Free)
1. Push this repo to GitHub (private)
2. Go to https://share.streamlit.io
3. Connect your GitHub account
4. Select this repo → `app.py`
5. In Advanced Settings → Secrets, add:
   ```
   GEMINI_API_KEY = "your-key-here"
   ```
6. Click Deploy

## Tech Stack
- Python 3.11+
- Streamlit
- Google Gemini 1.5 Flash (AI bill reading)
- SQLite (local database)
- Pandas + OpenPyXL (Excel export)

