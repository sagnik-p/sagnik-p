# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

This is Sagnik Pramanik's GitHub **profile repository** (`sagnik-p/sagnik-p`). `README.md` renders directly on https://github.com/sagnik-p. There is no build, lint, or test step - the only workflow is editing `README.md` and pushing to `main` (the README only renders on GitHub, so changes aren't "live" until pushed).

`Sagnik_Pramanik_Resume.pdf` in the repo root is the **source of truth** for all factual content (roles, dates, CGPA, skills). When updating the README, pull facts from the latest resume rather than trusting existing README text.

## Design system

The README uses a cohesive **Tokyo Night** palette across every visual element - keep any new element in these colors:

- Background `1a1b26` · muted `414868` · blue `7aa2f7` · purple `bb9af7` · foreground `c0caf5`

External services rendering the page (verify URLs return 200 with `curl -sI` after editing):

- **capsule-render.vercel.app** - waving gradient banner (header). Custom gradient via `color=0:1a1b26,50:414868,100:7aa2f7`.
- **readme-typing-svg.demolab.com** - animated typing intro. Use the demolab domain, not the flaky herokuapp one.
- **img.shields.io** - all badges, `style=for-the-badge` in the tech stack and social rows.
- Profile photo is a GitHub user-asset URL (returns a 302 redirect to the image - that's normal).

## Gotchas and content rules (owner preferences)

- **Typing SVG clips silently.** At `size=26` Fira Code inside `width=750`, lines longer than ~47 characters get cut off. Shorten the line or raise `width` when editing those lines.
- **GitHub merges adjacent markdown lines** into one paragraph - use a trailing `<br/>` for hard line breaks (e.g. the two roles under sync. labs).
- **Plain hyphens only** - never em dashes (—) or en dashes (–), including in date ranges.
- **No phone number** in the README (public repo; email/LinkedIn/X only).
- The company is written "**sync. labs**" (the link stays `https://sync.so`).
- **Keep it lean.** The owner deliberately removed: experience bullet summaries and company taglines, featured projects, contribution snake (and its workflow), GitHub analytics/stats/streak/trophy cards, the profile-views counter, and the achievements/certifications section. Don't re-add these without being asked.
