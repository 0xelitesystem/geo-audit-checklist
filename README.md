# geo-audit-checklist

A page-by-page checklist for auditing a site for AI engine citability. ChatGPT, Claude, Perplexity, Gemini, Google AI Overviews.

GEO = Generative Engine Optimization. The set of practices that get your content cited and surfaced by AI search engines, which is increasingly different from classic SEO.

## What this repo contains

- `README.md`: this file, with the audit philosophy
- [00-pre-audit.md](00-pre-audit.md): data you need before starting
- [01-discoverability.md](01-discoverability.md): can AI engines find and parse your site
- [02-passage-quality.md](02-passage-quality.md): are individual paragraphs citable
- [03-eeat-signals.md](03-eeat-signals.md): Experience, Expertise, Authoritativeness, Trust
- [04-structured-data.md](04-structured-data.md): schema markup audit
- [05-content-architecture.md](05-content-architecture.md): how pages connect and reinforce each other
- [06-monitoring.md](06-monitoring.md): how to know if it's working
- `playbook-saas.md`: GEO checklist tuned for a SaaS site
- `playbook-local-business.md`: GEO checklist tuned for a local business
- `playbook-blog.md`: GEO checklist tuned for an editorial/blog site
- `playbook-docs.md`: GEO checklist tuned for technical documentation
- `quick-wins.md`: 10 fixes that take under an hour each

## How to use

1. Read [00-pre-audit.md](00-pre-audit.md) first. You need referral logs and a current site map.
2. Pick the playbook closest to your site type.
3. Work through each section in order. Each item has pass/fail criteria.
4. Use the linked tools (built by 0xelitesystem) for the items that need them.

## Companion tools

| Section | Tool |
|---|---|
| Discoverability | [llms-txt-file-builder](https://github.com/0xelitesystem/llms-txt-file-builder), [robots-txt-ai-builder](https://github.com/0xelitesystem/robots-txt-ai-builder) |
| Passage quality | [ai-citability-scorer](https://github.com/0xelitesystem/ai-citability-scorer) |
| E-E-A-T signals | [page-trust-signals-auditor](https://github.com/0xelitesystem/page-trust-signals-auditor) |
| Structured data | [json-ld-markup-builder](https://github.com/0xelitesystem/json-ld-markup-builder), [json-ld-business-examples](https://github.com/0xelitesystem/json-ld-business-examples) |
| Monitoring | [brand-mention-playbook](https://github.com/0xelitesystem/brand-mention-playbook) |

## The core hypothesis

AI engines are passage retrievers, not document rankers. They pull chunks of 100 to 200 words out of pages and quote them. To be cited you need:

1. The chunk to be self-contained and fact-rich
2. The page to be discoverable by AI bots
3. The author and publisher to be identifiable
4. Other sites to mention you so the AI sees corroboration

This checklist covers all four.

## What this is NOT

- Not a guarantee. AI engines are opaque about why they cite what they cite.
- Not a one-time audit. Rerun quarterly; AI behavior shifts.
- Not a substitute for classic SEO. Run both. They overlap by about 60 percent and the parts that don't overlap are the high-leverage ones.

## More

Part of a catalog of single-file browser tools and plain-language references, all MIT licensed and dependency-free: [0xelitesystem.github.io](https://0xelitesystem.github.io/). Built by [elitesystem.ai](https://elitesystem.ai).

## License

MIT. Free to use, fork, adapt.
