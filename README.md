# 🚀 n8n LinkedIn Content Automation Workflow

## 📌 Project Overview

This project demonstrates an automated LinkedIn content generation workflow built using **n8n**.

The workflow runs on a schedule, fetches pending content topics from Google Sheets, generates LinkedIn-formatted posts, updates the sheet, and sends the generated content via email for review.

For security reasons, direct LinkedIn posting was intentionally disabled, as the connected account is a university-registered official account.

---

## ⚙️ Workflow Architecture

The automation follows this structure:

Schedule Trigger  
↓  
Fetch Pending Topic (Google Sheets)  
↓  
Generate LinkedIn-Style Content  
↓  
Update Sheet (Status → Done)  
↓  
Send Email Notification  
↓  
Mark as Posted  

---

## 📊 Google Sheets Structure

The workflow uses the following sheet structure:

| ID | Topic | Status | Generated_Content | Posted |
|----|--------|--------|------------------|--------|

### Status Values:
- Pending
- Done

### Posted Values:
- Yes
- No

This ensures:
- No duplicate processing
- Controlled state management
- Clean automation flow

---

## 📬 Email-Based Publishing Simulation

Instead of automatically posting to LinkedIn, the generated content is sent via email for approval.

This approach:
- Prevents unintended public posting
- Protects official LinkedIn accounts
- Simulates real-world approval workflows

The LinkedIn node can be enabled in production with proper authorization and approval mechanisms.

---

## 🛠 Technologies Used

- n8n (Cloud)
- Google Sheets Integration
- HTTP Request Node
- Gmail Node
- Scheduled Trigger Automation

---

## 🎯 Key Features

- Fully automated scheduled execution
- Dynamic topic fetching from Google Sheets
- LinkedIn-style content formatting
- Duplicate prevention logic
- Status-based workflow control
- Safe publishing simulation via email

---

## 🔐 Security Note

The LinkedIn integration was intentionally disabled because the connected account is an official university-registered profile.

Auto-posting was avoided to maintain account integrity and prevent unintended public publishing.

---

## 🚀 Future Enhancements

- Approval column before publishing
- Direct LinkedIn integration with admin approval
- AI-based advanced content generation
- Logging & error handling improvements
- Slack/Teams notification integration


[Your Name]  
Automation Internship Project – n8n Workflow
