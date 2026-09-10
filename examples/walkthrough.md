# Five-minute SEO opportunity demo

This walkthrough uses fabricated data, not a customer report or a measured Brandvane result. It demonstrates the supplied-data workflow without a Brandvane account, connection, or research charge. Claude's own access and usage requirements are separate.

## 1. Load the plugin

Follow the [local installation instructions](../README.md#install-locally), then open [keyword-report.md](keyword-report.md) in the same Claude session. If a connection prompt appears, skip authentication for this demo.

## 2. Run this prompt

```text
/brandvane:seo-opportunities
Use examples/keyword-report.md as the only evidence. It contains synthetic data.
Recommend the first educational article for solo marketing consultants.
Explain the tradeoffs and missing evidence. Do not connect to Brandvane,
call external tools, or run paid research.
```

## 3. Compare the response with this illustrative reasoning

This is an authored example, not a captured or guaranteed Claude response:

> A reasonable first article is "How to track ChatGPT referrals in GA4."
> The supplied synthetic report gives that topic 260 estimated monthly searches
> and difficulty 18, compared with 1,900 and 62 for "AI visibility tools."
> The narrower how-to topic fits consultants who need an actionable reporting
> task. "AI referral traffic report" is another plausible starting point with
> lower illustrative difficulty, but less illustrative demand.
>
> These fabricated estimates cannot establish a real ranking opportunity.
> We still need actual search results, audience evidence, existing content,
> and conversion goals before committing a production content plan.

A different first choice can be valid when its reasoning stays within the evidence. Do not interpret the example as a ranking prediction or a validated keyword recommendation.

## 4. Turn the evidence into a brief

```text
/brandvane:content-brief
Using the same synthetic report, draft a brief for the selected topic:
audience, reader problem, proposed outline, and questions to verify.
Mark assumptions. Do not invent metrics, existing URLs, or product results.
Do not publish content or use external tools.
```

## Acceptance checklist

- The response labels the input as synthetic.
- Every metric comes from the supplied three-row report.
- Missing rankings, conversion data, and site content remain unknown.
- No authentication, external tool call, paid job, or publication occurs.
- The brief is an editable proposal, not a claim of measured success.

For real research, see [Brandvane](https://brandvane.ai) and the [connection and cost disclosures](../README.md#connect-the-optional-hosted-service). Connected acceptance is tracked separately in [REVIEW.md](../REVIEW.md).
