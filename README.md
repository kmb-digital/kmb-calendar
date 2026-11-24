# KMB Calendar 2027

Every Kolej MARA Banting event, exam, test and deadline for 2027 in one place, with countdowns and a date checker for teachers.

Developed by **Digitalisation in Teaching & Learning Unit** for **Academic Affairs Unit**.

## How it works

- This page (`index.html`) is hosted on GitHub Pages.
- The events live in a Google Sheet. The page reads and saves them through a Google Apps Script web app (`Code.gs`).
- Everyone can view. Only editors with a PIN (Editors tab in the sheet) can add, edit or delete events.

## Files

| File | What it is |
|---|---|
| `index.html` | The calendar page |
| `thumb.jpg` | Preview image shown when the link is shared (1200 × 630) |
| `favicon.png` | Browser tab icon |
| `apple-touch-icon.png` | Icon when saved to a phone home screen |

## Setup

1. Set up the Apps Script web app first (`Code.gs` + `Index.html`, run `setup`, Deploy → Web app, Execute as: Me, Who has access: Anyone). Copy the `/exec` link.
2. Open `index.html`, find `TAKWIM_API` near the top, and paste the `/exec` link between the quotes.
3. If the site address is not `https://kmb-digital.github.io/kmb-calendar/`, replace that address in the `og:url`, `og:image` and `twitter:image` lines.
4. Upload all files to the repository, then Settings → Pages → Deploy from branch → `main` / root.

When the Apps Script code changes, use Deploy → Manage deployments → New version so the `/exec` link stays the same.
