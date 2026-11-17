# group-02-hello-world

Reference project for **scenario 1** of the group 02 Netlify clone: the smallest end-to-end deployment of a static site.

- No build step: the repository root is the site.
- `index.html` sits at the root, which is what the platform's readiness check looks for (hotspot H3).
- Stylesheet and logo use absolute paths (`/style.css`, `/logo.svg`). They only load when the site is served from the root of its own host, so a page with styling and logo proves subdomain routing serves the build unmodified.
- The logo is also the favicon, so the browser makes no request for `/favicon.ico`.

**Done when:** the page loads on `http://hello-<suffix>.platform.localhost` with styling and logo and no 404s in the network tab.
