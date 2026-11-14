# 06. Monitoring

How to know if your GEO work is paying off. AI engines do not give you analytics dashboards, so you have to build the signal yourself.

## Checklist

### Brand mention tracking

- [ ] Google Alerts set up for brand name (exact match)
- [ ] Google Alerts set up for "yourbrand alternative" and "yourbrand vs"
- [ ] Talkwalker Alerts or Mention.com as backup (catches mentions Google misses)
- [ ] Monthly review of new mentions logged in a spreadsheet

See [brand-mention-playbook](https://github.com/0xelitesystem/brand-mention-playbook) for templates.

### AI engine direct test

- [ ] Monthly recurring test: ask ChatGPT, Claude, Perplexity, Gemini your 5 baseline prompts
- [ ] Track in a spreadsheet: which engine, which prompt, were you mentioned, were you cited by URL
- [ ] Compare against the same prompts about your top 3 competitors

### Server logs

- [ ] Weekly review of AI bot hits in server logs
- [ ] Track which pages each bot fetches most
- [ ] Track new AI bots that appear (the list grows)
- [ ] Alert if any AI bot drops to zero hits for 30 days

### Search Console

- [ ] Track impressions and clicks for branded queries
- [ ] Track CTR for AI Overview-eligible queries
- [ ] Note when impressions rise but clicks fall (AI Overview is summarizing without driving traffic)

### Bing Webmaster Tools

- [ ] Track Bingbot crawl rate; Bing powers Copilot
- [ ] Submit sitemap to Bing as well as Google

## Quarterly metrics worth tracking

| Metric | What it tells you |
|---|---|
| Number of AI bot hits per month | Discoverability |
| Number of brand mentions per month | Authority signal AI engines pick up |
| Number of times cited by URL in AI engines | Direct citation success |
| Number of times mentioned by brand name in AI engines | Brand recognition even without citation |
| Number of pages with E-E-A-T score over 70 | Internal quality |
| Number of pages with citability score over 70 | Internal quality |

## What NOT to obsess over

- Exact rank in AI engine answers. The engine reranks per query; no stable position.
- Page count in sitemap. More pages is not better; better pages is better.
- Schema validation errors on third-party widgets you don't control. Fix what you can.

## The 90-day rhythm

- Month 1: Implement changes
- Month 2: Wait. AI engines re-crawl on their own schedule.
- Month 3: Rerun the baseline AI engine tests. Compare against month 0.

GEO is a 90-day feedback loop, not a 7-day one. Patience.

## Companion tool

[brand-mention-playbook](https://github.com/0xelitesystem/brand-mention-playbook) has the spreadsheet templates for everything in this section.

## You're done

You have a baseline. Rerun this checklist quarterly.
