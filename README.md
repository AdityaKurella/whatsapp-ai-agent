# WhatsApp AI Agent

An n8n workflow for a WhatsApp assistant that handles text, image, and audio messages, can search the web and calculate, and can retrieve context from a Pinecone knowledge base.

## Included workflow

- `WhatsApp_Agent.json` — 27-node workflow export.

## Requirements

- n8n with the WhatsApp Business Cloud, OpenAI, SERP API, Pinecone, and HTTP Header Auth integrations available.
- WhatsApp Business Cloud app, phone number, and webhook configured for your n8n instance.
- Pinecone index and any required MCP server endpoint.

## Import and configure

1. Import `WhatsApp_Agent.json` into n8n.
2. Create and assign credentials for WhatsApp, OpenAI, SERP API, Pinecone, and the authenticated media-download requests. The exported credential bindings were removed; select your own credentials on the affected nodes.
3. Set your WhatsApp phone number ID, recipient/test destination, media API endpoint, Pinecone index, and MCP server endpoint.
4. Configure the WhatsApp webhook with Meta and activate the workflow only after testing in your environment.

The exported webhook and provider IDs have been regenerated or replaced with setup placeholders.

## Notes

This repository contains a sanitized workflow export, not provider credentials, a Pinecone index, an MCP server, or a hosted n8n instance. Review each node and provider requirements before enabling live messaging.

