# Mercy College Work Dashboard

Personal work command center for Mercy College of Health Sciences staff.

## Overview

A single-page HTML dashboard providing quick access to all key tools, enrollment data, upcoming events, and social media feeds — built in the MCHS brand (purple + green).

## Features

- **Time-based greeting** — automatically says Good morning / Good afternoon / Good evening
- **Live data placeholders** — four enrollment metric tiles wired to future dashboards (Enrollment, Admissions Funnel, Enrollment Forecast)
- **Tool tiles** — Slate CRM, Website Admin (WordPress), Marketing Analytics (GA4), Brand Resources
- **Interactive task list** — click to toggle complete, open count updates live
- **Upcoming Events** — attempts to load live from the Pulse Campus Calendar via SharePoint REST API; shows an auth error with sign-in link if session has expired
- **Social media feed** — tabbed LinkedIn / Facebook / Instagram feed (simulated; API-ready)
- **Quick nav sidebar** — links to MCHS homepage, staff/student portals, CRM & admin tools, social channels

## Deployment (GitHub Pages)

1. Create a new GitHub repository (e.g. `mchs-dashboard`)
2. Upload `mchs-dashboard.html` and rename it to `index.html` (or keep the filename and link to it directly)
3. Go to **Settings → Pages**
4. Set source to **Deploy from a branch → main → / (root)**
5. Your dashboard will be live at `https://[your-username].github.io/mchs-dashboard/`

## File Structure

```
mchs-dashboard.html   ← Single self-contained HTML file (no dependencies)
README.md             ← This file
```

## Future Integrations

| Metric | Source dashboard | Status |
|--------|-----------------|--------|
| Total Enrollment | Enrollment Dashboard | To build |
| AY Total New Students | Admissions Funnel | To build |
| Forecast Total Enrollment | Enrollment Forecast | To build |
| Forecast New Enrollment | Enrollment Forecast | To build |

Social media live feeds will require API credentials:
- **LinkedIn** — LinkedIn Marketing Developer Platform
- **Facebook** — Facebook Graph API (Page token)
- **Instagram** — Instagram Basic Display API

## Brand

Colors, typography, and logo follow the [Mercy College Visual Identity Guide](https://www.mchs.edu/marketing).

- Primary: `#4A2C6B` (Mercy Purple)
- Accent: `#5A8C3C` (Mercy Green)
- Typography: Libre Baskerville (serif) + Source Sans 3 (sans-serif)
