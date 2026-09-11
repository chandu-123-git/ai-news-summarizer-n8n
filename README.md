# AI News Summarizer with n8n

An AI-powered newsletter automation workflow built using **n8n, RSS feeds, SerpApi, Google Gemini, and Gmail**.

The workflow collects AI news, technology updates, and live event information, summarizes the content using AI, and delivers a daily newsletter directly to email.

## Workflow

```text
Schedule Trigger
       ↓
AI News RSS Feed ──────┐
                       │
Tech Updates RSS Feed ─┼──→ Data Merger → Aggregate
                       │                         ↓
SerpApi Events ────────┘                  Google Gemini
                                                 ↓
                                           Gmail Newsletter
```

## How It Works

1. The Schedule Trigger starts the workflow.
2. RSS feeds collect AI news and technology updates.
3. SerpApi searches Google for relevant AI and technology events.
4. The collected data is merged and aggregated.
5. Google Gemini summarizes the information into a newsletter.
6. Gmail sends the completed newsletter to the configured email address.

## Technologies Used

- **n8n** — Workflow automation
- **RSS Feeds** — News and technology updates
- **SerpApi** — Real-time Google search results
- **Google Gemini** — AI-powered summarization
- **Gmail** — Newsletter delivery

## Setup

1. Import the workflow JSON into n8n.
2. Configure the RSS feeds.
3. Configure your SerpApi API key.
4. Configure Google Gemini credentials.
5. Configure Gmail credentials.
6. Set the desired schedule.
7. Activate the workflow.

> API keys, credentials, and secrets are not included in this repository. Configure your own credentials when importing the workflow.

## Repository Contents

- `AI News Summarizer.json` — n8n workflow

## Author

**Chandu Sri Nellepalli**
