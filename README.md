🕵️‍♀️ Scam Detective Application
Detect scams and deepfakes straight from your browser — powered by AI and n8n automation.

🔍 Overview

Digital Detective is a lightweight, browser‑based toolkit designed to help users verify digital content instantly.
It offers two main AI detection tools:

Text Detective – analyzes suspicious messages to determine if they are potential scams or safe communications.
Deepfake Detective – checks uploaded images or short videos for possible manipulation or synthetic generation.
Each feature connects to n8n webhooks that forward the user input to API.AI, processes the data, formats the response, and returns a clear result directly within the web interface.
All webhook endpoints are embedded in the HTML but safely hidden from display.

💡 Key Features

💬 Scam Message Detection: Paste any suspicious text and get an instant AI‑based safety analysis.
🎭 Deepfake Analysis: Upload an image or video to check for signs of manipulation.
🔗 Automated Integration via n8n: Smooth connection between the frontend and API.AI through webhook workflows.
📱 Mobile‑First Experience: Fully responsive phone‑style interface designed for clarity and ease of use.
🧩 System Architecture

Frontend

Built entirely with HTML, CSS, and Vanilla JavaScript.
Three core pages:
index.html → Dashboard hub
text_detective.html → Scam message detection
deepfake_detective.html → File‑based deepfake analysis
Integration Flow (via n8n)

Each tool triggers an n8n webhook → formats data → sends it to API.AI → formats and returns results → responds to the webhook → displays on screen.


Text Detective Flow
User Input → Webhook (text) → Text Formatter → API.AI → Response Formatter → Frontend

Deepfake Detective Flow
User Upload → Webhook (photo/video) → Data Formatter → API.AI → Response Formatter → Frontend
All webhook URLs are stored within the JavaScript section of the HTML files (hidden and not publicly shown).

🧑‍💻 My Role & Responsibilities

🎨 Frontend Development: Designed and coded the complete user interface for all pages.
🔗 Integration Setup: Configured all n8n → API.AI webhooks and connected them to the frontend.
🧭 Project Coordination: Acted as main correspondent during hackathon collaboration and handled system testing.
🛠️ Tech Stack

Category	Technology Used
Interface	HTML5, CSS3, JavaScript
Automation	n8n Cloud (Webhook & Data Formatting)
API Engine	API.AI
Design Focus	Mobile‑first responsive design + interactive “phone frame” UI

🏆 Hackathon Background

This project was built as part of a 2025 Generative AI Hackathon, demonstrating how simple front‑end tools can securely connect to AI systems through workflow automation and webhooks — enabling real‑time detection that anyone can use.

⚠️ Important Reminder

🚨 Webhooks Hidden:
For privacy and security, the n8n webhook URLs inside this project are hidden.
If you wish to run your own version with live AI analysis, please:

Create your own n8n account on n8n.io.
Set up new webhook workflows for your text and deepfake detectors.
Replace the hidden N8N_URL and N8N_DEEPFAKE_URL values in the HTML <script> sections with your own webhook URLs.
