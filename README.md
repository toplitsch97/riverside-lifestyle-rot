# Riverside Lifestyle — Hub-Portal

Statische Portal-Landingpage (HTML/CSS/JS, kein Build) für die Dachmarke **Riverside Lifestyle**.
Drei full-bleed Video-Panels (Auto-Spotlight) verlinken auf die Marken **Ink** (Tattoo), **Beauty** und **Gastro**.
Look: dunkel, rot/weiß/schwarz, Cormorant Garamond + Inter.

## Lokal starten
```bash
python3 -m http.server 8078
# http://localhost:8078
```

## Aufbau
- `index.html` — Portal: Hero mit 3 Video-Panels, die direkt auf die Marken-Homepages weiterleiten.
- `css/styles.css`, `js/main.js` — Styling + Auto-Spotlight (nur das aktive Panel spielt Video).
- `impressum.html`, `agb.html`, `datenschutz.html` — Rechtsseiten (Vorlagen mit Platzhaltern).
- `robots.txt`, `llms.txt` — Suchmaschinen + KI-Crawler.
- JSON-LD in `index.html`: `Organization` + `TattooParlor`/`BeautySalon`/`Restaurant`.

## Noch zu ersetzen (Platzhalter, im Code mit `TODO` markiert)
- **Marken-Links**: Beauty + Gastro zeigen auf `#` (Ink → riverside-ink.ch).
- **Videos** `assets/video/beauty.mp4`, `gastro.mp4`, `ink.mp4` — Stock-Platzhalter (Mixkit, frei). Gegen echtes Material tauschen (gleiche Dateinamen).
- **Rechtstexte**: alle `[Platzhalter]` in Impressum/AGB/Datenschutz mit echten Daten füllen, juristisch prüfen lassen.
- Datenschutz: Google Fonts werden extern geladen — für strikte DSGVO lokal hosten.
