# v2 — Engagement features

**Date:** April 2026
**Status:** Live for user testing

## What's new in v2 (vs v1)

| Feature | What it does |
|---|---|
| Welcome banner with prize draw | Big celebratory hero banner at top: confetti animation, gift icon pulse, large £50/€$65 prize amount with shine effect. Country-aware (URL `?country=uk\|us\|ca`). Dismissible, sessionStorage-backed |
| Native share button | Footer button using Web Share API on mobile. Falls back to clipboard copy + toast on desktop |
| Static survey CTA | Soft sky-tinted card between recipe grid and footer linking to Tally survey. Understated |
| Triggered survey prompt | After 2 unique recipes are opened-and-closed, a slide-up bottom sheet appears (500ms after second close) inviting feedback. Single-shot per session, dismissible. Hidden behind modal scrim when a recipe is open |
| Cropped logo | OATOLOGY logo auto-trimmed from 2000x2000 padded to tight 1494x660. Renders larger and crisper |

## Carried over from v1
- 6 recipe cards in 2-col mobile grid
- Real food photography (3-4 images per recipe, optimised WebP)
- Full-screen slide-up modal with hero photo, ingredients, method, tips
- Horizontal thumbnail gallery (tap to swap hero photo)
- Mobile-optimised: iOS scroll lock, safe-area insets, 44px touch targets
- Single inline HTML file, no frameworks

## Known placeholders / future work
- Country detection currently reads URL param only. Need to wire up via Tally redirect once configured

## To roll back to this version
Copy everything in this folder back into `current/` (overwriting), then re-mirror to `deploy/` and re-upload to GitHub.
