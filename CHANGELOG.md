# Changelog

Every release of WebX.

## v0.1.1 — 2026-10-17

- A spec with `settings.delivery: "static"` builds a static export: the server-only files (the proxy, the API routes, the sitemap, the `.well-known` route) carry `.server.ts` and leave that build, every locale and screen is pre-rendered, `/` enters the default locale, robots stays static and browser beacons stay quiet.
- The hello feature is client-owned, so a `render: "client"` panel renders it after hydration while a server-delivered site still ships it in the HTML.
- The demo spec is gone: `admin` is a static, client-rendered panel and `client` a server-rendered site.

## v0.0.2 — 2026-10-17

- The spec-driven Next.js engine: screens, blocks and features compiled from specs into sites and panels.
- One element, one component and one feature render a single hello page from every spec.
