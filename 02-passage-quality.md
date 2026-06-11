# 02. Passage quality

AI engines retrieve and quote passages of 100 to 200 words. They do not quote whole pages. Each paragraph on your important pages has to stand on its own.

## Checklist

### Structure

- [ ] Each H2 section answers a complete question
- [ ] Paragraphs under each H2 are 100 to 220 words (target 134 to 167)
- [ ] First paragraph in each section makes the claim before explaining it
- [ ] Definitions appear immediately after the term, not later

### Self-containment

- [ ] No "as mentioned above", "see below", "in the previous section" inside paragraphs
- [ ] Acronyms are spelled out on first use within each section, not just once on the page
- [ ] Subject is named in every sentence (replace "it", "this", "that" with the actual noun)

### Specificity

- [ ] At least one number, date, or named entity per paragraph on key pages
- [ ] Claims have sources: "per [Study] (2026)" or "[Expert] reported"
- [ ] No empty adjectives: cut "innovative", "robust", "world-class", "leading"
- [ ] No filler openers: cut "in today's world", "there are many", "when it comes to"

### Format

- [ ] Tables for comparisons (price, feature, version)
- [ ] Numbered lists for procedures
- [ ] Bullet lists for non-ordered items
- [ ] Code blocks for code (no inline `code` for multi-line)
- [ ] One topic per paragraph

## Tool

Run any paragraph through [ai-citability-scorer](https://github.com/0xelitesystem/ai-citability-scorer) before publishing. Target 70+ on the 100-point scale.

## Audit procedure

1. Open your top-20 traffic pages.
2. Score the first 3 paragraphs of each in the citability scorer.
3. Average score per page = page citability.
4. Pages averaging below 50 get rewritten.
5. Pages averaging 50-69 get edits to fix specific failing checks.
6. Pages averaging 70+ are left alone.

## Pass criteria

- Top-20 pages average over 65 on the citability scorer
- Zero paragraphs use "as mentioned above" or similar intra-doc references
- Zero filler-opener paragraphs on the homepage and pricing page

## Common failures

- Author thinks the audience reads pages top-to-bottom; writes "as we covered above". AI engines extract bottom-up.
- Author uses "it" 10 times in a row; AI extracts a passage where the subject is lost.
- Author leads with backstory; the citable claim is in paragraph 4 where AI engines won't find it first.
- Empty adjective stacking ("our innovative, robust, world-class platform") instead of one concrete fact.

## Next

Move to `03-eeat-signals.md`.
