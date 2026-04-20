# SA Flow

## Overview

A large-scale Sales Automation flow for conference exhibitor lead generation. It scrapes exhibitor data from MapYourShow event pages via Apify, uses AI to find missing company domains, enriches organizations through Apollo, applies ICP filtering, searches for marketing decision-makers, cleans and deduplicates leads, saves to dynamically created Google Sheets, and pushes qualified leads to Aimfox LinkedIn and Instantly email campaigns. This is one of the most comprehensive lead generation pipelines in the collection.

## How It Works

```
Form (event URL) -> Apify MapYourShow Scraper -> Clean exhibitor data -> AI find domains -> Apollo Org Enrichment -> ICP Filter -> Apollo People Search -> Clean + Deduplicate -> Create Google Sheet -> Save leads -> Aimfox + Instantly campaigns
```

## Integrations

- **Apify** - MapYourShow exhibitor scraping
- **OpenAI** - Domain research and ICP analysis
- **Apollo** - Organization enrichment and people search
- **Google Sheets** - Dynamic lead storage
- **Aimfox** - LinkedIn outreach
- **Instantly** - Email outreach

## Setup

1. Import `SA_Flow.json` into your n8n instance.
2. Configure all credentials.
3. Activate and submit the form with an event URL.
