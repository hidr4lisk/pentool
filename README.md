# Hidr4lisk_Pentool

**Interactive Pentesting Guide** — a guided checklist & note-taking tool for penetration testing.
100% client-side · offline-first · no backend · no tracking.

🌐 **[Live demo](https://hidr4lisk.github.io/pentool/)** · 🇦🇷 **[Leer en español](./README.es.md)**

---

## What it is

A single-page web app that walks you through a pentest as a set of ordered steps — network-wide and
per-target — keeping your notes, the tools you've used and the commands you ran all in one place.
Built for studying and for real engagements: the checklist you wish you had open on a second monitor.

Everything lives in your browser. Your findings never touch a server. You move your work between
machines by exporting/importing a file — nothing else.

## Features

| # | Feature | Description |
|---|---------|-------------|
| 01 | **One guided methodology** | A single PTES / kill-chain funnel — recon → enumeration → vuln analysis → exploitation → post-exploitation → reporting — that zooms from the whole network down to the individual host. Each step carries a scope chip (`NET` / `OSINT` / `WEB` / `HOST`) so there's no tab-switching and no duplicated tooling. |
| 02 | **60+ tools with examples** | Every step lists the relevant tools as chips. Click a tool to see ready-to-use command examples; click a command to copy it. |
| 03 | **Per-step notes** | A notes field on every step, auto-saved as you type, with line/char counters. |
| 04 | **Multiple sessions** | One isolated workspace per engagement/target — create, rename, duplicate, delete. Each keeps its own notes and tool checklist. |
| 05 | **Export / Import** | Markdown (`.md`) per session for a clean report, or JSON for *all* sessions — your portable backup. |
| 06 | **Progress & trail** | Progress bars per category, a tool-journey trail of what you used where, and live search across notes and tools. |
| 07 | **Comfort** | Font-size control (A−/A+), 1- or 2-column layout, full keyboard shortcuts, dark terminal theme. |

## Privacy

- **Zero network connections** — the page loads no external resources; open it once and it works with no internet.
- No cookies, no analytics, no fingerprinting, no backend.
- All state lives in `localStorage`; your pentest data never leaves your browser.
- Portability is explicit: *you* decide when to export a `.md` / `.json` file.
- The whole thing is one auditable HTML file.

## How your data moves

```
 your browser (localStorage)  ──Export .md / JSON──▶  a file you own
         ▲                                                  │
         └───────────────────  Import  ◀────────────────────┘
```

No account, no sync, no server. Move between machines by carrying the file.

## Stack

- **Vanilla JS** — a single self-contained HTML file, no dependencies, no build step.
- **Web Storage API** — `localStorage` for live state (notes, tool checks, sessions, preferences).
- **GitHub Pages** — static deploy.

## Intended use

For **authorized** penetration testing, lab practice and security study only (CTFs, your own
networks, engagements with written permission). It is a note-taking checklist — it runs no scans
and attacks nothing by itself. Use it only where you are allowed to.

## License

[MIT](./LICENSE)
