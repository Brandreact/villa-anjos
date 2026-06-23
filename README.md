# Villa Anjos — Landingpage

Exklusive One-Page-Landingpage für die Luxusvilla **Villa Anjos** in Ponta do Sol, Madeira
(privater Salzwasser-Infinity-Pool · Meerblick · 5 Gäste · 3 Master-Suiten · 4 Bäder).

## Tech-Stack

- Eine einzige, eigenständige Datei: [`index.html`](index.html)
- **Tailwind CSS** (Play-CDN) + Custom-CSS
- Schriften: **Cormorant Garamond** (Headlines) · **Inter** (Fließtext)
- Vanilla JavaScript (kein Build-Schritt nötig)

## Struktur

Hero · Das Anwesen (Key-Facts) · Ausstattung · Galerie (Lightbox) · Lage · Buchungsanfrage · Footer

## Lokal starten

Da es eine statische Datei ist, genügt ein beliebiger Static-Server:

```bash
python3 -m http.server 4173
# → http://localhost:4173
```

## Bilder

Die Galerie wird dynamisch aus dem `PHOTOS`-Array (unten im `<script>`) gerendert.
Aktuell laden die Bilder von den CDNs der Inserate (Airbnb / Booking.com).

> **Für Produktion empfohlen:** Original-Fotos herunterladen und selbst hosten
> (`/assets/…`), um unabhängig von den Plattform-CDNs und Signatur-Hashes zu sein.

## Produktions-Hinweise

- Tailwind statt Play-CDN per CLI/PostCSS zu statischem CSS kompilieren.
- Buchungsformular nutzt aktuell einen `mailto:`-Fallback (kein Backend) →
  bei Bedarf an einen Endpoint (z. B. Formspree / eigene API) anbinden.
- `Impressum` / `Datenschutz` sind Platzhalter-Links.

## Kontakt

Buchungsanfragen: **villa.anjos.gb@gmail.com**
