---
name: b12-website-editor
description: Edit and improve a live B12 website using Claude's browser access in Claude Cowork. Claude can take screenshots, scroll, click, and type directly into the B12 editor to apply design changes, add sections, rewrite copy, and build web app features.
---

# B12 Website Editor Skill

## Goal

Help the user edit and improve their B12 website or web app using browser access. You can take screenshots, scroll, click, and type directly into the page.

> **Requires browser access.** This skill only works in Claude Cowork (Claude in Chrome extension). Make sure the B12 editor tab is active before invoking.

## What You Can Do

- Analyze the current design and suggest specific improvements
- Apply any visual style (minimal, dark, luxury, SaaS, playful, corporate, etc.)
- Add or redesign sections (hero, pricing, testimonials, nav, footer, forms, cards, etc.)
- Add web app features (booking forms, pricing tables, dashboards, member areas, directories)
- Rewrite copy, headlines, CTAs, and page content
- Restructure navigation and page layout

## The B12 Editor Interface

The B12 editor is at: `https://b12.io/client/{CLIENT_ID}/site_builder/#/website`

The page has:
- A left panel with an AI Agent chat
- An **"Ask AI Agent..."** text input at the bottom of the left panel
- A live website preview on the right that you can scroll

## How to Work

1. Take a screenshot first to see the current state of the site
2. Scroll through the full preview to understand all sections
3. Either follow the user's specific instruction, or suggest 3–5 concrete improvements and ask which to apply
4. Use the browser to click the **"Ask AI Agent..."** input, type the instruction, and press Enter
5. Wait for the agent to finish (watch the preview update), then screenshot to verify
6. Keep instructions short — the B12 agent works best with 1–3 actions at a time
7. If a change doesn't look right, immediately send a correction to the agent

## Rules for Writing B12 Agent Instructions

- Keep each message to 1–3 focused actions
- Be specific: use hex color codes, name exact sections, describe exact locations
- Separate style changes from layout changes into different messages
- If the agent does something wrong, say: *"Undo that and try: [clearer version]"*

## Style Translation Guide

When the user describes a style, translate it into specific instructions:

| Style | Translate to |
|---|---|
| Dark / cinematic | `#0a0a0a` background, bold white type, red or gold accent, full-bleed imagery |
| Minimal / clean | White background, lots of whitespace, single accent color, no decorative elements |
| Luxury / premium | Black + gold/cream, serif fonts, full-bleed photography, elegant spacing |
| SaaS / tech | Feature grids, pricing tables, social proof logos, dashboard screenshots |
| Bold / agency | Large type, high contrast, asymmetric layouts, strong color blocks |
| Playful / consumer | Bright colors, rounded corners, friendly tone, large CTAs |

## Example Instructions That Work Well

- "Change the background to `#0f0f0f` and all text to `#ffffff`"
- "Make the hero full-width with a bold headline on the left and a red CTA button"
- "Add a 3-column pricing section with Starter, Pro, and Enterprise tiers"
- "Add a 'See All →' link on the right side of each section heading"
- "Rewrite the homepage headline to focus on the main benefit for the target audience"
- "Add a horizontal scrollable row of cards labeled 'Featured' with left/right arrows"
- "Make the navigation bar dark with white text and a blur effect"
- "Add a testimonials section with 3 quotes, names, and star ratings"
- "Redesign the contact page to include a booking/appointment form"
- "Add a SaaS-style features grid with icons, titles, and one-line descriptions"

## On Invocation

Take a screenshot immediately and describe what you see, then wait for the user's first instruction — or ask what they'd like to change.
