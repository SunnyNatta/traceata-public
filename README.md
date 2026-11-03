# traceata-public

Public website for **Traceata**, an iOS GPS logger for personal trip memories —
no account, no cloud, no feed. This repo holds only the static site
(landing page, privacy policy, support contact). The app itself lives in a
private repository.

## Pages

- `index.html` — landing page + support contact
- `privacy.html` — the public privacy policy. **Master source:** the
  `traceata-privacy-policy.md` kept with the project's planning files.
  If the policy text changes, update the master first, then re-render
  `privacy.html` from it — the two copies must never diverge.
- `.nojekyll` — tells GitHub Pages to serve the plain HTML as-is.

## Publishing (GitHub Pages)

1. Push these files to the root of the `main` branch.
2. Repo **Settings → Pages** → Source: *Deploy from a branch* → `main` / `(root)`.
3. The site goes live at `https://sunnynatta.github.io/traceata-public/`
   and the policy at `https://sunnynatta.github.io/traceata-public/privacy.html`
   — that privacy URL is the one that goes into App Store Connect.

## Custom domain (later)

When `traceata.com` is registered, point it at GitHub Pages
(Settings → Pages → Custom domain, plus the DNS records GitHub shows there).
HTTPS is automatic. The App Store Connect privacy and support URLs then move
to `traceata.com/privacy` equivalents.
