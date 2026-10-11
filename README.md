# Week-ahead econ calendar (12–21 Oct 2026)

Static page: browse events by day or by country, with a short summary per tab, text filter and a "key events only" toggle. No build step or dependencies.

## Deploy on GitHub Pages
1. Create a repo and add `index.html` at the root.
2. Settings → Pages → Deploy from branch → `main` / root.
3. Open `https://<user>.github.io/<repo>/`.

## Update the data
Edit the `D` array in `index.html`. Each row is:
`[day, time, country, event, period, previous, estimate, key(1/0), note]`
Add day/country summaries in the `DAY` and `CTY` objects.

## Sources and caveats
- Times are London (BST), as in the TradingEconomics paste.
- Only key events are included; most bill and bond auctions are omitted.
- Estimates come from the TE consensus, else forecast, else MNI/ITC.
- Argentina's September CPI previous annual rate differs between sources (33.7% TE, 33.5% MNI).
