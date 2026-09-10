---
name: ai-evidence
description: Explain Brandvane AI visibility evidence, keeping recorded AI-source mentions separate from fresh sampled answers and avoiding unsupported visibility scores.
---
Read ../../references/research-rules.md.

Establish the domain and which evidence the user wants explained. Supplied reports can be analyzed without a connection. Otherwise use seo_usage/seo_result for recorded mentions and seo_ai_usage/seo_ai_result for fresh answers. Use seo_visibility_report only with selected same-domain owned jobs; do not guess IDs.

For each conclusion, identify whether it came from provider-recorded source mentions, one fresh API answer, or the user's supplied material. Explain time, platform and query limitations. Empty coverage is not proof of no visibility. A fresh answer is not what every ChatGPT or Claude user sees. Do not compute a market-wide share-of-voice score from these samples.

If asked for new evidence, quote llm_mentions in SEO credits or seo_ai_quote in separate AI units according to the user's purpose. Fresh research needs approval. Suggest actions that follow from the evidence, and keep hypotheses distinct from observed facts. Do not promise that a change will cause AI recommendations.
