---
name: connect
description: Set up or troubleshoot this plugin's Brandvane MCP connection in Claude Code or Cowork and verify it with free balance reads and a quote.
---
Use the plugin's bundled Brandvane server at https://app.brandvane.ai/mcp. Read ../../references/research-rules.md before calling its tools.

Guide the user to the client's MCP/plugin connection controls. In Claude Code, /mcp lists the plugin server and its authentication action. Have the user complete Google sign-in and Brandvane workspace consent in their browser. Never request a Google password, session cookie, API key or bearer token in chat.

For Claude Code, explain that the callback returns to an application on the user's computer; for hosted Claude it returns to claude.ai. Do not change redirect configuration to work around an error. Report the actual error and the support address support@brandvane.ai when configuration needs investigation.

After connection, call seo_balance and seo_ai_allowance. If the user wants a no-spend demonstration, call seo_quote for keyword_research with keyword "AI SEO tools", location_code 2840 and language_code en. Explain the five-credit, 25-row ceiling. Do not execute the paid request as part of setup.

A zero balance or absent AI period on an unsubscribed account is not a broken connection. Supplied-data skills can still work without a subscription. For removal, explain both uninstalling the plugin and revoking its connection in Brandvane; one does not imply the other.
