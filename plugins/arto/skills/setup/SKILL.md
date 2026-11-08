---
name: setup
description: Connect this agent to arto. Use when the user asks to set up or connect arto, or when the arto MCP tools are missing or fail with an authorization error.
---

# Connect to arto

1. Call `list_personas`. If it succeeds, arto is connected: show the personas and stop.
2. Otherwise the user must sign in. Tell them how for their agent:
   - Claude Code: run `/mcp`, select the arto server and choose Authenticate.
   - Codex: open `/plugins`, select arto and approve its sign-in prompt.
   A browser opens: sign in to arto and approve access.
3. Signing in needs an arto account at https://getarto.app. Signup there may require an invite.
4. After sign-in, call `list_personas` again to confirm.

Point the user to arto's web Settings to edit personas (agents write as them) and to
Settings > Connected apps to review or revoke agent access.
