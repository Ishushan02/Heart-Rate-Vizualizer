# HeartWise

A biomedical informatics project that turns raw heart rate numbers into real-time 3D cardiac visualization — making the heartbeat legible for patients and clinicians alike.

## Structure

- `/` — Landing page (HeartWise marketing site)
- `/Heartwise/` — Live demo (3D anatomical heart with EKG)
- `/storyBoard/` — Project storyboard and design rationale

## Running locally

Open `index.html` directly in a browser, or serve with any static file server:

```
npx serve .
```

The demo at `/Heartwise/` requires a server (not `file://`) due to ES module imports.

## Tech

- Three.js (v0.165.0) via ES module import map
- Vanilla JS, HTML, CSS — no build step
- Hosted on GitHub Pages

## Team

Built by the Design Innovations Group, 2025.
