# PromptEvaluator

A small Prompt Evaluator app (Express backend + static frontend) to grade model outputs against prompts/references using a heuristic scorer or an optional OpenAI-based evaluator.

Features
- Heuristic scoring (local, no API key needed)
- Optional LLM-based scoring using OpenAI (set OPENAI_API_KEY)
- Simple web UI for entering prompt, reference, and receiving a score + breakdown

Quickstart
1. Clone the repo
2. Install:
   npm install
3. Copy .env.example to .env and set OPENAI_API_KEY if you want LLM scoring
4. Start:
   npm run dev
5. Open http://localhost:3000

Files added
- server.js (Express API + evaluator)
- package.json
- public/index.html, public/app.js, public/style.css
- .env.example
- .gitignore

Notes
- This is a starter implementation; extend the heuristic or the evaluation prompt to fit your needs.