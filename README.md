# International Brotherhood of Hoodsters — Local 4663

Static **marketing** site for Local 4663 (GitHub Pages → **local4663.com**).

This repo is launch landing only — not the full Union Books product.

## Live sites

| URL | Repo | Role |
| --- | --- | --- |
| **https://local4663.com** | this repo (`ibh`) | Landing — jacket + **JOIN LOCAL 4663** (launch mode: hover → Coming Soon) |
| **https://local4663.com/pledge** | this repo | Membership card — **PLEDGE TRIBUTE** (no wallet) |
| **https://local4663.com/books** | this repo | Easter egg — sealed notice (unlinked) |
| **https://buildtogetherlabs.github.io/union-hall-preview/** | [`union-hall-preview`](https://github.com/buildtogetherlabs/union-hall-preview) | **Demo** — full Union Books UI · mock numbers · view-only |
| **https://buildtogetherlabs.github.io/union-hall-testnet/** | [`union-hall-testnet`](https://github.com/buildtogetherlabs/union-hall-testnet) | **Testnet** — connect MetaMask · try ETH→$HOOD |
| https://buildtogetherlabs.github.io/ibh/ | this repo | GitHub Pages fallback for marketing |

**Launch mode (local4663.com):** public landing/pledge show **COMING SOON** on hover (no wallet). Product app is not hosted on this domain yet.

## Pages (this repo)

| File / path | Role |
| --- | --- |
| `index.html` | Landing — jacket; launch-mode join button |
| `home.html` | Poster hero + logo (legacy home) |
| `join.html` | Redirects to landing |
| `pledge/index.html` | Membership card; launch-mode CTA (no wallet) |
| `books/index.html` | Easter egg — Form 4663-B hall status; books sealed until launch |

## Assets

| File | Use |
| --- | --- |
| `IBHjacket.png` / `IBHjacket-20260721b.png` | Landing center image |
| `IBHposter.png` | Home page hero |
| `HoodstersLogoWhite.png` | Site logo + favicon (circle on white; all pages) |
| `IBHlogo.png` | Same as white logo (legacy filename) |
| `IBHlogoGreen.png` | Green-square logo — **profile images only** |
| `IBHjacketrear.png` | Jacket rear (reserved) |
| `IBHmembercard.png` | Membership card (pledge page) |

## Workflow

1. Branch → commit → open a PR (or push `main` for deploys)
2. Review and merge to `main`
3. GitHub Pages deploys from `main` automatically → local4663.com

## Local preview

```bash
python3 -m http.server 8080
```

Then visit http://localhost:8080, http://localhost:8080/pledge, and http://localhost:8080/books
