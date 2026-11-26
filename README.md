# 🏓 BD RCM Table Tennis Tournament 2026

A live tournament hub I built for our office table tennis tournament: draw, schedule, group tables, knockout bracket and live match scoring in one page, synced in real time for everyone watching.

![HTML](https://img.shields.io/badge/HTML%2FCSS%2FJS-single_file-0F172A?logo=html5&logoColor=E34F26)
![Firebase](https://img.shields.io/badge/Firebase-Realtime_Database-0F172A?logo=firebase&logoColor=FFCA28)

## Features

| Tab | What it does |
|---|---|
| **Draw** | Load 32 teams (paste a list, upload a file, or add manually), then run an animated ball-by-ball group draw |
| **Schedule** | Auto-generated group-stage fixtures; reset or replay a single match |
| **Bracket** | Visual knockout bracket that fills itself from group winners and runners-up; walkovers supported |
| **Points** | Live group standings |
| **Live match** | Coin toss and serve choice, then point-by-point scoring that every viewer sees instantly |

- **Real-time sync:** state is saved to Firebase Realtime Database, so phones and the projector screen show the same score
- **Admin mode:** scoring and resets are locked behind an admin passcode; viewers get a read-only view
- **Offline fallback:** state is cached in `localStorage`
- **Zero build:** one `index.html`, no framework, no server

## Run it

Open `index.html` in a browser, or serve it from any static host (GitHub Pages, Firebase Hosting). To use your own database, change `FIREBASE_DB_URL` near the top of the script.

## Tech

Vanilla JavaScript, CSS custom properties, Firebase Realtime Database (compat SDK 9.23).
