# Inspire Plugin for Claude

Connect Claude to your Inspire account to read your data and create new records directly from your Claude conversation. NOTE: Only available to current Inspire licensed users using Microsoft 365 (Entra Id).

## What's included

**MCP Connectors**

| Connector | Purpose |
|-----------|----------|
| `inspire` | Read access — objectives, check-ins, 1-1 agendas, roles |
| `inspire-actions` | Write access — create objectives, save check-ins, give recognition |

## Setup

Authentication is handled via OAuth 2.0. When you first use an Inspire tool, Claude will prompt you to connect your Inspire account. No environment variables required.

## Usage

Once installed, just ask Claude naturally:

- "Show me my objectives for this quarter"
- "Add a check-in to my growth objective"
- "Who on my team has a 1-1 this week?"
