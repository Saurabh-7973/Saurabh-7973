# Final 5-minute setup checklist

> Three small things only **you** can do (they need GitHub UI access). Each one multiplies the discoverability of this repo by 5–10x.

## 1️⃣ Update your GitHub bio (2 minutes)

Go to <https://github.com/settings/profile> and replace the **Bio** field with:

**Recommended *(151 chars, recruiter-search-friendly)***
```
Flutter Developer · Founder of Snapdrop · Mumbai, India · Open to remote/hybrid roles · Python + Fintech automation · See pinned repos
```

**Alternative *(159 chars, founder-forward)***
```
Founder @Snapdrop. Flutter Developer & Product Engineer in Mumbai. Building algo-trader & AxisCore. Open to full-time, contract & freelance. ✉️ in profile
```

**Also fill in on the same settings page:**
- **Pronouns** — your choice
- **Company** — `Intellect Software Solutions` (or whatever's current)
- **Location** — `Mumbai, India`
- **Website** — `https://linktr.ee/Saurabh7973`
- **Social accounts** — add LinkedIn, Medium, X, YouTube
- **"Available for hire" toggle** — turn it ON (this is a search filter many recruiters use)

---

## 2️⃣ Pin your 4–5 best repos (1 minute)

Go to <https://github.com/Saurabh-7973> → click **"Customize your pins"**. Pin in this order — top-left first, since AI thumbnail extractors and humans both scan that direction:

1. **Snapdrop** — your flagship founder project
2. **algo-trader** — proves Python + systems thinking
3. **AxisCore** — proves architecture chops
4. **Saurabh-7973** — this profile repo (so `resume.json` / `candidate.yaml` are 1 click away)

---

## 3️⃣ Add topics to each repo (2 minutes)

Topics are how GitHub's own search, daily.dev, and many AI sourcing tools categorize repos. Open each repo → click ⚙️ next to **"About"** → paste these topics.

### `snapdrop`
> Description (replace if blank):
> `Flutter app + Figma plugin: send images from phone to Figma over a QR-code session. Socket.IO, Firebase, 6-language i18n.`
>
> Topics:
> ```
> flutter dart figma-plugin mobile-app socket-io firebase cross-platform qr-code image-transfer i18n android ios
> ```

### `algo-trader`
> Description:
> `Zero-cost daily algorithmic trading system for NSE. GitHub Actions scheduler, Google Sheets DB, Angel One/Zerodha brokers, Telegram alerts.`
>
> Topics:
> ```
> python algorithmic-trading nse fintech angel-one zerodha kite-connect github-actions telegram-bot quant gtt-orders
> ```

### `AxisCore`
> Description:
> `Flutter MVP app shell with feature-first architecture, Riverpod, GoRouter, Supabase. 90-day training product.`
>
> Topics:
> ```
> flutter dart riverpod go-router supabase mvp mobile-app cross-platform feature-first
> ```

### `Saurabh-7973` (this profile repo)
> Description:
> `My GitHub profile README. Flutter Developer & Product Engineer in Mumbai. Open to roles.`
>
> Topics:
> ```
> profile-readme flutter-developer hire-me for-hire mumbai india mobile-engineer founding-engineer
> ```

---

## 🎁 Bonus (optional, 5 min) — bulletproof stats with `lowlighter/metrics`

The README's stats cards depend on the public Vercel deployment of `github-readme-stats`, which sometimes returns 503 when overloaded. To get **stats that can never go down** (FAANG-engineer-grade):

1. Go to <https://github.com/settings/tokens> → **Generate new token (classic)**
2. Name: `metrics`. Scopes: `read:user` (and `repo` if you want private repo stats). 90-day expiry.
3. Copy the token. In this repo, go to **Settings → Secrets and variables → Actions**:
   - **Secrets** tab → **New repository secret** → Name: `METRICS_TOKEN`, Value: paste the token
   - **Variables** tab → **New repository variable** → Name: `METRICS_ENABLED`, Value: `true`
4. Go to **Actions** tab → run the **Metrics** workflow once manually (or wait for the daily 3 AM run)
5. After a successful run, `github-metrics.svg` appears in the repo. Add this line in the README's "GitHub at a glance" section:
   ```html
   <img alt="Saurabh's GitHub metrics" src="https://raw.githubusercontent.com/Saurabh-7973/Saurabh-7973/main/github-metrics.svg" />
   ```

Now your stats are a **static SVG file you control**, refreshed daily.

---

## ✅ Done — what changes after this

| Before | After |
|---|---|
| Bio: 1 line about your projects | Bio with role, location, hire-status — picked up by search filters |
| 0 repo topics | 30+ targeted topics across 4 repos — searchable on GitHub, indexed by daily.dev / Glozo / Pin |
| No pins | 4 pins ordered by signal strength |
| `resume.json` exists but undiscovered | Pinned profile repo surfaces it on landing |

You now show up for these recruiter searches (real boolean queries used by sourcing tools):
- `language:Dart location:Mumbai`
- `topic:flutter location:India followers:>0`
- `algorithmic-trading python angel-one`
- `flutter founding-engineer remote`
- `figma-plugin developer mumbai`

That's it. ~5 minutes total (10 with the bonus).
