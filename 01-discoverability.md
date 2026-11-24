# 01. Discoverability

Can AI engines find and parse your site? If no, nothing else matters.

## Checklist

### robots.txt

- [ ] `robots.txt` exists at `yoursite.com/robots.txt`
- [ ] It does NOT block AI bots you want to allow (GPTBot, ClaudeBot, PerplexityBot, etc)
- [ ] It DOES block AI bots you want to exclude (Bytespider, CCBot for some sites)
- [ ] `Sitemap:` directive points to your sitemap.xml
- [ ] `Sitemap:` directive points to your llms.txt (optional but recommended)
- [ ] All 17 named AI bots have an explicit rule, not just `User-agent: *`

Use [robots-txt-ai-builder](https://github.com/0xelitesystem/robots-txt-ai-builder) to generate this.

### sitemap.xml

- [ ] `sitemap.xml` exists and is reachable
- [ ] All canonical pages are listed
- [ ] No 404 or 301 URLs in the sitemap
- [ ] `<lastmod>` is set and accurate (not all the same date)
- [ ] Sitemap is under 50,000 URLs and 50 MB (or split into sub-sitemaps)
- [ ] Submitted to Google Search Console and Bing Webmaster Tools

### llms.txt

- [ ] `llms.txt` exists at site root (or planned)
- [ ] Lists 10 to 30 of your most important pages
- [ ] Every link has a specific description (not "Docs" or "About")
- [ ] Grouped into logical sections (Products, Reference, Pricing, etc)
- [ ] Tagline and brand paragraph are concrete, not adjectives

Use [llms-txt-file-builder](https://github.com/0xelitesystem/llms-txt-file-builder).

### Page-level basics

- [ ] All pages return 200 status (no soft 404s on important pages)
- [ ] Server responds in under 800ms for AI bot user agents
- [ ] No login wall on pages you want indexed
- [ ] No infinite scroll on content-heavy pages (or implement pushState)
- [ ] No JavaScript-only rendering for primary content (AI bots vary in JS support)

### Internal linking

- [ ] Every important page is reachable from the homepage in 3 clicks or fewer
- [ ] Anchor text uses descriptive nouns ("BYOK pricing study") not "click here"
- [ ] Footer or sidebar links to llms.txt and sitemap.xml
- [ ] No orphan pages (pages with zero inbound internal links)

## Pass criteria

- 90% of items checked
- Logs show at least 3 named AI bots fetching pages in the last 30 days
- All top-20 traffic pages return 200 to AI bot user agents

## Common failures

- Site blocks all bots except Googlebot (legacy `User-agent: *` `Disallow: /`)
- Sitemap last updated 2 years ago
- llms.txt is missing entirely
- Pages render content only after JavaScript executes; bots see empty shells

## Next

Move to `02-passage-quality.md`.
