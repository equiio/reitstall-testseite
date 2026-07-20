# Reitstall-Testseite

Eine statische Test-Webseite für das equiio-Reitstallkonzept. Sie besteht aus HTML, CSS, JavaScript und optimierten Bilddateien.

## Dateien

- `index.html` enthält die Startseite und Bereichsauswahl.
- `anlage.html`, `einsteller.html`, `schulbetrieb.html`, `digitales.html` und `aktuelles.html` enthalten die Unterseiten.
- `content/beitraege.json` enthält zentral alle Neuigkeiten.
- `home.css`, `style.css`, `bereiche.css` und `aktuelles.css` enthalten die Gestaltung und Smartphone-Anpassungen.
- `script.js`, `bereich-demo.js` und `aktuelles.js` enthalten die lokalen Demo-Funktionen.
- `assets/` enthält die Bilder; Beitragsbilder liegen unter `assets/aktuelles/`.

## Neuen Beitrag hinzufügen

1. Das optimierte Beitragsbild unter `assets/aktuelles/` ablegen.
2. In `content/beitraege.json` ein neues Objekt ergänzen.
3. `titel`, `date` im Format `JJJJ-MM-TT`, `kurztext`, `text` als Liste von Absätzen, `image` und einen aussagekräftigen `alt`-Text ausfüllen.
4. Für Musterinhalte `demo` auf `true` setzen; reale Beiträge erhalten `false`.

Die Beiträge müssen nicht von Hand sortiert werden. `aktuelles.js` zeigt automatisch das neueste Datum oben vollständig und ältere Beiträge darunter geschlossen an. Ein neuer Beitrag kann künftig aus einem Foto und einigen Stichpunkten erstellt werden, solange Bildrechte, Inhalt und Alternativtext vor der Veröffentlichung geprüft werden.

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
