# matejmicek.github.io

Personal scratch space for hosting one-off static pages. Each subfolder is an independent drop, served at `https://matejmicek.github.io/<folder>/`.

## Add a new page

```bash
cd ~/Developer/matejmicek.github.io
mkdir <folder>
# put index.html (and any assets) inside
# add a row to the root index.html
git add . && git commit -m "<folder>" && git push
```

GitHub Pages auto-deploys from `main` branch root. Live in ~30 seconds.

## Drops

| Path | Date | What |
|------|------|------|
| `/exotic-woods/` | 2026-06-16 | Wood price gallery — wood-shop.cz exotic + domestic boards normalized to Kč/m³ incl. VAT, 39 species, finished/oiled photos on hover |
| `/superplane-other-git-activity/` | 2026-04-29 | Deep git-activity analysis on superplanehq/superplane |
| `/superplane-stars/` | 2026-04-28 | Stargazer EDA on superplanehq/superplane |
