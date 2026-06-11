# 00. Pre-audit data gathering

Before you start auditing, collect this data. Without it the audit produces guesses.

## Required data

| Item | Where to get it | Why |
|---|---|---|
| Last 90 days of referral logs | Server logs, Cloudflare analytics, or any log aggregator | To see which AI bots actually visit your site and which pages they fetch |
| Current sitemap.xml | yoursite.com/sitemap.xml | To know what you are claiming to publish |
| Current robots.txt | yoursite.com/robots.txt | To know what you are currently allowing/blocking |
| Top 20 pages by traffic | Analytics tool | These are the pages worth optimizing first |
| Top 20 pages by inbound links | Ahrefs, Moz, or any backlink tool | Strong inbound link signals raise everything else |
| Current Search Console performance | Google Search Console | Compare classic search position to AI citation rate |

## Optional but valuable

| Item | Why |
|---|---|
| Bing Webmaster Tools data | Bing powers Copilot, so this is a direct AI signal |
| Brand mention scrape (last 6 months) | Use [brand-mention-tracker](https://github.com/0xelitesystem/brand-mention-tracker) to set this up |
| Manual AI engine test results | Ask ChatGPT, Claude, Perplexity, Gemini about your brand and topics; save the answers |

## How to identify AI bots in logs

Search your logs for these user-agent strings:

```
GPTBot
OAI-SearchBot
ChatGPT-User
ClaudeBot
Claude-Web
anthropic-ai
PerplexityBot
Perplexity-User
Google-Extended
Applebot-Extended
CCBot
Meta-ExternalAgent
Bytespider
Amazonbot
FacebookBot
DuckAssistBot
```

If you see zero hits across 90 days, your site is not being crawled by AI engines. Discoverability is your first problem; see `01-discoverability.md`.

If you see hits but the bots are only fetching `/robots.txt` and not deeper pages, your sitemap or internal linking is the issue.

## Baseline test: ask the AI engines

Spend 30 minutes asking each engine these prompts about your brand:

1. "What is [your brand]?"
2. "Best [your category] for [your audience]?"
3. "How does [your brand] compare to [competitor]?"
4. "Who is the founder of [your brand]?"
5. "What does [your brand] do that [competitor] doesn't?"

Save the answers. Note:
- Were you mentioned at all?
- Was the information correct?
- Were you cited by URL?
- Were competitors cited but you weren't?

Repeat this test after each round of changes. This is your ground truth.

## Next

Move to `01-discoverability.md`.
