# zamora_osi

Working framework for the Organizational Strategy & Impact function. Irving ISD branded.

## Structure

```
index.html                    Hub — thesis, six domains, year one, roadmap
portfolio-capacity.html       Domain 01 · Portfolio & Capacity
organizational-health.html    Domain 03 · Organizational Health
capacity-measurement.html     Domain 05 · Campus Capacity Measurement
effectiveness-model.html      Domain 06 · District Effectiveness Model
assets/css/style.css          Shared design system (Irving ISD palette)
```

Domain 02 (Strategic Planning & Execution) and Domain 04 (Strategic Compensation) are stubbed as cards on the hub and not yet built.

## Privacy posture

- All pages carry `noindex, nofollow, noarchive, nosnippet`
- `referrer: no-referrer` set on all pages
- No author name, no confidentiality banner, no contact details in markup
- **Do not link this repo from any public site, profile, or README**

## Deploying to GitHub Pages

1. Push these files to the root of `main`.
2. Settings → Pages → Source: `main` / `/ (root)`.
3. URL will be `https://<username>.github.io/zamora_osi/`.
4. Share the URL directly. Do not add it to any index or profile.

## Adding a domain deep dive

Copy any existing deep dive as the template. Each uses:
- `.hero` with a `Domain 0X · Deep dive` eyebrow
- `.toc` jump links
- `.prose` for body copy, `.callout` / `.callout.gold` for pull-outs
- Page-specific components in a `<style>` block after the stylesheet link

Then update the matching `.domain` card in `index.html` — swap the `<div>` for an `<a href>` and replace `.domain-soon` with `.domain-go`.

## Roadmap status pills

In `index.html`, the `.track` section. Status classes: `.now` (gold), `.next` (blue), `.later` (gray). Update as work moves.
