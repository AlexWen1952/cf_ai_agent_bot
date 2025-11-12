# AI Prompts Used for Development

In accordance with the assignment instructions, this document records the AI prompts and interactions used to assist in the development of this application.

## 1. Project Initialization & Environment Setup
- "What are the recommended tools for building a Cloudflare AI app with memory and user input?"
- "How do I use `npm create cloudflare` with the `agents-starter` template?"
- "How to fix PowerShell 'PSSecurityException' when running `npx wrangler login`?"

## 2. Backend Logic (Durable Objects & Workers AI)
- "Where is the Durable Object code located in the starter template?"
- "How to modify the System Prompt to create a specific persona?"
- "Refactor the agent to act as a 'Job Interview Assistant' that asks questions one by one."
- "Is there an issue with importing `createWorkersAI` at the top level of the file? How to fix scope issues?"
- "How to switch the AI model to Llama 3.3 (`@cf/meta/llama-3.3-70b-instruct-fp8-fast`)?"

## 3. Debugging & Troubleshooting
- "How to fix `ReferenceError: env is not defined` when accessing environment variables?"
- "Troubleshooting `InferenceUpstreamError` (internal error) when running locally vs deploying."
- "How to handle TypeScript errors when the Llama 3.3 model ID is not assignable to `TextGenerationModels`?"
- "How to define and register a `workers.dev` subdomain for deployment?"

## 4. Frontend Customization (React & Tailwind)
- "Which files control the frontend UI in the agents-starter template?"
- "Modify `App.tsx`, `index.html`, and `styles.css` to change the branding to 'Cloudflare Interview Assistant'."
- "Change the color theme from orange to a professional blue/white style."
- "Remove the 'OpenAI API Key Not Configured' warning component."
- "Generate a custom SVG component for an 'AI Interviewer' icon using Phosphor Icons."