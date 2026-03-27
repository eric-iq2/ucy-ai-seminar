# UCY AI Seminar Project

## Context
This repo contains the AI seminar presentation for the University of Cyprus (UCY), specifically for the **Directorate of Administration & Finance** department. First delivered March 27, 2026.

## Audience
University of Cyprus administrative staff (Directorate of Administration & Finance) — NOT teachers or lecturers. Content focuses on admin workflows, finance, communications, and processes.

## Ownership & Identity
- **GitHub account:** `eric-iq2` (NOT `ericosg` — that's personal)
- **Domain:** iq2.org (Eric's professional domain)
- **Email:** eric@iq2.org
- All UCY-related work should be under the `eric-iq2` account

## Hosting — Two locations

### 1. Primary: Firebase (iq2.org)
- **Live URL:** https://iq2.org/ucy/ai.html
- **Firebase project:** `iq2org`
- **Site repo:** `eric-iq2/iq2` (private) → cloned at `~/sandbox/iq2`
- **File location:** `~/sandbox/iq2/public/ucy/ai.html`
- **Deploy command:** `cd ~/sandbox/iq2 && firebase deploy --only hosting --project iq2org`
- The homepage (`iq2.org`) links to this page under "Read more on: AI"
- The blockchain seminar is at `iq2.org/ucy/blockchain.html`

### 2. Backup: GitHub Pages
- **URL:** https://eric-iq2.github.io/ucy-ai-seminar/
- **Repo:** `eric-iq2/ucy-ai-seminar` (public) → this repo, cloned at `~/sandbox/ucy`
- **Deploy:** Automatic on push to `main` (GitHub Pages legacy build)

## How to update the presentation

1. Edit `~/sandbox/ucy/index.html` (this is the source of truth)
2. Copy to Firebase site: `cp ~/sandbox/ucy/index.html ~/sandbox/iq2/public/ucy/ai.html`
3. Deploy Firebase: `cd ~/sandbox/iq2 && firebase deploy --only hosting --project iq2org`
4. Commit & push both repos:
   - `~/sandbox/ucy` → pushes to `eric-iq2/ucy-ai-seminar` (GitHub Pages updates automatically)
   - `~/sandbox/iq2` → pushes to `eric-iq2/iq2` (Firebase already deployed in step 3)

## Structure
- `index.html` — Single-file HTML presentation (40 slides, bilingual Greek/English)
- `backup_v1.zip` — Backup of v1 (teacher-targeted, before admin retargeting)
- `CLAUDE.md` — This file

## Presentation details
- **Format:** Single HTML file, dark theme, keyboard/touch navigation (arrows, spacebar, swipe)
- **Template origin:** Based on `~/sandbox/sara/skills_demo/presentation.html`
- **Part 1 (~90 min):** AI landscape, university use cases, amazing tools, EU AI Act
- **Part 2 (~90 min):** LLM tips (Eric's 3 key tips: English prompts, one topic per chat, token efficiency), prompting techniques, workflows, agentic AI, hands-on exercises

## Firebase setup
- Project: `iq2org` (project ID)
- Hosting site: `iq2org` → `iq2org.web.app` / `iq2.org`
- Auth: `firebase login` (Eric's Google account)
- Config: `firebase.json` serves from `public/` directory
- Analytics: Google Analytics integrated (measurement ID: `G-43XM6QWZT8`)

## Related files elsewhere
- Past seminar content: `~/Downloads/WORK/OTHER/ai 3h.md`
- Blockchain seminar: `~/Downloads/WORK/OTHER/blockchain 4h.md` (separate topic)
- Old AI resources: https://linktr.ee/aioct18 (outdated, Oct 2023)
