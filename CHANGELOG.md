# Changelog

Every release of WebX.

## v0.1.3 — 2026-10-18

- The README's Download block: `webx-installer.sh` / `.ps1` unpack the latest release's source, or clone and run `bun run dev`.

## v0.1.2 — 2026-10-18

- The client runtime (session, signals and the access guard) loads only when the spec declares ports, access, signals, a session cookie or realtime; a static panel without them ships none of it.
- `bun run build --all` builds every installed spec, so both deliveries are gated; the theme stylesheet comes from the engine.

## v0.1.1 — 2026-10-17

- A spec with `settings.delivery: "static"` builds a static export: the server-only files (the proxy, the API routes, the sitemap, the `.well-known` route) carry `.server.ts` and leave that build, every locale and screen is pre-rendered, `/` enters the default locale, robots stays static and browser beacons stay quiet.
- The hello feature is client-owned, so a `render: "client"` panel renders it after hydration while a server-delivered site still ships it in the HTML.
- The demo spec is gone: `admin` is a static, client-rendered panel and `client` a server-rendered site.

## v0.0.2 — 2026-10-17

- The spec-driven Next.js engine: screens, blocks and features compiled from specs into sites and panels.
- One element, one component and one feature render a single hello page from every spec.
