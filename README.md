# email-triage-AI
# Triange-AI

Triange-AI is an AI-powered email automation workflow built with n8n. It reads incoming Gmail messages, understands the intent, generates a professional reply, checks safety, and sends approved responses automatically.

## Problem

Businesses waste time manually reading, classifying, and replying to repetitive emails such as leads, follow-ups, support requests, and meeting messages.

## Solution

Triange-AI automates the email response workflow using AI agents. The system helps teams respond faster while keeping a safety approval step before sending emails.

## Key Features

- Gmail email trigger
- AI email triage
- Intent and priority detection
- Personalized reply generation
- Safety validation before sending
- Automatic Gmail reply sending
- Optional Google Sheets logging
- Website/Lovable integration using n8n Webhook

## Workflow Access

The complete n8n workflow used for Triange AI is available inside this repository.

Workflow File:

* `TriangeAI_n8n_Workflow.json`

This workflow contains:

* AI Email Intent Detection
* Automated Reply Generation
* Reply Optimization
* Safety Validation
* Automated Email Sending
* Analytics Extraction
* Google Sheets Logging

To test the workflow:

1. Open n8n
2. Click “Import Workflow”
3. Upload the provided JSON file
4. Configure required API credentials
5. Run the workflow

##USER FLOW DIAGRAM

Incoming Email (Gmail)
        ↓
Trigger Activated
        ↓
AI Agent analyzes email
        ↓
Intent Classification
   ├── Lead Inquiry
   ├── Support Request
   ├── Meeting Request
   └── General Email
        ↓
AI Response Generator
        ↓
Approval Check (Optional)
        ↓
Auto Send Email
        ↓
Update Database (Firebase)
        ↓
Dashboard Analytics Update
        ↓
Notification Sent (User)


