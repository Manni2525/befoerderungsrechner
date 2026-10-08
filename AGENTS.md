# Vorgaben für Agents

Nach jeder Änderung, die Nutzerinnen und Nutzer des Beförderungsrechners sehen, die Versionsseite in derselben Änderung fortschreiben.

Betrifft Verhalten, Texte, Daten und Layout in `index.html`. Reine Agent- oder Repository-Dateien, die an der Seite nichts ändern, bekommen keinen neuen Eintrag.

## Versionsseite

In `index.html`, neueste Fassung zuerst:

1. Neuen Block oben in `#view-versionen` einfügen.
2. Die Versionsnummer um 0.1 erhöhen. Dieselbe Nummer steht an drei Stellen: im neuen Block, im Satz „Aktuelle Fassung“ und im Footer-Link `Version x.y`.
3. Datum ist der Tag der Änderung, zum Beispiel `8. Oktober 2026`. Im Satz „Aktuelle Fassung“ steht nach dem Tag ein geschütztes Leerzeichen: `8.&nbsp;Oktober 2026`.
4. Kurze deutsche Stichpunkte: was sich bei der Nutzung ändert.

```html
<section class="version">
  <p class="version-meta"><span class="num">Version 1.8</span><span class="since">seit dem 9. Oktober 2026</span></p>
  <ul>
    <li>Kurze Zusammenfassung der Änderung.</li>
  </ul>
</section>
```

Aktueller Stand zum Anlegen dieser Vorgabe: **Version 1.7** seit dem 8. Oktober 2026. Die nächste sichtbare Änderung ist Version 1.8.

## Veröffentlichen

`main` geht nur noch nach `origin`: https://github.com/Manni2525/befoerderungsrechner.git

Die öffentliche Seite ist https://manni2525.github.io/befoerderungsrechner/

```
git push origin main
```

Kein Force-Push.
