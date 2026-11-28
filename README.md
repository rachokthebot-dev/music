# Music apps — stable link

https://rachokthebot-dev.github.io/music/ forwards to wherever my self-hosted
[guitar practice apps](https://github.com/rachokthebot-dev/guitar-practice-apps) are currently
running. The apps are served from my own machine through a Cloudflare quick tunnel,
whose URL changes on every restart; this page reads `tunnel.json` and redirects, so
the public link never changes.

- `index.html` — fetches `tunnel.json` and forwards, keeping the path, query and hash
- `404.html` — the same, so deep links like `/music/shreddy` work
- `tunnel.json` — the current tunnel URL, rewritten automatically when the tunnel restarts

If the apps are offline the page says so. Source code for the apps:
[rachokthebot-dev/guitar-practice-apps](https://github.com/rachokthebot-dev/guitar-practice-apps).

MIT licensed.
