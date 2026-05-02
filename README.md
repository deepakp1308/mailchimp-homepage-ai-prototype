# Mailchimp Homepage AI Prototype

A pre-auth Mailchimp homepage prototype with **three switchable hero variants** and the **full homepage flow** beneath each. Built for stakeholder review.

## Live URL

**https://deepakp1308.github.io/mailchimp-homepage-ai-prototype/**

Deep links:

- Variant A · Ask Mailchimp → `#variant=a`
- Variant B · Persona pivot → `#variant=b`
- Variant C · Watch the agent → `#variant=c`

## What's here

- **Three heroes**, switchable from a sticky bar at the top of the page:
  1. **Ask Mailchimp** · conversational input with rotating prompts, 7 chip suggestions, and a streamed answer panel that explains which Mailchimp tools were used.
  2. **Persona pivot** · 4 persona pills (E-commerce / Agency / Nonprofit / B2B), each with its own headline, hand-drawn feature trio, agent demo card, and auto-rotating dots.
  3. **Watch the agent** · cinematic browser-frame mockup that auto-cycles 6 scenes (Editor / Segment / Analytics / Automation / SMS / Brand kit).
- **Shared below the fold**: Recommended for your business · Marketing that delivers results · Personalized tour · Pricing · 300+ integrations · Customer testimonials · FAQ · Final CTA · Footer.

## Stack

Plain HTML / CSS / vanilla JS, single `index.html`. No framework, no build step. Works directly on GitHub Pages.

## Brand consistency

- Same color tokens as `mailchimp-analytics-ai-prototype` (peppercorn, Cavendish yellow, deep teal, etc.)
- Cooper Light italic for hero headlines, Helvetica Neue for body
- Mini-spot ink illustrations carried over from the Mailchimp brand library
- Yellow Cavendish primary CTAs, dark peppercorn secondary
- No em/en dashes in copy; no emojis; no rainbow gradient text

## Implementation notes

- Variant switcher is sticky and always visible (this is a stakeholder review build).
- URL hash deep-links: `#variant=a|b|c` so PMs can share specific variants.
- Persona auto-rotation pauses on hover and stops on first manual click.
- Cinematic scene cycler honors `prefers-reduced-motion`.
- All event listeners guard for null nodes — clicking a variant tab will never throw.

## Sibling prototype

This repo lives alongside the **analytics-only** prototype:

- Analytics: https://github.com/deepakp1308/mailchimp-analytics-ai-prototype
- Homepage: https://github.com/deepakp1308/mailchimp-homepage-ai-prototype  ← (this one)

The two prototypes are independent. Updates here do not affect the analytics page.
