# Gekkoo-essen — versie 2 van de Gekkoo-site

Dit project is een **onafhankelijke kopie** van de GekkooPedia-vrijwilligersgids
(origineel: `C:\Users\victor\projecten\website`). Het bestaat **náást** de
originele site en mag een eigen kant op evolueren, met andere doeleinden.

> Het concrete doel van versie 2 wordt nog bepaald. Tot dan is dit een
> identieke startkopie van de originele site.

## Git & deployment — BELANGRIJK

- Dit project heeft een **eigen, aparte GitHub-remote**. Push **uitsluitend**
  naar die eigen remote.
- Push **NOOIT** naar de remotes van de originele site
  (`gekkoopedia` = victorvansande/gekkoopedia, of `origin` = victorvansande/website).
- **Auto-push**: na elke afgeronde wijziging meteen `git add` + `git commit` +
  `git push` naar de eigen remote, zonder eerst te vragen.
- Vergeet bij elke wijziging de **service-worker cacheversie** te bumpen
  (`service-worker.js`, constante `CACHE`), zodat bezoekers de nieuwste versie krijgen.

## Over de site

- Statische SPA (geen build-stap): `index.html` + `style.css` + `script.js`
  (+ `game.js`, `game2.js`, `game3.js`, `regio.js`).
- Navigatie via `showView(id, push)` met de History API.
- Service worker: HTML/CSS/JS network-first, statische assets cache-first.
- Glassmorphism via `backdrop-filter` (altijd ook de `-webkit-`-prefix erbij voor Safari/iOS).
- Dev server / preview draait via de config in `.claude/launch.json`.

## Contentrichtlijn (overgenomen van het origineel)

- Gebruik de exacte woorden **"klare taal"** niet op de site.
