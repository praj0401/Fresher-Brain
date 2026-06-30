# Fresher Brain — AI Career OS for Freshers

A free AI career coach for students and freshers hunting their first job. Resume parsing, mock interviews, JD analysis, real job matching, application tracking — all in a single HTML file with zero backend.

## Features

- **Resume parser** — upload a PDF or paste text, auto-fills your entire profile
- **10 dedicated chat modes** — resume review, recruiter review, salary intel, cold email, LinkedIn optimizer, salary negotiation, learning roadmap, weekly plan
- **JD Analyzer** — ATS score, keyword gaps, tailored resume rewrite, predicted interview questions
- **Mock Interview Engine** — resume-aware, JD-aware, scored on clarity/STAR/relevance/depth
- **Job Matches** — real, live job postings via Adzuna, not AI-generated
- **Company Prep Hub** — hiring process, interview stages, common questions per company
- **Application Tracker** — full pipeline board with follow-up reminders
- **Analytics** — interview score history, weak topic tracking

## How it works

No signup, no account, no server. Bring your own free API key (Groq recommended — no credit card needed) and everything runs client-side. Your data and API keys never leave your browser.

## Setup

1. Open the deployed site (or open `index.html` locally)
2. Go to Settings → add a free Groq key from [console.groq.com](https://console.groq.com)
3. Fill in your profile, or upload your resume to auto-fill it
4. Start using any feature

### Optional integrations (also free)

- **Serper** (web search) — grounds Company Hub and interview predictions in live data. Free key at [serper.dev](https://serper.dev)
- **Adzuna** (job search) — powers the Job Matches tab with real postings. Free key at [developer.adzuna.com](https://developer.adzuna.com)

## Deploy your own

This is a static site — deploys anywhere that serves HTML.

**Vercel (recommended):**
```bash
npm i -g vercel
vercel
```
Or connect this repo directly at [vercel.com/new](https://vercel.com/new).

## Tech

Single HTML file. No build step, no framework, no backend. Uses:
- [PDF.js](https://mozilla.github.io/pdf.js/) for client-side PDF text extraction
- LocalStorage for all persistence
- Direct browser fetch calls to OpenAI / Gemini / Groq / Serper / Adzuna APIs

## License

MIT — use it, fork it, ship it.
