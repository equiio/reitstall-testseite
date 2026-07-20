# Reitstall-Testseite

Eine statische Test-Webseite für das equiio-Reitstallkonzept. Sie besteht aus HTML, CSS, JavaScript und optimierten Bilddateien.

## Dateien

- `index.html` enthält die Startseite und Bereichsauswahl.
- `anlage.html`, `einsteller.html`, `schulbetrieb.html` und `digitales.html` enthalten die Unterseiten.
- `home.css`, `style.css` und `bereiche.css` enthalten die Gestaltung und Smartphone-Anpassungen.
- `script.js` und `bereich-demo.js` enthalten die lokalen Demo-Funktionen.
- `assets/` enthält die Bilder.

## Deployment

Das Repository ist mit **IONOS Deploy Now** verbunden.

- Produktionsbranch: `main`
- Maßgebliche öffentliche Testadresse: https://home-5020967539.app-ionos.space
- Zusätzliche Testadresse über GitHub Pages: https://equiio.github.io/reitstall-testseite/
- Jeder Push auf `main` löst automatisch ein neues IONOS-Deployment aus.

Vor jeder Veröffentlichung müssen mindestens folgende Punkte geprüft werden:

1. HTML-Struktur und interne Links
2. CSS und responsive Darstellung
3. JavaScript ohne Syntaxfehler
4. Darstellung auf Desktop und Smartphone
5. Vorhandensein aller referenzierten Bilder und Dateien

Nach der Veröffentlichung ist zuerst die IONOS-Testadresse zu kontrollieren. GitHub Pages dient nur als zusätzliche Testmöglichkeit.

### Geschützte IONOS-Dateien

Die Dateien unter `.github/workflows/` werden von IONOS Deploy Now verwaltet. Sie dürfen nicht gelöscht, verschoben oder ohne ausdrückliche Anweisung verändert werden.
