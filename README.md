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
