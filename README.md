# Oluwadamilola & Oluwatobiloba — Engagement Website

A single-page engagement website for **Oluwadamilola Esther Adedeji** and
**Oluwatobiloba Emmanuel Otujo**, celebrating their engagement on
**Saturday, 21 November 2026** at the Lighthouse Event Centre (RCCG, Tabernacle
of David), Ilaje, Ajah, Lagos.

It tells the couple's story, shows their photo gallery, lists gift account
details, and lets guests RSVP — all on one scrolling page with no backend, no
database and no sign-in.

> **Live site:** add your deployed URL here once it's up.

---

## Features

| Section | What it does |
| --- | --- |
| **Hero** | Arched photo frame, event date, live countdown to the day, "Add to Calendar" |
| **How We Met** | The couple's own write-up, 17 paragraphs, with a pinned photo alongside the text and a highlighted pull quote |
| **Gallery** | 13 photos in a masonry grid — no empty cells at any photo count, tap any tile to open it full-size |
| **Event Details** | Venue, address, live countdown, Google Maps link, "Add to Calendar" |
| **Gifts & Good Wishes** | A warm note plus two account cards (GBP and NGN), each with a "Copy Account Details" button |
| **RSVP** | Opens WhatsApp with a pre-filled message — guest name, whether they're coming, and how many |
| **Blessing** | A closing verse over a slowly breathing background photo |

**Details that matter**

- **No backend, no data collection.** RSVPs open WhatsApp with a pre-filled
  message; nothing is ever stored, sent to a server, or written to a database.
- **Copy-to-clipboard** for account numbers, with a confirmation toast.
- **Scroll-in animations** on every section and gallery tile, through one shared
  `Reveal` wrapper that switches itself off for visitors who prefer reduced
  motion.
- **Fully responsive** — the same page adapts from phone to desktop.
- **Self-contained build.** All 15 photos are bundled into the output, so the
  deployed site makes zero requests outside your own hosting.
- **Accessible touches:** semantic landmarks, keyboard-openable lightbox,
  `prefers-reduced-motion` respected, `aria-label`s on icon buttons.

---

## Tech stack

- [TanStack Start](https://tanstack.com/start) v1 (React 19, file-based routing)
- [Vite](https://vite.dev) 8
- [Tailwind CSS](https://tailwindcss.com) v4 (design tokens in `src/styles.css`)
- TypeScript
- [Vitest](https://vitest.dev) for tests
- [shadcn/ui](https://ui.shadcn.com) + Radix primitives

The site ships as **static output** — prerendered HTML plus assets. There is no
server function, API route, database or auth.

---

## Getting started

```sh
git clone <your-repo-url>
cd <repo-name>
npm install
npm run dev
