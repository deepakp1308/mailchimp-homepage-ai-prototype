# Mailchimp Homepage AI Prototype

A pre-auth Mailchimp homepage prototype with a single **persona-pivot hero** that embeds the **full Analytics AI playground**, plus the complete homepage flow underneath. Built for stakeholder review.

## Live URL

**https://deepakp1308.github.io/mailchimp-homepage-ai-prototype/**

## What's here

- **The hero** · 4 persona pills (E-commerce founder · Agency · Nonprofit · B2B services) sit above a 2-column layout: persona-specific headline + feature trio on the left, and the **embedded Analytics AI playground** on the right (dark navy frame, Analytics AI pill, two-column chat plus live visualization). A `Sample data | Upload Excel / CSV` toggle sits above the playground, with drag-drop CSV / XLSX parsing that auto-generates insights from any uploaded file.
- **Persona-aware playground** · clicking a persona instantly swaps the toolbar business name (Oat Lord · Live demo / PixelEdge Agency / Reach Out · Live demo / Sundial SaaS), the greeting, the four suggested-question chips, and the pre-loaded sample insight chart. Each suggested question renders a rich, persona-specific answer + chart (line+anomaly, donut, forecast fan, ranked horizontal bars, deliverability heat grid, bubble scatter, retention trend, donor cohort table, churn-risk tier card).
- **Auto-rotation** · personas auto-cycle every 8s and pause on hover or first manual interaction (chip click, persona pill, dot, input typing, mode toggle, or file upload).
- **Shared below the fold** · Recommended for your business · Marketing that delivers results · Personalized tour · Pricing · 300+ integrations · Customer testimonials · FAQ · Final CTA · Footer.

## Stack

Plain HTML / CSS / vanilla JS, single `index.html`, plus PapaParse and SheetJS loaded from jsDelivr for the upload zone. No framework, no build step. Works directly on GitHub Pages.

## Brand consistency

- Same color tokens as `mailchimp-analytics-ai-prototype` (peppercorn, Cavendish yellow, deep teal, etc.)
- Cooper Light italic for hero headlines, Helvetica Neue for body
- Yellow Cavendish primary CTAs, dark peppercorn secondary
- The playground frame is intentionally dark navy `#15100A` so it reads as a "live tool" embedded in the cream homepage canvas
- No em/en dashes in user-facing copy; no emojis; no rainbow gradient text

## Implementation notes

- One hero, no variant switcher. Earlier review builds shipped 3 hero variants (A · Ask Mailchimp, B · Persona pivot, C · Watch the agent); the persona-pivot hero with the embedded playground was the strongest, so the other two were removed.
- All event listeners guard for null nodes; uploading a file in the playground works without page reload.
- Cinematic scenes (the auto-rotation between personas and the chip / chart animations) honor `prefers-reduced-motion`.

## Sibling prototype

This repo lives alongside the **analytics-only** prototype:

- Analytics: https://github.com/deepakp1308/mailchimp-analytics-ai-prototype
- Homepage: https://github.com/deepakp1308/mailchimp-homepage-ai-prototype  ← (this one)

The two prototypes are independent. Updates here do not affect the analytics page.
