# axo — Landing Page

Landing page for **axo**, a Telegram Mini App that introduces children aged 5–9 to English vocabulary through coding commands.

Kids give the hero simple English commands — `jump`, `go up`, `go(3)` — and see the result on screen. The word isn't memorised in the abstract: it's the tool that gets the hero through the challenge. Language meets logic in one calm, timer-free game.

axo is an **introductory stage** — an entry point into English words and command logic, not a full language course. Lessons cover letters, sounds, first words, and simple sequences of commands.

## Live

**https://arinaesp.github.io/axo-landing/**

Deployed via GitHub Pages from `main`. Push to deploy.

## Structure

```
├── index.html        # Landing page (RU/EN bilingual, styles + script inline)
├── privacy.html      # Privacy Policy (RU/EN)
├── terms.html        # Terms of Use (RU/EN)
└── assets/
    ├── icons/        # Favicon set, axo brand logo (SVG)
    └── og-image.png  # Social preview
```

This repo holds the landing page only. The Mini App itself, its lesson content, and its database live in a separate private repository.

## Stack

Vanilla HTML, CSS, and a few lines of JS. No framework, no bundler, no build step, no dependencies — `index.html` is self-contained, with one inline `<style>` block and one inline `<script>`. Fonts are the only external request.

Deliberate: the page is a single document served from a CDN edge, reached mostly from an Instagram bio link on a phone, and it needs to stay fast on a slow connection more than it needs a toolchain.

## Features

- Bilingual RU/EN toggle across all pages — content switches without a page reload
- Inline SVG Venn diagram showing axo at the intersection of Coding and English
- Scroll-triggered reveal animations (`IntersectionObserver` + CSS `@keyframes`, spring easing)
- Mascot float animation with interactive hover
- Responsive — single-column on mobile, expands on desktop
- Respects `prefers-reduced-motion`
- Keyboard-accessible with visible focus states
- No cookies, no analytics, no third-party trackers

## Brand

| Role       | Value                                      |
|------------|--------------------------------------------|
| Primary    | `#693B37` warm brown                       |
| Background | `#F5F2EB` cream                            |
| Accent     | `#E07A3E` orange                           |
| Sage       | `#CCDBB2` green (mascot circle, chart)     |
| Display    | M PLUS Rounded 1c (800)                    |
| Brand      | Caprasimo (single-storey "a" wordmark)     |
| Body       | Figtree (400, 600, 700)                    |

## Methodology

axo's approach to teaching English through coding commands was designed by Arina Bolotbekova, drawing on hands-on classroom experience with children. It builds on TPR (Total Physical Response), developed by psychologist James Asher in the 1960s: a word is learned through the action it produces, so the child types a command and immediately watches it happen on screen.

## Official channels

axo is free. The only official sources are the bot [t.me/axocoder_bot](https://t.me/axocoder_bot), which opens the game, and the public channels **AXO GLOBAL** [t.me/axoglobal](https://t.me/axoglobal) (English) and **AXO Lab** [t.me/axo_lab](https://t.me/axo_lab) (Russian). Any other account, channel, or bot acting on behalf of axo is unaffiliated. axo does not answer private messages in Telegram, never asks for payment, and never asks for passwords, Telegram login codes, SMS codes, or card details. See [Terms of Use §2](https://arinaesp.github.io/axo-landing/terms.html) for details.

## Author and rights

Arina Bolotbekova — developer, methodology creator, and lesson author.

The brand, mascot, lesson content, and methodology belong to the author. Use in classes, links, and screenshots with credit are allowed on the conditions in [Terms of Use §5](https://arinaesp.github.io/axo-landing/terms.html); anything else needs the author's written consent (§5.6, §6).

Contact: by email only, [hello@axolab.space](mailto:hello@axolab.space)
