# Iron Veil: Outpost

A playable 3D browser FPS with procedural assets, enemy waves, shooting effects, audio, HUD, pickups, mobile controls, and an industrial outpost map.

## Play

The production site is published from `main` with GitHub Actions:

**https://baklawaa.github.io/iron-veil/**

For the first deployment, open **Repository Settings → Pages** and select **GitHub Actions** as the source. Every later push to `main` deploys automatically.

## Install as a PWA

The repository includes:

- a web app manifest;
- an installable app icon;
- a service worker for application-shell and runtime caching;
- standalone, landscape-oriented display settings.

On a supported browser, use **Install app** or **Add to Home Screen**. The initial launch needs a network connection to load the Three.js engine; repeat launches can use the service-worker cache.

## Desktop controls

- **WASD** — Move
- **Mouse** — Look
- **Left click** — Fire
- **Right click** — Aim
- **Shift** — Sprint
- **Space** — Jump
- **R** — Reload
- **Esc** — Release pointer / pause

## Touch controls

- **Left virtual stick** — Move
- **Drag the game view** — Look
- **FIRE** — Shoot
- **R** — Reload
- **↑** — Jump

## Deployment

The workflow at `.github/workflows/pages.yml` packages the repository as a static Pages artifact and deploys it to the `github-pages` environment. The `.nojekyll` marker keeps the game files untouched by Jekyll processing.