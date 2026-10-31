# AI Lead Management and Qualification Pipeline

An automated lead scoring and qualification system built with **n8n**, **Google Gemini**, and **Google Workspace** that processes form submissions, evaluates lead fit using AI, and routes qualified records to Google Sheets[cite: 1].

---

## 📌 Features

- **Automated Lead Intake:** Listens for incoming responses directly from Google Forms via webhook triggers[cite: 1].
- **AI-Powered Lead Scoring:** Evaluates lead intent, budget, and business requirements against qualification criteria using Google Gemini[cite: 1].
- **Structured Categorization:** Labels leads into structured tiers (e.g., Qualified, Follow-up, Unqualified)[cite: 1].
- **Automated Spreadsheet Routing:** Stores enriched applicant data and scoring rationale directly into Google Sheets[cite: 1].

---

## 🛠️ Tech Stack

- **Automation:** n8n[cite: 1]
- **AI / LLM:** Google Gemini API[cite: 1]
- **Workspace Tools:** Google Forms, Google Sheets[cite: 1]
- **Data Protocols:** JSON, REST APIs, Webhooks[cite: 1]

---

## ⚙️ Workflow Architecture

1. **Trigger:** Receives form submission payload from Google Forms[cite: 1].
2. **Preprocessing:** Formats submission fields into a standardized JSON schema[cite: 1].
3. **AI Qualification:** Passes lead responses to Google Gemini with a defined scoring prompt[cite: 1].
4. **Data Sync:** Writes qualified lead details, scores, and summary notes into Google Sheets[cite: 1].

---

## 🚀 Setup & Installation

1. Import `workflow.json` into your **n8n** instance.
2. Configure credentials:
   - **Google Gemini API Key**[cite: 1]
   - **Google Sheets OAuth2 / Service Account**[cite: 1]
3. Connect your Google Form submission webhook to the workflow trigger node.
4. Set your destination Google Sheet spreadsheet ID.
5. Activate the workflow.
