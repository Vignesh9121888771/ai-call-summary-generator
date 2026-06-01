# AI Call Summary Generator

> GenAI Prototype #7 — Submitted for the Available GenAI Prototypes assignment

A single-page AI-powered tool that takes raw telecaller notes or call transcripts and automatically extracts structured CRM-ready summaries using the Claude API.

---

## What It Does

Telecallers and sales teams often write messy, unstructured notes after calls. This tool converts those notes into a clean, structured summary with:

| Field | Description |
|---|---|
| **Client** | Name and company |
| **Requirement** | What the client needs (1–2 sentences) |
| **Interest Level** | Hot / Warm / Cold |
| **Budget** | Stated budget or "Not mentioned" |
| **Timeline** | Expected deadline or "Not mentioned" |
| **Objection** | Main hesitation or blocker |
| **Next Action** | Clear next step for the team |
| **Priority** | High / Medium / Low |

The output is one-click copyable for pasting directly into any CRM.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Vanilla HTML, CSS, JavaScript |
| AI Model | Claude claude-sonnet-4-20250514 (Anthropic) |
| AI Technique | Prompt engineering — structured JSON output |
| Hosting | Netlify / Vercel (static file) |

**Skills demonstrated:** LLMs, prompt engineering, JSON structured output, text summarisation

---

## How to Run Locally

1. Clone this repo:
   ```bash
   git clone https://github.com/YOUR_USERNAME/ai-call-summary-generator.git
   cd ai-call-summary-generator
   ```

2. Open `index.html` directly in your browser — no build step, no dependencies.

3. The API key is handled by the Claude.ai sandbox when running inside Claude artifacts. For standalone deployment, add your Anthropic API key:
   - Open `index.html`
   - Find the `fetch` call to `https://api.anthropic.com/v1/messages`
   - Add your key to the headers: `'x-api-key': 'YOUR_API_KEY_HERE'`

   > ⚠ Never commit your API key. Use environment variables or a backend proxy for production.

---

## Deploy to Netlify (Free, 30 seconds)

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag and drop the `index.html` file
3. Your live URL is ready instantly

---

## Project Structure

```
ai-call-summary-generator/
├── index.html      # Complete app (HTML + CSS + JS in one file)
└── README.md       # This file
```

---

## Example Inputs

**Hot lead:**
> Called Priya from StyleMart, she's launching an online clothing store. Needs a full e-commerce website with Razorpay integration. Budget is 1.5 lakh, wants to go live before Diwali. Asked for a detailed quote. Follow up Thursday.

**Cold call:**
> Cold call to Sanjay at BuildPro. Polite but busy. Old website, no budget allocated yet, not deciding for 3–4 months. Call back in January.

**Support issue:**
> Support call from Ananya, existing client. Contact form not sending emails since yesterday. SMTP issue after server migration. Escalated to backend team. ETA 4 hours. Ticket #4421.

---

## Submission Details

- **Student:** Vignesh
- **Registration No.:** 252U1R6030
- **Section:** 1A — AIML
- **Institution:** Aurora's Higher Education and Research Academy

---

## License

MIT — free to use and modify.
