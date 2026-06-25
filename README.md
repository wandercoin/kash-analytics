# Kash Analytics

A small, independent analytics dashboard built on top of the **public Kash API**
(`app.kash.bot/api`). It runs fully in the browser, uses no logins or private keys,
and reads only public data. It shows useful things about Kash markets that the main
app does not show yet.

> Community tool — not affiliated with Kash.

## Pages

- **⚡ Reality Check** — compares reported volume with real activity (unique traders,
  24h volume, trades per market). A transparency / data-quality view.
- **Insights** — volume and engagement by category, concentration, and the
  most-traded vs highest-volume markets side by side.
- **Resolution Calibration** — once markets resolve, checks whether prices were
  accurate (Brier score). Fills in over time.
- **🎯 Consistency** — confirms multi-outcome markets price cleanly (outcomes sum to
  100%, no hidden margin).
- **Markets** — searchable, filterable list of every live market.

See [OVERVIEW.md](OVERVIEW.md) for a plain-language description of each page.

## Run locally

It is a single static file. Just open `index.html`, or serve it:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy on GitHub Pages

1. Push this repo to GitHub.
2. Repo **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
3. Branch: `main`, folder: `/ (root)`. Save.
4. Your dashboard goes live at `https://<user>.github.io/<repo>/`.

## License

MIT — see [LICENSE](LICENSE).
