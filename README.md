# email-triage-AI
Triange AI
Triange AI is a production-style AI SaaS prototype for autonomous email automation and workflow operations.

What is included
Premium landing page with animated AI email visuals
Glassmorphism Google sign-in UI and session route structure
Live dashboard with counters, agent monitoring, notifications, workflow logs, and analytics
n8n-inspired workflow visualization
Analytics page for email distribution, response metrics, accuracy, and performance
Demo simulation buttons for incoming email, AI reply generation, workflow execution, and automated send
Modular service layer for AI, Gmail, Firebase, and n8n integration points
Run locally
Install dependencies, then start the development server:

npm install
npm run dev
Open http://localhost:3000.

Integration map
app/api/ai/reply/route.ts calls the AI service layer for intent detection, reply generation, and safety validation.
app/api/gmail/simulate/route.ts represents incoming Gmail reads.
app/api/workflows/run/route.ts simulates n8n execution, Gmail send, and Firebase event persistence.
lib/services/* contains provider modules that can be replaced with real SDK calls.
Environment
Copy .env.example to .env.local and fill in provider credentials for Firebase, Gmail OAuth, n8n, OpenAI, or OpenRouter.
