# cfpkit

> **Self-hosted, open-source community tooling.** Built with a focus on structural clarity, speed, and privacy.

---

`cfpkit` is an organization dedicated to building lightweight, developer-focused, self-hosted tools for local tech meetups and community organizers. We replace heavy, bloated, and expensive SaaS platforms with elegant, single-command deployable applications that put you in full control of your community's data.

---

## 🛠 Featured Project: `cfpkit` (web-app)

Our flagship project is [**cfpkit/web-app**](https://github.com/cfpkit/web-app) — a self-hosted community CFP (Call for Papers) platform that simplifies the entire talk submission, review, and selection lifecycle.

```
                  ┌──────────────────────────────┐
                  │      Caddy Reverse Proxy     │
                  └──────────────┬───────────────┘
                                 │
                   ┌─────────────┴─────────────┐
             /     ▼                           ▼   /api/*
        ┌──────────────────┐           ┌──────────────────┐
        │    React SPA     │           │ PocketBase (Go)  │
        │  (Vite + TW4)    │           │ (SQLite + WAL)   │
        └──────────────────┘           └──────────────────┘
```

### Key Features
*   **Customisable Forms:** Drag-and-drop form builder with conditional logic to ask speakers the right questions.
*   **Public CFP Pages:** Clean, Sessionize-style landing pages with event details and submission countdown timers.
*   **Blind Review:** Server-enforced anonymised grading so review panels can rate talks without speaker bias.
*   **Email Lifecycle Automation:** Custom transactional emails (via Resend SMTP) for submissions, acceptances, and rejections.
*   **Zero-Maintenance Deploy:** Instant spin-up via `docker compose up -d` with automated SSL and domain routing handled by Caddy.

Explore the codebase and deploy your own instance by visiting the [web-app repository](https://github.com/cfpkit/web-app).

---

## 🎨 Visual Philosophy: "The Mechanical Editorial"

All tools in the `cfpkit` ecosystem share a strict visual identity. We reject generic SaaS palettes, heavy drop-shadows, and excessive animations in favor of a clean, editorial layout inspired by printed zines and technical manuals.

*   **Flat-by-Default:** Structure is defined by solid 1px borders (`#DDE6FA`) and light spacing—never drop shadows or complex glassmorphism.
*   **High Contrast Typography:** Editorial serif headlines (**IBM Plex Serif**) paired with light, clean body copy (**IBM Plex Sans**) and monospace labels (**JetBrains Mono**).
*   **The Rarity Rule:** We use a single, vibrant Electric Blue (`#1348DC`) for key interactions and active states, limited to less than 10% of any screen layout to preserve visual intent.

---

## 🗺️ Roadmap & Ecosystem

We are actively designing a complete suite of lightweight utilities for meetup organizers. Our vision includes:

1.  **cfpkit** (Call for Papers & Submissions) — *Active Development*
2.  **badgekit** (Offline attendee badge generator & check-in UI) — *Planning*
3.  **schedulekit** (Drag-and-drop scheduler with auto-generated public agendas) — *Planning*
4.  **surveykit** (Anonymised feedback collection post-event) — *Planning*

---

## 🤝 Getting Involved

We welcome community contributions, feedback, and ideas! 

*   **Deploy it:** Try running `cfpkit` for your next local meetup.
*   **Contribute:** Check out the issues on [cfpkit/web-app](https://github.com/cfpkit/web-app/issues) for frontend enhancement, backend hooks, or setup documentation.
*   **Design:** Help us refine our mechanical-editorial component library.

All `cfpkit` code is open-source and released under the [MIT License](https://github.com/cfpkit/.github/blob/main/LICENSE).
