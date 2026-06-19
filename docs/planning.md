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
| Jekyll scaffold | done | | Gemfile, _config.yml, _layouts/default.html |
| About section | done | | Single paragraph in index.html |
| Projects section | done | | Cards: fellowship-app.com, sdamatch.app |
| Custom domain live | done | | _config.yml wired; verify DNS on GitHub Pages settings |

### Future Additions

| Feature | Status | Tags | Notes |
|---|---|---|---|
| Contact / inquiry form | deferred | [post-launch] | Add when there's real inbound |
| Blog / devotionals | deferred | [post-launch] | Only if org content strategy warrants |
| Donation / giving link | deferred | [post-launch] | Not applicable to LLC currently |

---

## Active Backlog

Nothing in active backlog. See Future Additions in the status table for deferred items.

---

## Needs Discussion

Nothing currently blocked on a decision.

---

## Decided — Do Not Revisit Without Discussion

- **Jekyll over Astro/plain HTML**: GitHub Pages native support means zero build config and free hosting. Revisit only if content needs outgrow Jekyll.
- **Single-page to start**: No nav, no multi-page structure until the content genuinely needs it.
- **No donation/giving integration**: This is an LLC site, not a church giving portal.
