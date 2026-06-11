# 05. Content architecture

How pages connect, reinforce each other, and form a topical authority cluster. AI engines reward depth on a topic, not breadth across unrelated topics.

## Checklist

### Topic clusters

- [ ] Pick 3 to 5 core topics your brand wants to own
- [ ] Each core topic has a pillar page (2000+ words, covers the topic deeply)
- [ ] Each pillar has 8 to 15 supporting articles linking back to it
- [ ] Pillar links out to every supporter; every supporter links back to pillar
- [ ] No orphan articles disconnected from any cluster

### Internal linking

- [ ] Anchor text uses the target page's primary keyword phrase
- [ ] No two pages compete for the same primary keyword
- [ ] Related-articles section at the bottom of every post
- [ ] Breadcrumb navigation on every non-homepage page
- [ ] Breadcrumbs marked up with `BreadcrumbList` schema

### URL structure

- [ ] URLs use lowercase, hyphens, no underscores
- [ ] URLs match the H1 conceptually
- [ ] No date in the URL for evergreen content (`/post-title` not `/2023/03/post-title`)
- [ ] Trailing slash policy is consistent across the site
- [ ] No URLs over 60 characters where avoidable

### Canonicalization

- [ ] Every page has a `<link rel="canonical">` to itself
- [ ] Duplicate content (filter pages, paginated pages) canonicalizes to the master
- [ ] WWW vs non-WWW redirects to one version
- [ ] HTTP redirects to HTTPS

### Content freshness

- [ ] Top-20 traffic pages reviewed at least every 6 months
- [ ] `dateModified` updated when content actually changes (not for typos)
- [ ] Outdated stats refreshed annually
- [ ] Comparison tables checked monthly if competitors update prices

## Pillar structure example

```
Pillar: "Complete guide to BYOK SaaS"
  -> What is BYOK
  -> How to set up an OpenAI API key
  -> How to set up a Claude API key
  -> How to set up a DeepSeek API key
  -> BYOK vs bundled pricing comparison
  -> 20 BYOK tools we recommend
  -> Security best practices for API keys
  -> When BYOK is wrong (anti-recommendation)
  -> BYOK pricing math
  -> Migrating from bundled to BYOK
```

Each supporter is 800 to 1500 words, focused on its sub-topic. The pillar is 2500 to 4000 words and links to every supporter inline (not just in a TOC).

## Audit procedure

1. List every page on your site by URL.
2. For each, identify which topic cluster it belongs to. Pages that don't fit a cluster are flagged.
3. For each pillar candidate, count inbound internal links from supporters. Under 5 = thin pillar; rewrite supporters to link more naturally.
4. For each supporter, check it links to its pillar in the first 200 words.

## Pass criteria

- 90% of content pages belong to a defined cluster
- Every pillar page has 8+ supporters linking back
- Every supporter links to its pillar
- Zero orphan pages

## Common failures

- 200 blog posts on 200 unrelated topics. No topical authority anywhere.
- Pillar page exists but supporters link to the homepage instead of the pillar.
- Two articles compete for the same keyword (cannibalization). Pick one, redirect the other.
- "Recent posts" widget links chronologically, not by topic. Replace with related-by-cluster.

## Next

Move to `06-monitoring.md`.
