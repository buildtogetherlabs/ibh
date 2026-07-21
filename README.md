# International Brotherhood of Hoodsters — Local 4663

Static site for the IBH Union Hall.

## Live sites

| URL | Role |
| --- | --- |
| **https://local4663.com** | Landing — jacket + **JOIN LOCAL 4663** |
| **https://local4663.com/pledge** | Airdrop / tribute — membership card + **PLEDGE TRIBUTE** |
| https://pledge.local4663.com | Same pledge site (needs Cloudflare CNAME — see below) |
| https://gibtogether.github.io/ibh/ | GitHub Pages fallback for landing |

### Optional: `pledge.local4663.com` DNS (Cloudflare)

In Cloudflare → **local4663.com** → **DNS** → **Add record**:

| Type | Name | Target | Proxy status |
| --- | --- | --- | --- |
| CNAME | `pledge` | `gibtogether.github.io` | DNS only (grey cloud) |

Until that record exists, use **https://local4663.com/pledge** (already live via this repo).

## Pages (this repo)

| File | Role |
| --- | --- |
| `index.html` | Landing — jacket; join links to `https://local4663.com/pledge` |
| `home.html` | Union Hall home — poster hero + logo |

## Assets

| File | Use |
| --- | --- |
| `IBHjacket.png` | Landing center image |
| `IBHposter.png` | Home page hero |
| `IBHlogo.png` | Site logo + favicon |
| `IBHjacketrear.png` | Jacket rear (reserved) |

## Workflow

1. Branch → commit → open a PR
2. Review and merge to `main`
3. GitHub Pages deploys from `main` automatically

## Local preview

Open `index.html` in a browser, or from the repo root:

```bash
python3 -m http.server 8080
```

Then visit http://localhost:8080
