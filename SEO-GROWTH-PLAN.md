# Parrish Projects, SEO growth plan

On-page and technical SEO are done and live (see commit "SEO: crawler-readable prerender snapshot..."). Ranking is won OFF the page. This is the £0, do-it-yourself plan, ordered by leverage. Source frameworks: SEO 2025 (Adam Clarke), Traffic Secrets Dream 100.

## What is already shipped (on-page / technical)
- Crawler-readable content snapshot so Google, GPTBot, ClaudeBot, PerplexityBot and social scrapers index the full page (was a blank SPA shell before).
- JSON-LD: ProfessionalService + WebSite + contactPoint + 6 services.
- Meta description tuned to 157 chars, robots directive, canonical, OG/Twitter cards, valid sitemap + robots.txt, HTTPS, single clean H1, mobile-first, fast TTFB (~0.2s).

## Phase 1, foundation (week 1, free, ~2 hrs total)
1. Google Search Console: verify parrishprojects.com (DNS TXT or HTML tag), submit https://parrishprojects.com/sitemap.xml. This is how you SEE what is working. Non-negotiable.
2. Bing Webmaster Tools: import from GSC in one click (covers Bing + ChatGPT search surfaces).
3. Google Analytics 4 or a lightweight free alt (Plausible has no free tier; use GA4): track traffic + which pages convert.
4. Google Business Profile: even as a remote studio, a GBP with service-area = Guernsey/UK gives a local entity + map presence + a review surface. Free. Fill EVERY field, pick the most specific category (e.g. "Software company" / "Website designer").

## Phase 2, the Dream 100 (week 1-2, free)
Before any outreach, list 30+ specific places your buyers already gather. Minimum split:
- 10 communities: r/smallbusiness, r/automation, r/nocode, Guernsey/Channel Islands business Facebook groups, relevant Slack/Discord ops communities.
- 10 creators: automation / no-code / ops YouTubers, n8n & Make community voices, LinkedIn ops influencers.
- 5 publications/newsletters: no-code newsletters, local Guernsey business press, automation blogs that run roundups.
- 5 competitors: other automation/systems studios, to mine their backlinks (see Phase 3).
Keep this list in a sheet. All traffic work targets these 100, not the whole internet.

## Phase 3, backlinks (ongoing, free, the real ranking lever)
"Without backlinks from quality, relevant sites, you will not rank for competitive keywords." Order of effort:
1. Free quality directories (do 10-15, no more): Clutch, GoodFirms, The Manifest, DesignRush, Crunchbase, local Guernsey business directory, Google Business Profile. Keep NAP (name, email, area) identical everywhere.
2. Connectively (formerly HARO): sign up free, answer journalist queries about AI/automation/small-business ops. Expect 5-15% land rate. Each landed answer = a high-authority backlink + EEAT.
3. Competitor backlink mining: pick a competitor, find who links to them (free: Ahrefs free backlink checker, or Bing "linkfromdomain:"), pitch the same sources your better angle.
4. Testimonials: for every tool in your stack you genuinely use (Stripe, n8n, Supabase, Vercel...), offer a short testimonial. Many publish it WITH a homepage link back to you.
5. Be useful first: comment substantively in the Dream 100 communities, link to them, then ask. No cold link begging.

## Phase 4, content that earns links + ranks (compounding, free)
The home page alone cannot rank for much. Add a small set of intent-matched pages/posts:
- One "money" page per core service (Automation, Web/App, Lead recovery, Integrations, Dashboards). Each targets one transactional/commercial keyword (e.g. "small business workflow automation", "lead recovery system"). This is the highest-ROI content add and worth doing next in the codebase.
- 2-4 informational posts answering real buyer questions (mine r/smallbusiness, AlsoAsked, AnswerThePublic for the actual phrasing). Snippet-bait: 40-50 word concise answers under question-style H2s. Add FAQ JSON-LD.
- Publish on a fixed cadence. Consistency beats volume. Share each piece to the Dream 100 on publish day and again 2-3 days later.

Note: adding routes to a client-rendered SPA on GitHub Pages needs either hash routing or per-path prerendered HTML. When you build service pages, extend the existing `seo-snapshot.js` pattern to emit a static snapshot per route, or move to a host with SSR/SSG. Flag for a future build.

## Phase 5, measure and compound (monthly)
- GSC: which queries show impressions but low CTR -> rewrite that page's title/description.
- GSC: which pages rank position 5-15 -> add internal links + depth to push to page 1.
- GA4: which pages convert to enquiries -> make more like them.
- Build links GRADUALLY. Sudden spikes trigger spam filters. Brand-name anchor text most common, natural variation, never bulk-buy.

## The one-line strategy
Niche relevance + steady quality backlinks + intent-matched service pages + EEAT trust signals, compounded monthly. No single tactic wins; consistent execution across all of them does.
