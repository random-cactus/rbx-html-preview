# Moved → https://random-cactus.github.io/

Clothing Studio (the free Roblox clothing previewer / template maker) used to be
served from this repository at `random-cactus.github.io/rbx-html-preview/`.

**It now lives at the domain root: https://random-cactus.github.io/**
The editor itself is at https://random-cactus.github.io/rbx.html

## Why this repo still exists

GitHub Pages cannot issue a real 301 redirect, so this repository is kept alive
purely to serve redirect stubs for the old URLs:

| file | redirects to |
|---|---|
| `index.html` | `https://random-cactus.github.io/` |
| `rbx.html` | `https://random-cactus.github.io/rbx.html` |
| `404.html` | `https://random-cactus.github.io/` (catch-all for every other old path) |

Each stub carries a `<link rel="canonical">`, a zero-second `<meta http-equiv="refresh">`
and a `location.replace()`, plus a plain link as the fallback for crawlers and
no-JS clients. Together that is the closest equivalent to a permanent redirect
that GitHub Pages can serve.

**Do not delete this repository and do not disable Pages on it** — that would turn
every previously shared link into a hard 404 and drop the redirect that
consolidates the old URLs into the new ones.
