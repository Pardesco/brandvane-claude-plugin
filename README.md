# Brandvane for Claude Code and Cowork

Turn SEO evidence into a clear next step. This plugin combines five focused skills with the [Brandvane](https://brandvane.ai) hosted MCP service.

Submitted to the Claude plugin directory for review; not yet approved. Package validation has passed. The bundled OAuth connection still awaits deployment of tested server compatibility changes and an installed-client acceptance run. Until those are complete, use the supplied-data workflows; do not assume live authentication is ready.

## What you can do

- **Find SEO opportunities:** prioritize actions from supplied or saved keyword and competitor evidence.
- **Write a content brief:** build an evidence-backed brief without inventing search volumes or rankings.
- **Explain AI visibility:** distinguish recorded AI mentions from fresh sampled answers.
- **Compare rankings:** explain changes between compatible saved Google snapshots.
- **Connect Brandvane:** set up OAuth and verify the connection with free reads and quotes.

The supplied-data workflows work without a Brandvane subscription. The example in [examples/keyword-report.md](examples/keyword-report.md) is synthetic and can be used without a Brandvane login. Claude plan and usage requirements remain separate.

## Install locally

For a reproducible, no-account example, follow the [five-minute demo](examples/walkthrough.md). It includes a synthetic input, a copyable prompt, an illustrative output, and checks for unsupported claims. No paid research is needed.

Clone this repository and start Claude Code with the plugin directory:

```sh
git clone https://github.com/Pardesco/brandvane-claude-plugin.git
claude --plugin-dir ./brandvane-claude-plugin
```

Use `/brandvane:seo-opportunities`, `/brandvane:content-brief`, `/brandvane:ai-evidence`, `/brandvane:rank-changes`, or `/brandvane:connect`. In Cowork, use its plugin interface to upload the packaged plugin when that option is available to your account. The plugin has been submitted through Console; no directory acceptance or verified badge is claimed.

## Connect the optional hosted service

The bundled server is `https://app.brandvane.ai/mcp`. In Claude Code, open `/mcp`, select the Brandvane server contributed by the plugin, and authenticate in the browser. In Cowork, use the connection controls shown for the plugin. Sign in to Brandvane with Google, confirm the selected workspace and callback host, and allow the connection. No API key or client secret belongs in this repository or in chat.

A connection to Claude Code returns to a loopback callback on your computer. Approve it only when you started the connection. The hosted Claude flow returns to claude.ai. If authentication fails, preserve the error and contact support; do not add wildcard callbacks or paste bearer tokens into URLs.

Start with:

> Show my Brandvane SEO credits and separate fresh AI allowance. Quote US keyword research for "AI SEO tools". Do not run paid research.

The keyword quote is five SEO credits for up to 25 results. An unsubscribed Brandvane account starts with zero credits.

## Costs and limits

The plugin source is free under MIT. Brandvane research is a separate service: SEO is $29/month with 900 SEO credits and five fresh AI checks; Pro+ is $59/month with 2,200 credits and 20 checks shared by an owner and one teammate. Check [current pricing](https://brandvane.ai/pricing/) before purchasing. Allowances do not roll over, and account or shared safety limits can pause new work.

Quotes and saved reads/exports are free. New SEO research consumes quoted credits. A fresh AI answer uses one separate AI unit. Optional weekly Google checks require explicit recurring approval and may run as soon as created. This plugin's skills do not enroll users in schedules. No payment, checkout, team management or account-deletion action is exposed by these skills.

After a lost response, recover the receipt by the original request key; never create a replacement paid request automatically.

## Privacy Policy

[Brandvane privacy policy](https://brandvane.ai/privacy/) describes the hosted service. Google provides sign-in, Cloudflare hosts the application, DataForSEO supplies SEO and recorded-mention data, and OpenAI supplies fresh AI answers. Stripe handles hosted billing outside the plugin.

Only inputs selected for tool calls are sent to Brandvane. The plugin does not request access to Google Drive or Gmail. Supplied documents remain in the user's Claude session unless the user explicitly requests a tool action that sends selected inputs. Claude processes that session under its own terms.

Saved research is private to the selected Brandvane workspace; Pro+ members share that workspace. Research retention is 90 days for SEO and 365 days for Pro+. Revoke the connection from Brandvane's account controls; removing the local plugin alone is not server-side revocation.

## Evidence and limitations

Provider search metrics are estimates. Google ranks are bounded snapshots. Recorded AI-source mentions and a fresh sampled answer describe different evidence. Missing coverage means unknown, not zero visibility. The plugin does not promise search rankings, backlinks, DR increases or AI recommendations.

## Review and development

Run `claude plugin validate --strict .`. See [REVIEW.md](REVIEW.md) for no-account and connected tests. There are no local executable hooks, background agents, bundled credentials or telemetry in this package.

Support: [support@brandvane.ai](mailto:support@brandvane.ai). [Service terms](https://brandvane.ai/terms/).
