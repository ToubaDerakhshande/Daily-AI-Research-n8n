<div align="center">

# 🚀 Daily AI Research Digest

✨ **Automated AI & Research Paper Curation Powered by n8n** ✨

[![n8n](https://img.shields.io/badge/n8n-Workflow-ff6d5a?style=flat-square&logo=n8n&logoColor=white)](https://n8n.io)
[![OpenRouter](https://img.shields.io/badge/AI-OpenRouter-purple?style=flat-square)](https://openrouter.ai)
[![Telegram](https://img.shields.io/badge/Delivery-Telegram-24a1de?style=flat-square&logo=telegram&logoColor=white)](https://telegram.org)

</div>

---

## 🌟 Overview
Staying updated with the latest artificial intelligence research can be exhausting. **Daily AI Research Digest** is a seamless n8n automation workflow that aggregates cutting-edge papers from multiple top-tier sources, intelligently summarizes them using advanced LLMs, and broadcasts a clean, structured digest directly to Telegram.

---

## 🔥 Key Features

- ⏰ **Automated Daily Trigger:** Runs on a scheduled cron job to deliver fresh insights every day.
- 📡 **Multi-Source Aggregation:** 
  - 📚 **arXiv API** (`cs.AI` category)
  - 🤗 **Hugging Face Daily Papers** (Community trending favorites)
  - 🌿 **Nature RSS Feed** (Top scientific journal publications)
- 🧠 **AI-Powered Summaries:** Leverages **OpenRouter** models to generate crisp, structured summaries (Problem & Goal, Method & Innovation, Key Results).
- 🧹 **Smart Deduplication:** Caches up to the last 2,000 sent papers in workflow static data to prevent any duplicate notifications.
- 📱 **Clean Formatting:** Publishes beautifully formatted HTML messages without clutter.

---

## ⚙️ Quick Workflow Flow

1. ⏱ **Schedule** triggers the workflow daily.
2. 📥 **Fetch** latest papers concurrently from arXiv, Hugging Face, and Nature.
3. ⚙️ **Filter & Process** raw data and filter out previously seen items.
4. 🤖 **Summarize** selected highlights using OpenRouter LLM.
5. 📤 **Format & Deliver** clean markdown/HTML updates to Telegram.

---

## 🛠 Prerequisites & Setup

To get this workflow running smoothly in your n8n instance:

1. **Import Workflow:** Import the provided `Daily AI Research Digest.json` file into your n8n dashboard.
2. **Credentials Setup:**
   - Configure your **OpenRouter API Key** credential for the AI Agent node.
   - Set up your **Telegram Bot Token** credential for the Telegram node.
3. **Configure Channel:** Update the target chat ID/channel destination in the Telegram send node.
4. **Activate:** Toggle the workflow from `Inactive` to **`Active`**.

---

## 💡 Pro-Tip
*Make sure to respect rate limits when fetching from external APIs like arXiv by keeping proper delays between requests if you modify the trigger frequency.*

---
