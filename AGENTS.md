# Dreamist DAO — Agent Guide

## Purpose
This repository contains the working agreement and operating materials for Dreamist DAO. Keep the published site faithful to the Markdown source documents.

## Website synchronization rule
`index.html` and `meeting.html` are the GitHub Pages visual companions to this repository. Whenever a change affects member-facing content, update the matching section of the relevant HTML page in the same change. `meeting.html` must contain the complete member-facing content of `meetings/MONTHLY_MEETING.md`.

Update the site for changes to:

- `meetings/MONTHLY_MEETING.md` — meeting rhythm, agenda, sharing flow, Deep Dive, meeting guidelines, and after-meeting practice.
- `community/*.md` — purpose, trust, conduct, onboarding, or friendship practices.
- `governance/*.md` — leadership, decision-making, or active proposal information shown on the site.
- `ROADMAP_90_DAYS.md` — launch plan or milestones shown on the site.

For template-only changes, update `index.html` when the template’s member-facing instructions or meeting flow changes. Cosmetic or internal-only changes do not require a site update.

Before finishing a content change:

1. Check that `index.html` and/or `meeting.html` still match the relevant Markdown source.
2. Preserve the site’s confidentiality guidance: never add private examples, member names, or meeting notes.
3. Run `git diff --check`.

## GitHub Pages
The Pages workflow is `.github/workflows/deploy-pages.yml`. It deploys the HTML pages and repository assets on pushes to `main`. Repository settings must allow GitHub Pages deployments via GitHub Actions.
