# SHWETA — Law, Rights & Independent Thought

This is a static, multi-page publication site designed for Vercel. It keeps the editorial identity of the original site while giving each publication section its own clean route.

## Routes

- `/` — concise publication homepage
- `/journal` and `/journal/[article]` — article archive and full essays
- `/casebook` and `/casebook/[case]` — searchable case library and structured case files
- `/rights` and `/rights/[topic]` — practical topic hubs
- `/perspective` and `/perspective/[essay]` — Shweta's essays
- `/research` and `/research/[publication]` — research previews and case collections
- `/the-brief` and `/the-brief/[issue]` — newsletter archive
- `/about` and `/editorial-standards`

## Content and deployment

`content.json` is the structured content source. It contains article, case, topic, research and newsletter records, including their relationships and source links. `build_site.py` generates the route HTML, search index, sitemap and robots file from that source.

To update the site, edit `content.json`, run `python build_site.py` from this folder, then redeploy this folder to the existing Vercel project. Vercel serves the generated pages as static files; no server build command is required.

## Working features

- Individual clean URLs with page titles, descriptions, canonical links and WebPage structured data
- Global search across articles, cases, rights guides, research and Brief issues, with content type and topic filters
- Archive filters for journal, cases and research
- Save buttons and a saved-reading list stored locally in the current browser
- Reading progress on long articles and research pages
- Reader preferences for text size, reading width and dark mode, stored locally
- Responsive navigation and reduced-motion support

## Service-backed features not connected yet

There is no remote CMS, secure user account, device-to-device bookmark sync, subscriber capture, email delivery, premium checkout, analytics dashboard or admin publishing workflow. The current JSON content model is the editable publishing source; adding a hosted CMS and database is the next infrastructure phase. Research entries marked “Preview” are not for sale, and no payment flow is implied.

## Editorial note

Legal summaries are educational and should be checked against the linked primary materials and current law before publication. Have the site's disclaimer and jurisdiction-specific policies reviewed professionally. This site does not provide legal advice or create a lawyer–client relationship.
