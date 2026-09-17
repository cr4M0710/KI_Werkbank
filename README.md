# Werkbank — dein Blog

Eine einfache, selbstgebaute Blog-Vorlage aus HTML/CSS. Kein Framework,
keine Abhängigkeiten — du kannst jede Datei direkt im Editor bearbeiten.

## Struktur

```
blog/
├── index.html          ← Startseite mit der Beitragsliste
├── style.css           ← Gesamtes Design (Farben, Schrift, Layout)
└── posts/
    └── beispiel-post.html   ← Ein Beitrag; auch als Vorlage für neue Posts
```

## Kostenlos online stellen mit GitHub Pages

1. **Account & Repository:** Erstelle (falls noch nicht vorhanden) einen
   kostenlosen Account auf github.com. Lege ein neues Repository an, z. B.
   `werkbank-blog`.
2. **Dateien hochladen:** Lade den gesamten Ordnerinhalt (`index.html`,
   `style.css`, `posts/`) in das Repository hoch — entweder per Drag & Drop
   im Browser ("Add file" → "Upload files") oder per Git.
3. **Pages aktivieren:** Im Repository unter *Settings → Pages* die Quelle
   auf den `main`-Branch und den Root-Ordner (`/`) stellen und speichern.
4. **Fertig:** Nach ein bis zwei Minuten ist die Seite erreichbar unter
   `https://<dein-github-name>.github.io/werkbank-blog/`.
5. **Optional — eigene Domain:** Falls du später eine eigene Domain (z. B.
   `deinname.de`) verwenden willst, lässt sich das in den Pages-Einstellungen
   unter "Custom domain" hinterlegen (DNS-Eintrag beim Domain-Anbieter
   erforderlich, meist ~10 €/Jahr für die Domain selbst).

## Neuen Beitrag hinzufügen

1. Kopiere `posts/beispiel-post.html` und benenne die Kopie um
   (z. B. `posts/winkel-im-unterricht.html`).
2. Öffne die neue Datei und ersetze Titel, Kategorie-Punkt (`dot-mathe`,
   `dot-arbeitslehre`, `dot-making` oder `dot-sonstiges`), Datum und Text.
3. Öffne `index.html` und füge einen neuen `<li>`-Block oben in der Liste
   ein (Vorlage steht als Kommentar direkt in der Datei), der auf die neue
   Seite verlinkt.
4. Änderungen zu GitHub hochladen — die Seite aktualisiert sich automatisch.

## Design anpassen

Alle Farben und Schriften stehen gesammelt oben in `style.css` unter
`:root { ... }`. Wenn du z. B. die Akzentfarbe ändern willst, reicht es,
den Wert von `--rust` anzupassen — er wird überall automatisch übernommen.
