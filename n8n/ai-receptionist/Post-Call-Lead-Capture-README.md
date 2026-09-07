# Post-Call Lead Capture

An n8n workflow that processes post-call information from an AI receptionist and stores structured lead, appointment, and call data across Supabase and Notion.

## What It Does

- Receives post-call data through an ElevenLabs webhook
- Extracts caller and appointment information
- Handles missing or incomplete fields
- Processes booked appointments and inquiries
- Stores lead and appointment information in Supabase
- Creates or updates corresponding Notion records
- Handles appointment cancellations
- Stores call logs, transcripts, and related metadata in Supabase

## Workflow Stack

- **n8n** — Workflow orchestration
- **ElevenLabs** — AI receptionist and post-call data source
- **Supabase** — Structured database for leads, appointments, and call data
- **Notion** — Lead/appointment record management

## Setup

Before importing and running this workflow, configure your own:

- ElevenLabs webhook configuration
- Supabase credentials
- Supabase project/table references
- Notion credentials
- Notion database/page references
- Any environment-specific webhook or API settings

The workflow is intended to be connected to your own accounts and infrastructure.

## Security

This repository version has been sanitized for public sharing. Real pinned/test call payloads have been removed to prevent publishing private caller and appointment information.

**Never commit API keys, passwords, OAuth tokens, caller information, transcripts, or other private data to GitHub.**

## Import

1. Open n8n.
2. Select **Import from File**.
3. Select `post-call-lead-capture-sanitized.json`.
4. Connect your own ElevenLabs, Supabase, and Notion credentials.
5. Verify the database and Notion mappings.
6. Test with a non-sensitive test call before enabling production execution.
