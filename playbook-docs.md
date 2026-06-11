# Playbook: Technical documentation

Tuning the full GEO checklist for technical documentation (developer docs, API references, SDK guides).

## Highest-impact items

1. **llms.txt with every major doc page listed and specifically described.** Devs and AI engines both use it.
2. **llms-full.txt with concatenated markdown of all reference pages.** This is the killer feature for docs sites.
3. **Self-contained code examples.** Every code block runs as-is, no "see imports above" references.
4. **Clear navigation hierarchy.** AI bots crawl the sidebar; bad nav = missed pages.
5. **HowTo schema on tutorial pages** with `step` array including code.

## Lower priority

- LocalBusiness schema (skip)
- Person schema for engineers (only for senior public-facing devs)
- Article schema on reference pages (use TechArticle or skip)

## Docs-specific paragraphs

- Each function/method reference: one sentence describing what it does, one showing signature, one example, one note on errors
- Tutorials: numbered steps, each with code + expected output
- Concept docs: one definition paragraph, one paragraph on when to use, one on common gotchas

## Docs-specific E-E-A-T

- "Last updated" visible on every page
- "Edit this page on GitHub" link (proves the docs are real and maintainable)
- Author of the SDK or library is named on the homepage
- Changelog links from version-specific pages

## Common docs mistakes

- Code examples assume context from earlier examples on the page; AI extracts one block and it breaks
- "Click here" links instead of "see the authentication guide"
- Documentation framework auto-generates pages with no real content
- Reference docs are auto-generated from source comments that are themselves bad
- No llms.txt (worst miss for docs specifically)
