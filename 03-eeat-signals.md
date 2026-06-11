# 03. E-E-A-T signals

Experience, Expertise, Authoritativeness, Trust. Google introduced E-A-T in 2014, added the second E (Experience) in 2022. AI engines weight these signals similarly when deciding what to cite.

## Checklist

### Experience signals

- [ ] First-person language present ("I", "we", "our") on guide pages
- [ ] Concrete numbers in each major claim
- [ ] Case study or example phrases ("for example", "in practice", "last quarter")
- [ ] Original screenshots, original photos, or original data charts (not stock)

### Expertise signals

- [ ] Visible author byline at top of every content page
- [ ] Author bio section or link to dedicated author page
- [ ] Substantial content depth (500+ words for blog posts, 1500+ for guides)
- [ ] Credentials stated where relevant ("CFA", "MD", "15 years building APIs")

### Authoritativeness signals

- [ ] Person schema for every author
- [ ] Article schema with `author` pointing to the Person
- [ ] `sameAs` array in Person schema with 3+ profile URLs (GitHub, LinkedIn, Twitter, personal site)
- [ ] Outbound citations to primary sources (3+ per long-form page)
- [ ] Pages get inbound links from third-party sites in your niche

### Trust signals

- [ ] `datePublished` in schema for every article
- [ ] `dateModified` updated when content is revised (not just typo fixes)
- [ ] Visible date in the page header (not buried in the footer)
- [ ] Contact link in header or footer
- [ ] Publisher organization named in schema
- [ ] About page exists and is linked from every page

## Tool

Run any page's HTML through [e-e-a-t-auditor](https://github.com/0xelitesystem/e-e-a-t-auditor) for a scored breakdown across all 13 checks.

## Audit procedure

1. Pick the top 10 traffic pages.
2. View source, copy HTML.
3. Run each through the E-E-A-T auditor.
4. Pages scoring under 50 are restructured (add byline, add schema, add dates).
5. Pages scoring 50-74 get the failing individual checks addressed.
6. Pages scoring 75+ are templates for the rest of the site.

## Pass criteria

- Every content page has a visible byline linking to an author page
- Every content page has Article + Person schema
- 100% of articles have `datePublished` and `dateModified`
- Top-10 pages score 70+ in the E-E-A-T auditor

## Common failures

- Anonymous content. AI engines (and Google) discount anonymous pages heavily.
- Author page exists but has no `sameAs` profile links; the author looks unverifiable.
- Schema is present but the author field is just `"Admin"` or `"Editor"`.
- Last updated 2021 but the page reads "as of this year". AI engines clock the staleness.
- No outbound citations. Looks like an opinion piece even when it's research.

## Next

Move to `04-structured-data.md`.
