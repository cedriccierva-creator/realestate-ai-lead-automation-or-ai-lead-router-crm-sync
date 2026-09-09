# Real Estate Lead AI Automation & CRM Sync

## 📖 Overview
In high-ticket sales, 78% of prospects sign with the agency that responds first. This project eliminates manual response friction by automating instant lead allocation, categorization, and personalized email drafting. Upon receiving an inquiry, the system parses the unstructured data, syncs with multiple CRMs, and drafts a contextual reply in under two seconds.

## ✨ Features
* **Instant Lead Processing:** Triggers immediately upon receiving a new lead email inquiry.
* **AI Data Extraction:** Uses Google Gemini AI to parse unstructured email text into structured JSON containing specific budget and property preferences.
* **Intelligent Routing:** Directs data payloads to different endpoints based on the extracted information.
* **CRM Synchronization:** Automatically creates and updates contact profiles in GoHighLevel and Brevo simultaneously.
* **AI Email Drafting:** Leverages an HTTP POST request to an AI drafting engine to generate a highly personalized, ready-to-send response in Gmail.

## 🛠️ Tech Stack
* Make.com (Workflow Orchestration)
* Google Gemini AI (Data Parsing & Extraction)
* GoHighLevel (CRM)
* Brevo (Contact Management)
* Gmail (Trigger & Draft Destination)

## 🚀 How It Works
1. A new lead inquiry arrives in the designated Gmail inbox.
2. The workflow triggers and passes the raw email body to Google Gemini.
3. Gemini extracts specific details (e.g., $1,250,000 budget, 1845 Alki Ave SW) into a structured JSON payload.
4. A router splits the workflow to handle CRM syncing and email generation in parallel.
5. GoHighLevel and Brevo receive the new contact details via direct integrations and phone number parsing.
6. The AI drafting engine generates a customized follow-up email referencing the specific property and budget.
7. The customized email is placed directly in the sales team's Gmail drafts folder, ready to send.

## 📈 Business Impact
* Eliminates manual data entry across multiple databases.
* Reduces lead response time from hours to less than two seconds.
* Guarantees zero-delay outreach before the prospect explores competitors.
