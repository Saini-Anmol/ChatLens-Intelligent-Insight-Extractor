# ChatLens – Intelligent Insight Extractor

ChatLens is an intelligent analysis pipeline designed to extract, classify, score, and summarize high-value information from **Telegram chat export files**.  
It identifies signals related to **military activity, geopolitics, armed groups, trafficking, fraud networks, drones, weapons**, and more.

The entire workflow runs seamlessly in **Google Colab** and generates:

- Clean JSON datasets of extracted intelligence paragraphs  
- Weighted scoring based on domain-specific keyword categories  
- Telegram-style HTML visualizations  
- AI-generated summaries using T5-small  
- Direct “View Original” links pointing to messages in Google Drive  

ChatLens is ideal for OSINT workflows, conflict monitoring, geopolitical analysis, and intelligence research.

---

## 🔥 Features

### ✔ **1. Intelligent Message Extraction**
Automatically extracts only relevant messages from Telegram HTML files based on domain-specific lexicons such as:
- Troop movements  
- Airstrikes & bombing  
- Drones / aircraft  
- Weapons & artillery  
- Armed groups & military factions  
- Border & regional activities  
- Trafficking, drugs, gambling  
- Fraud / online crimes  
- Geopolitical and cross-border interactions  

### ✔ **2. Weighted Keyword Scoring Engine**
Each keyword is assigned a weight (example: `drone:0.7`, `convoy:0.6`).  
ChatLens computes:
Final Score = Σ (weight × frequency of keyword)

This results in highly accurate prioritization of messages based on their intelligence value.

### ✔ **3. Location Extraction**
ChatLens detects potential geographical indicators using keywords such as:
`border`, `mountain`, `region`, `village`, `checkpoint`, etc.

### ✔ **4. Telegram-Style HTML Output**
Readable message cards include:
- Username  
- Timestamp  
- Full message text  
- Weighted score  
- Word count  
- “View Original” deep link to Google Drive  
- Telegram-inspired UI design  

### ✔ **5. AI-Based Summaries (T5-small)**
Long paragraphs are automatically summarized using the T5-small model.  
Summaries appear in highlighted yellow blocks.

### ✔ **6. Research-Ready JSON Output**
The clean JSON file includes:
- Matched keywords  
- Weighted scores  
- Word counts  
- Locations  
- Full text  
- User metadata  

Useful for ML/AI pipelines, dashboards, and data analytics.

---
