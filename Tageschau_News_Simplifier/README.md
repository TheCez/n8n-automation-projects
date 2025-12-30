# 🚀 Automated News Simplifier and Whatspp Message Scheduler

## 💡 What it does
This n8n workflow automates the process of gathering  latest news from Tagesschau, formatting it with AI, Simplifying it, and checking if the date matches today before sending it through whataspp.

## 🛠️ Tools Used
* **n8n** (Logic & Orchestration)
* **RSS Feeds** (Data Source)
* **JavaScript** (Date Parsing & Custom Logic)
* **Gemini 3.0 flash** (Content Summarization)

## ⚙️ How it works
1. **Trigger:** Runs every morning at 8:00 AM CET.
2. **Fetch:** Pulls RSS data from Tagesschau.
3. **Filter:** Compares `pubDate` with `currentDate` using custom Javascript logic to ensure relevance.
4. **Transform:** Summarizes the article into a Whatsapp message-friendly format.
5. **Post:** Sends the content to the Whatsapp number.

## 📸 Workflow Diagram
![Workflow Screenshot](./diagram.png)

## 📦 How to use
1. Download the `workflow.json` file.
2. Import it into your n8n instance.
3. Set up your LinkedIn credentials.