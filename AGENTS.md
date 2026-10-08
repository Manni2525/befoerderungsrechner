# Vorgaben für Agents

Nach jeder Änderung, die Nutzerinnen und Nutzer des Beförderungsrechners sehen, die Versionsseite in derselben Änderung fortschreiben.

Betrifft Verhalten, Texte, Daten und Layout in `index.html`. Reine Agent- oder Repository-Dateien, die an der Seite nichts ändern, bekommen keinen neuen Eintrag.

## Versionsseite

In `index.html`, neueste Fassung zuerst. Pro Kalendertag höchstens eine Versionsnummer. Mehrere Änderungen desselben Tages in den Stichpunkten dieses einen Blocks zusammenfassen. Überholte Zwischenschritte desselben Tages nicht einzeln stehen lassen, sondern den Stand am Ende des Tages beschreiben.

1. Liegt der oberste Block schon auf dem Tag der Änderung, die Nummer nicht erhöhen. Neue Stichpunkte in diesen Block einfügen.
2. Nur wenn der oberste Block ein anderes Datum trägt, einen neuen Block darüber setzen und die Versionsnummer um 0.1 erhöhen.
3. Dieselbe Nummer steht an drei Stellen: im Block des Tages, im Satz „Aktuelle Fassung“ und im Footer-Link `Version x.y`.
4. Datum ist der Tag der Änderung, zum Beispiel `9. Oktober 2026`. Im Satz „Aktuelle Fassung“ steht nach dem Tag ein geschütztes Leerzeichen: `9.&nbsp;Oktober 2026`.
5. Kurze deutsche Stichpunkte: was sich bei der Nutzung ändert.

```html
<section class="version">
  <p class="version-meta"><span class="num">Version 1.4</span><span class="since">seit dem 9. Oktober 2026</span></p>
  <ul>
    <li>Kurze Zusammenfassung der Änderung.</li>
  </ul>
</section>
```

Aktueller Stand: **Version 1.4** seit dem 9. Oktober 2026. Eine weitere sichtbare Änderung an diesem Tag ergänzt die Stichpunkte von 1.4. Die nächste Nummer ist 1.5, am ersten späteren Tag mit einer sichtbaren Änderung.

## Veröffentlichen

`main` geht nur noch nach `origin`: https://github.com/Manni2525/befoerderungsrechner.git

Die öffentliche Seite ist https://manni2525.github.io/befoerderungsrechner/

```
git push origin main
```

Kein Force-Push. Das alte Repository `wann-endlich-a9z` bleibt bestehen und leitet nur noch auf https://manni2525.github.io/befoerderungsrechner/ weiter. Nicht löschen.
