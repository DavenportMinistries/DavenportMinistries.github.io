# Davenport Ministries — Planning Doc

Reference before starting any non-trivial work. Update when decisions change.

**Completed milestone details → [docs/history.md](history.md)**

---

## Strategic Principles

1. **Minimal footprint**: Stay as simple as the content allows — no frameworks, plugins, or complexity until there's a real need.
2. **Business credibility first**: The site's primary job is to establish legitimacy for platform verification (Facebook, etc.) and make the org easy to find.
3. **Projects are the product**: The LLC's value is its apps; the site exists to surface them cleanly.
4. **Grow the org entry before the site**: Add depth (blog, contact form, media) only after the core projects are mature enough to warrant it.

---

## Master Feature Status

Status: `done` · `planned` · `needs-design` · `needs-decision` · `deferred` · `bug`
Tags: `[post-launch]` `[needs-design]` `[needs-decision]`

### Site Foundation

| Feature | Status | Tags | Notes |
|---|---|---|---|
| Repo + GitHub Pages setup | done | | CNAME + initial commit |
| Jekyll scaffold | planned | | Gemfile, _config.yml, index |
| About section | planned | | Brief org description |
| Projects section | planned | | fellowship-app.com, sdamatch.app |
| Custom domain live | planned | | CNAME exists; needs Jekyll config |

### Future Additions

| Feature | Status | Tags | Notes |
|---|---|---|---|
| Contact / inquiry form | deferred | [post-launch] | Add when there's real inbound |
| Blog / devotionals | deferred | [post-launch] | Only if org content strategy warrants |
| Donation / giving link | deferred | [post-launch] | Not applicable to LLC currently |

---

## Active Backlog

### Jekyll Scaffold

Stand up the minimum Jekyll structure so GitHub Pages renders properly:

- `Gemfile` with `github-pages` gem
- `_config.yml` with site title, description, baseurl, and url
- `index.md` (or `index.html`) with front matter
- Minimal `_layouts/default.html` or rely on a GitHub Pages theme

Constraints: no plugins outside the GitHub Pages whitelist.

### About Section

One short paragraph describing Davenport Ministries LLC — what it is, what it builds, and who it serves. Keep it factual and credibility-oriented (for platform verification readers as much as general visitors).

### Projects Section

A list or card layout for active projects. Each entry needs:
- Project name
- One-line description
- Link to the project URL

Initial projects:
- **Fellowship App** — fellowship-app.com
- **SDA Match** — sdamatch.app

Spec is intentionally open on visual treatment — start with a simple list, upgrade to cards if design warrants.

### Custom Domain Wiring

CNAME file exists (`davenportministries.com`). Ensure `_config.yml` sets `url: "https://davenportministries.com"` and `baseurl: ""` so Jekyll generates correct links. Verify DNS is pointed at GitHub Pages.

---

## Needs Discussion

Nothing currently blocked on a decision.

---

## Decided — Do Not Revisit Without Discussion

- **Jekyll over Astro/plain HTML**: GitHub Pages native support means zero build config and free hosting. Revisit only if content needs outgrow Jekyll.
- **Single-page to start**: No nav, no multi-page structure until the content genuinely needs it.
- **No donation/giving integration**: This is an LLC site, not a church giving portal.
