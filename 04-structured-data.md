# 04. Structured data

Schema markup is the structured-data layer AI engines parse to disambiguate your content. Without it the engine guesses; with it the engine knows.

## Checklist

### Site-wide schema

- [ ] `Organization` or `LocalBusiness` schema on homepage
- [ ] Logo URL in `Organization` is square, 112x112 minimum, hosted on your domain
- [ ] `sameAs` array on Organization with all official social profiles
- [ ] Phone, email, and address present (if applicable)
- [ ] `WebSite` schema with `SearchAction` for site search

### Article and content pages

- [ ] Every blog post has `Article`, `NewsArticle`, or `BlogPosting` schema
- [ ] `headline` matches the `<h1>` exactly
- [ ] `image` references an absolute https URL, 1200x630 or similar
- [ ] `datePublished` and `dateModified` are ISO 8601
- [ ] `author` is a Person object (not just a string), with `url` and `sameAs`
- [ ] `publisher` is an Organization with logo

### Product and pricing pages

- [ ] `Product` or `SoftwareApplication` schema on every product page
- [ ] `offers` includes `price`, `priceCurrency`, `availability`, `url`
- [ ] `aggregateRating` only present if you have real reviews (no fakes)
- [ ] `review` schema for individual testimonials with `author.name`

### Local business pages

- [ ] `LocalBusiness` (or specific subtype: Restaurant, Dentist, etc) on contact page
- [ ] `address` is a `PostalAddress` object with all 5 fields
- [ ] `geo` has lat/lon for the actual address
- [ ] `openingHours` covers all days
- [ ] `priceRange` set ($, $$, $$$)

### FAQ pages

- [ ] `FAQPage` schema on dedicated FAQ pages
- [ ] Each question has `acceptedAnswer` with full text (not "see link")
- [ ] Questions match the visible H3 text on the page
- [ ] No fake or rewritten questions; use real user questions

### Video and course pages

- [ ] `VideoObject` for embedded videos with `thumbnailUrl`, `uploadDate`, `duration`
- [ ] Transcript in `transcript` field (AI engines parse this directly)
- [ ] `Course` schema on course landing pages with `provider` and `instructor`

## Tools

- [json-ld-markup-builder](https://github.com/0xelitesystem/json-ld-markup-builder): generate JSON-LD for 12 types
- [json-ld-business-examples](https://github.com/0xelitesystem/json-ld-business-examples): real-world JSON-LD examples to study
- Google Rich Results Test: validate every schema block before publishing
- Schema.org validator: catch issues the Google tool misses

## Audit procedure

1. List every page type (homepage, blog post, product, pricing, contact, FAQ, etc).
2. For each type, decide what schema applies.
3. View source for one representative page per type.
4. Check for the schema. If missing, generate with the schema markup generator.
5. Validate every block in Google Rich Results Test.
6. Roll out to all pages of that type.

## Pass criteria

- 100% of homepages have Organization or LocalBusiness schema
- 100% of article pages have Article schema with Person author
- 100% of product pages have Product or SoftwareApplication schema
- Zero Schema.org validator errors

## Common failures

- Schema present but `author` is a string ("John Smith") not a Person object. Validates as warning, AI ignores.
- `aggregateRating` with `ratingValue: 5` and `ratingCount: 1`. Looks fake. AI discounts.
- Multiple `@type` on the same page in conflict (Article + Product + BlogPosting). Pick one primary.
- Schema added but page text doesn't match (schema says "$99" but page says "$149"). AI flags mismatches.

## Next

Move to `05-content-architecture.md`.
