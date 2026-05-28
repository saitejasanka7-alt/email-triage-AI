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

## Workflow

```text
Gmail Trigger
-> Triage AI Agent
-> Generate Reply
-> Safety Check
-> Check Safety Approval
-> Send Reply
-> Log Result


How It WorksA new email arrives in Gmail.
n8n triggers the workflow.
Triage AI Agent detects intent, priority, and summary.
Generate Reply Agent writes a professional response.
Safety Check Agent validates the reply.
If approved, Gmail sends the reply automatically.
The result can be logged to Google Sheets or shown on a website dashboard.
Safety DesignTriange-AI does not blindly send every AI response. The workflow includes a safety approval node:

approved = true  -> Send Reply
approved = false -> Skip / Log for review

This helps prevent unsafe, incorrect, or unprofessional automated emails from being sent.
Hackathon GoalThe goal of Triange-AI is to help businesses save time and improve communication speed by combining workflow automation with AI-powered email understanding and response generation.
Future ImprovementsMulti-account Gmail support
Better analytics dashboard
CRM integration
WhatsApp and Slack notifications
Human approval dashboard
Follow-up scheduling
Lead scoring
Team inbox support

