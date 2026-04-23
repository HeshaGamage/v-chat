# 🚗 Sri Lankan Vehicle Search Bot

A Telegram bot built with n8n that searches vehicles 
across Riyasewana.lk and ikman.lk simultaneously.

⚠️ Disclaimer: This project is for educational/personal use only.
Users are responsible for complying with the Terms of Service 
of any websites they interact with.

## Features
- 🔍 Natural language vehicle search via Telegram
- 🚗 Results from Riyasewana.lk
- 🏪 Results from ikman.lk
- 💰 Shows price and direct listing links
- 🤖 AI-powered search parameter extraction

## Example Queries
- "I need a Toyota Prado under 35 million"
- "Brand new Honda Vezel diesel"
- "Toyota Vitz under 8 million under 50000 km"
- "Used Mitsubishi Lancer registered"

## Tech Stack
- [n8n](https://n8n.io) - Workflow automation
- [Groq](https://groq.com) - AI (LLaMA model)
- [ScrapeNinja](https://scrapeninja.net) - Web scraping
- [Telegram Bot API](https://core.telegram.org/bots/api)

## How It Works
1. User sends vehicle request to Telegram bot
2. Groq AI extracts brand, model, price, mileage, condition
3. n8n builds search URLs for both sites
4. ScrapeNinja scrapes live listings
5. Results sent back with prices and links

## Setup Instructions
1. Import `workflow.json` into your n8n instance
2. Create credentials for:
   - Telegram Bot API
   - Groq API
   - ScrapeNinja API
3. Activate the workflow
4. Message your bot on Telegram!
