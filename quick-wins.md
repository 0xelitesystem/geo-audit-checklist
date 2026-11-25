# Quick wins

Ten changes you can make in under an hour each. Do these before the full audit if you need momentum.

## 1. Create llms.txt (20 minutes)

Use [llms-txt-file-builder](https://github.com/0xelitesystem/llms-txt-file-builder). List your top 10 pages with specific descriptions. Upload to site root.

## 2. Update robots.txt (15 minutes)

Use [robots-txt-ai-builder](https://github.com/0xelitesystem/robots-txt-ai-builder). Allow the AI bots you want; explicitly block the ones you don't. Most sites under-block (defaults to everyone).

## 3. Add Organization schema to homepage (10 minutes)

Use [json-ld-markup-builder](https://github.com/0xelitesystem/json-ld-markup-builder). Set name, URL, logo, sameAs (social profiles). Drop the JSON-LD in your `<head>`.

## 4. Add Person schema for the founder (15 minutes)

Same tool. Name, bio, jobTitle, sameAs with LinkedIn, GitHub, Twitter, personal site. Drop in the founder's page or the about page.

## 5. Make sure dateModified is set on top-10 pages (30 minutes)

Article schema needs `dateModified`. If it's missing, add it. Set to the actual last-edit date, not today.

## 6. Rewrite the first paragraph of your homepage (30 minutes)

Use [ai-citability-scorer](https://github.com/0xelitesystem/ai-citability-scorer). Target 70+. Lead with the specific claim and a number. Cut "in today's world" or any throat-clearing.

## 7. Add a visible byline to every blog post (45 minutes per template change)

If your CMS doesn't show authors, fix the template. Then write 2-sentence bios for each contributor and link to author pages.

## 8. Add contact info to the footer (10 minutes)

Email address as plain text. Physical address if applicable. Link to a contact page. AI engines flag pages with no contact info as low-trust.

## 9. Submit sitemap to Bing (5 minutes)

bing.com/webmasters. Verify your site. Submit sitemap. Bing powers Copilot directly.

## 10. Ask the AI engines about your brand and write down what they say (45 minutes)

ChatGPT, Claude, Perplexity, Gemini. Five prompts each (see `00-pre-audit.md`). Save the answers. This is your baseline for everything that follows.

## Total time: about 4 hours

If you do nothing else from this checklist, do these ten. Then come back when you have time for the full audit.
