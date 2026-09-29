# Sahas Foundation — website redesign

A redesign concept for [sahas-foundation.in](https://www.sahas-foundation.in/), a Mumbai-based NGO (Spreading Aid Health And Smiles). Static single-file HTML/CSS/JS — no build step, no dependencies.

## Running it

Just open `index.html` in a browser, or serve the folder with any static file server:

```bash
npx serve .
```

## Content

All copy (mission, project descriptions, founding story, committee bios, bank/80G details, contact info) is sourced directly from the current live site, not rewritten. The visual design — layout, typography, color system — is new.

## Structure

Everything lives in `index.html`: inline `<style>` for CSS, inline `<script>` for the small amount of JS (mobile nav toggle, copy-to-clipboard buttons, demo contact form). Sections, top to bottom:

- Hero
- Vision / About (`#about`)
- Registration & tax-exemption details (`#registration`)
- Projects (`#projects`) — 5 active programs
- Our Story (`#story`)
- Committee (`#team`)
- Get Involved (`#involved`)
- Donate / Contact (`#donate`)
- Footer

## Migrating to Wix

This was built to move to Wix eventually — each `<section>` above maps to one Wix section. The intent is to rebuild it in Wix's own editor (so non-technical committee members can maintain it), not to embed this code as-is. The contact form here is a local demo (`preventDefault` + a confirmation message) and isn't wired to a backend — replace it with Wix Forms, or your own backend, before using it for real submissions.

## Known gaps

- No photos — the current site has photos of named committee members; those were intentionally left out of this version for privacy. Replace the SVG icons/initials with real photography once you have consent to use it.
- Bank details and 80G certificate numbers are copied from the live site as of 2026-09; verify they're still current before publishing.
