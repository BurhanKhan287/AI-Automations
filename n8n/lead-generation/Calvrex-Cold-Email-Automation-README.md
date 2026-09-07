# Calvrex Cold Email Automation

An end-to-end B2B cold email automation workflow built with n8n for sourcing, enriching, filtering, and contacting salon leads.

## What It Does

- Pulls existing salon leads from Google Sheets
- Scrapes additional salon locations using Apify
- Filters leads based on booking-platform usage
- Extracts publicly available website email addresses
- Checks and manages lead outreach status
- Prevents duplicate outreach
- Sends cold emails and follow-ups through SMTP
- Updates lead records and sent dates in Google Sheets
- Supports automated follow-up sequencing

## Workflow Stack

- **n8n** — Workflow orchestration
- **Google Sheets** — Lead database and outreach tracking
- **Apify** — Lead/location scraping
- **SMTP** — Email delivery

## Setup

Before importing and running this workflow, configure your own:

- Google Sheets credentials
- Apify API token
- SMTP credentials
- Google Sheets/document IDs
- Target scraping parameters
- Email templates and follow-up timing

The exported workflow contains placeholders instead of private API tokens.

## Security

This repository version has been sanitized for public sharing. Pinned/test execution data and the original Apify API token have been removed.

**Never commit API keys, passwords, OAuth tokens, or other credentials to GitHub.**

## Import

1. Open n8n.
2. Select **Import from File**.
3. Select `calvrex-cold-email-automation-sanitized.json`.
4. Configure your credentials and environment-specific values.
5. Test the workflow before enabling production execution.
