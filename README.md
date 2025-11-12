# Cloudflare Interview Assistant 🤖💼

> **Fast Track Assignment Submission**
> An AI-powered mock interview agent built on the Cloudflare Developer Platform.

**[🔴 LIVE DEMO](https://cf_ai_agent_bot.xuwenjin824.workers.dev)** *(https://cf_ai_agent_bot.xuwenjin824.workers.dev)*

## 📖 Overview

The **Cloudflare Interview Assistant** is a stateful AI agent designed to help candidates practice for technical roles. Unlike stateless chatbots, this agent utilizes **Cloudflare Durable Objects** to maintain a persistent memory of the conversation, allowing it to remember the candidate's name, applied role, and previous technical answers throughout the session.

It simulates a real interview workflow: gathering candidate details, asking targeted technical questions (focused on Cloudflare technologies), and providing constructive feedback after every answer.

## 🚀 Key Features

* **🧠 Stateful Memory:** Powered by **Durable Objects**, the agent remembers context (User Name, Role, History) across the entire session.
* **🦙 Llama 3.3 Intelligence:** Utilizes `llama-3.3-70b-instruct` via **Workers AI** for high-quality, nuanced technical feedback.
* **🔄 Structured Workflow:** Implements a strict interview loop: *Question → Wait for Answer → Analyze & Provide Feedback → Next Question*.
* **🎨 Custom UI:** A professional, blue-themed React interface designed for a focused interview experience.

---

## ⚡️ Getting Started

Follow these steps to run the project locally or deploy it to your own Cloudflare account.

### Prerequisites
* **Node.js** (v16.13.0 or later)
* **NPM** (comes with Node.js)
* A **Cloudflare Account** with Workers AI enabled.

### 1. Installation

Clone the repository and install dependencies:

```bash
# Clone the repo
git clone https://github.com/AlexWen1952/cf_ai_agent_bot.git

# Navigate to the project folder
cd cf_ai_agent_bot

# Install NPM packages
npm install
```

### 2. Configuration
Step A: Authenticate Log in to your Cloudflare account to enable access to Workers AI and Durable Objects:
```bash
npx wrangler login
```
A browser window will open. Click "Allow" to authorize the connection.

### 3. Running Locally
Start the local development server. This mimics the Cloudflare environment (Workers & Durable Objects) directly on your machine:
```bash
npm start
```
* The app should now be running at http://localhost:5173.

* Open this URL in your browser to test the interview agent.

* Note: Local mode uses a proxy to connect to Cloudflare's AI models, so an internet connection is required.

### 4. Deployment
To publish your agent to the global Cloudflare network:
```bash
npm run deploy
```
* If prompted, register a workers.dev subdomain (this is required for your first deployment).

* Once finished, the terminal will output your live URL (e.g., https://cf_ai_agent_bot.xuwenjin824.workers.dev).