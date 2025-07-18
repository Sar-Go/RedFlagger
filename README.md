# 🧠 EmotiGuard — Emotional Intelligence for Your WhatsApp Chats

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![LangChain](https://img.shields.io/badge/LangChain-0.2.x-success)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o--ff69b4)
![Streamlit](https://img.shields.io/badge/Streamlit-App-red)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

**EmotiGuard** is an emotionally intelligent AI-powered analyzer for WhatsApp chats. It goes beyond generic sentiment analysis by identifying manipulation patterns, sudden emotional spikes, and potential red flags in day-to-day conversations.

Built with `LangChain`, `OpenAI`, and `Streamlit`, it transforms raw exported `.txt` WhatsApp files into insightful, color-coded visualizations that surface the *emotional truth* beneath the surface of your chats.

---

## 🚀 Features

- ✅ **WhatsApp Chat Loader & Cleaner** (media-aware)
- 🧠 **LLM-powered Sentiment Analyzer** (with fine-grained classification)
- 📉 **Sentiment Timeline Chart** (track emotional fluctuations)
- 🌩️ **Spike Detection & Red Flag Alerts**
- ☁️ **Color-coded Message Cloud**
- 🧪 Ready for **Agentic workflows** and **RAG-based enhancements**

## MVP System Design
- 🧾 Input Module: User uploads .txt export of WhatsApp chat. Parser splits messages: sender, timestamp, content.
- 🧮 Preprocessing & Chunking: Clean metadata, remove system messages. Chunk into: Per day / week Per topic turn (based on shifts in conversation)
- 🧰 Analysis Engines (Chains) 🔴 Red Flag Detector

## Prompts LLM to find:

- Gaslighting
- Breadcrumbing
- Guilt-tripping
- Blame-shifting
- Love bombing
- Silent treatment
- Output: Flag + explanation + message reference.

## 📊 Frontend (optional MVP interface): 
- Simple Streamlit UI: Upload chat Run analysis Visual output: flags, charts, downloadable report

---

## 🛠 Tech Stack

- `Python`
- `LangChain`
- `OpenAI GPT (gpt-3.5-turbo)` *(or configurable)*
- `Streamlit`
- `Matplotlib / Seaborn`
- `Pandas`

---

## 📂 How to Use

1. Export your WhatsApp chat as `.txt` file (without media).
2. Launch the Streamlit app:
   ```bash
   streamlit run emotiguard.py
   ```
3. Upload chat file, view timeline, red flags, and insights.

> ⚠️ Media placeholders (like `"<Media omitted>"`) are intelligently handled.

---

## 🤖 Coming Soon

- Relationship Health Score
- Toxicity Detection
- Persona-Based Behavior Summaries
- Support for multiple chat formats

---

## 📄 License

MIT License. Open for contributions!