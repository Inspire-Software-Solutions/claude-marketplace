# Inspire Plugin for Claude

Connect Claude to Inspire Software to create objectives, give recognition, and use AI-assisted performance workflows — without leaving your Claude conversation.

## What's included

**MCP Connectors**

| Connector | Purpose |
|-----------|---------|
| `inspire` | Read access — objectives, check-ins, 1-1 agendas, roles |
| `inspire-actions` | Write access — create objectives, save check-ins, give recognition |

**Skills**

| Skill | Trigger phrases |
|-------|----------------|
| Create objective | "create an objective", "add a new OKR", "set up a goal in Inspire" |
| Suggest recognition | "give recognition", "recognize a teammate", "send kudos", "suggest who to recognize" |

## Setup

Each client authenticates via OAuth 2.0. When you first use an Inspire tool, Claude will prompt you to connect your Inspire account.

No environment variables required — authentication is handled through the OAuth flow.

## Before releasing to production

The MCP URLs in `.mcp.json` currently point to the **staging** environment:

```
https://inspire-mcp-apim.azure-api.net/staging/mcp
https://inspire-mcp-apim.azure-api.net/staging/actions/mcp
```

Before distributing to production clients, update these to your production URLs.

## Usage

Once installed, clients can say things like:

- "Create an objective for Q3 focused on customer retention"
- "I want to recognize Sarah for shipping the new dashboard ahead of schedule"
- "Help me write a check-in for my growth objective"

## Adding more skills

This plugin is designed to grow. To add new skills, create a new subdirectory under `skills/` with a `SKILL.md` file following the existing pattern.
