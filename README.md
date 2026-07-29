# Marc Bertsch Immobilien – Website

Fertiger Astro-Code für bertsch-immo.de. Diese README ist die Kurzfassung –
die ausführliche Klick-für-Klick-Anleitung (GitHub → Netlify → Domain bei
STRATO) hast du separat als PDF/Chat-Nachricht bekommen.

## Lokal testen (optional, nur falls du Node.js installiert hast)

```bash
npm install
npm run dev
```

Öffnet unter http://localhost:4321

## Struktur

```
src/pages/       → jede Datei = eine Seite (index.astro = Startseite)
src/layouts/      → gemeinsames Grundgerüst (Header, Footer, Meta-Tags)
public/images/    → alle Fotos & das Logo
public/styles/    → das komplette Design (Farben, Schriften, Layout)
netlify.toml      → Build-Einstellungen für Netlify
```

## Wichtige offene Punkte (bitte vor dem Launch erledigen)

- **Impressum**: Erlaubnisnummer nach § 34c GewO fehlt noch (in
  `src/pages/impressum.astro` als TODO markiert)
- **Datenschutzerklärung**: Vor Launch von einem Generator (z. B. e-recht24)
  oder Anwalt final prüfen lassen
- **Formulare**: Laufen über Netlify Forms – funktionieren automatisch,
  sobald die Seite auf Netlify deployed ist (nicht schon im lokalen Test)

## Texte oder Bilder ändern

Alle Texte stehen direkt in den `.astro`-Dateien unter `src/pages/` – ganz
normaler HTML-Text, auch ohne Programmierkenntnisse auffindbar und änderbar.
Bilder einfach in `public/images/` austauschen (gleicher Dateiname behalten,
dann muss nichts im Code angepasst werden).
