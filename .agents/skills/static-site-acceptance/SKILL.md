---
name: static-site-acceptance
description: Validate this Enderloom static information site, local navigation, accessibility and accurate account-connection explanations without mixing in desktop implementation or altering policy claims casually.
---

# Static Enderloom site acceptance

Use for root HTML/CSS changes. Inspect `index.html`, `style.css`, `privacy.html`, `terms.html` and `docs/competitive-landscape.md`. There is no application build step or package manifest in this checkout.

1. Record starting commit and review existing copy before editing. Keep the site distinct from the Enderloom desktop repository. Describe current capability versus under-development tooling honestly.
2. Preserve `.nojekyll`, existing robots directives, skip navigation, heading hierarchy and responsive viewport. Do not turn indexing on because search visibility seems desirable without a scoped decision.
3. Check every changed local `href`/`src` resolves inside the repository; check fragment IDs exist on their destination page. Inspect outbound URLs for the intended repository, support and policy destinations. Do not treat a syntactically valid URL as a verified live destination.
4. Serve the repository with `python3 -m http.server 8000` and inspect homepage, privacy and terms pages at narrow/mobile and desktop widths. No build tools are required. Verify keyboard Tab order, skip link, visible focus, anchor navigation, text contrast and no horizontal overflow. Read console errors where browser tooling is available.
5. Compare connection copy against verified Enderloom behavior: persistent website sessions are not Google API permission grants; disconnect/revoke directions must remain accurate. Never place real tokens, account details or private screenshots in public test artifacts. Do not add legal promises, new permission scopes or telemetry claims without evidence and appropriate authorization.
6. If publishing is authorized, verify exact remote file identity separately from served-page behavior. A successful push alone is not a Pages deployment or browser acceptance result; record deployment and loaded HTML/CSS identity when available.

Retain a small evidence ledger: commit, changed pages, local link check, viewport/browser observations, any untested behavior and live-publication status. If a browser is unavailable, static checks can pass while visual/keyboard acceptance remains explicitly untested.
