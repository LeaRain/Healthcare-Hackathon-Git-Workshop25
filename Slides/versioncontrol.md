# Version Control -- Versionskontrolle

## Versionen und Zeitstempel

Reproduzierbarkeit eines Statuses -- von Dateien wie Code oder Daten  

slides.pdf vs. slidesfinal.pdf vs. slidesreallyfinal.pdf ... -> keine passende Versionskontrolle, lediglich Stand einer Datei mit final, reallyfinal, .. nicht eindeutig  

## Commit

Stand aller Dateien eines Projekts mit Zeitstempel dargestellt in einem langen Wert wie commit e351689decb3570c1cc2f7163cfeec24d2ac5ed3 (erster Commit dieses Projekts)

## Teamarbeit

Jedes Teammitglied kann Commit erzeugen durch eigene Änderungen von Dateien und Hinzufügen mit

```
git add <filename>
git commit -m "<commit message>"
git push
```

`add` -- Hinzufügen von Dateien zu aktuellen Stand  
`commit` -- Speichern eines Projektstatus
`push` -- Hochladen
