
# Text to PowerPoint – Automatic Deck Creator

Transform long text or markdown into a professional presentation in minutes.

This lightweight tool converts raw content (notes, essays, reports, or markdown) into a structured and styled PowerPoint deck. Bring your own slide template, provide an API key for your preferred LLM, and let the app build a polished .pptx for you.

---

## ✨ Features

* 📝 Flexible Input – Paste paragraphs, markdown, or raw text.
* 🎯 Custom Guidance – Add a short hint like “design as a startup pitch deck” or “summarize as lecture slides.”
* 🔐 Use Your Own API Key – Works with OpenAI, Anthropic, Gemini, and others (keys never stored or tracked).
* 🎨 Template Support – Upload your .pptx or .potx file to preserve fonts, colors, and layouts.
* 🖼️ Image Carryover – Reuses visuals already in your uploaded template.
* ⚡ Slide Splitting – Automatically divides text into well-sized slides.
* 📥 Quick Download – Get a ready-to-present .pptx instantly.
* 🔒 Privacy First – No saving of input text, templates, or API credentials.

---

## 🚀 Quick Start

### 1. Clone the repo

```bash
git https://github.com/DevyanshJain/TDS-PPT-Generator/edit/main/README.md
cd TDS-PPT-Generator
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run locally

```bash
uvicorn app:app --reload
```

Visit: [http://localhost:8000](http://localhost:8000)

### 4. Deploy (Railway/Render/Vercel/Heroku)

Compatible with Railway, Render, Vercel, Heroku, and similar platforms. Connect the repo and deploy directly.

---

## 🖥️ How It Works

1. Paste your content.
2. Optionally add a one-liner with style/tone preferences.
3. Provide your LLM API key.
4. Upload a PowerPoint template.
5. Hit Generate → download your finished deck.

---

## 🛠️ System Overview

* **Frontend**:

  * Clean UI for input, uploads, and downloads
  * Shows history and progress updates
  * Toasts and feedback for better UX

* **Backend (FastAPI)**:

  * Receives text, hints, template, and API key
  * Splits text into slide-sized chunks
  * Applies formatting and layout from uploaded template
  * Builds .pptx using python-pptx

---

## 🌟 Future Ideas

* Automatic speaker notes generation
* Predefined style presets (research summary, pitch deck, lecture notes)
* Real-time slide preview before download
* Smarter retries + stronger error handling for API timeouts

---

## 📄 License

MIT License – free to use, modify, and share.

