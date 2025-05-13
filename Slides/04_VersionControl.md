# Version Control -- Versionskontrolle

## Versionen und Zeitstempel

Reproduzierbarkeit eines Statuses -- von Dateien wie Code oder Daten  

slides.pdf vs. slidesfinal.pdf vs. slidesreallyfinal.pdf ... -> keine passende Versionskontrolle, lediglich Stand einer Datei mit final, reallyfinal, .. nicht eindeutig

## Teamarbeit

Jedes Teammitglied kann Commits erzeugen durch eigene Änderungen von Dateien und Hinzufügen mit

```bash
git add <filename>
git commit -m "<commit message>"
git push
```

## Arbeit mit Git als Versionskontrolle

### Clone

Kopieren eines Repos mit ...
- allen Daten
- allen Branches
- der gesamten Historie

```bash
git clone <repo>
```

### Add

Hinzufügen einer neuen Datei oder eines neuen Stands einer bestehenden Datei.

```bash
git add <file>
```

### Diff

Differezen zwischen dem aktuellen Stand des lokalen Repos und dem eingecheckten Stand anzeigen.
```bash
git diff
```

Geht auf für einzelne Files:
```bash
git diff <file>
```


### Commit

Stand aller Dateien eines Projekts mit Zeitstempel dargestellt in einem langen Wert wie der Commit `e351689decb3570c1cc2f7163cfeec24d2ac5ed3` (erster Commit dieses Projekts)

```bash
git commit -m "<message>"
```

Am besten mit der Option `-m` gleich ein Commit-Message setzen.

### Push

Hochladen aller Commits zum Remote-Repo

```bash
git push
```

### Fetch

Herunterladen der Informationen zu Änderungen im Remote-Repo.
```bash
git fetch
```

### Pull

Herunterladen und Anwenden der Änderungen im Remote-Repo.
```bash
git pull
```

### Branch

Erstellen eines neuen Branches:
```bash
git branch <branch>
```

### Checkout

Wechseln zu einem Branch:
```bash
git checkout <branch>
```

### Merge

Zusammenführen von Branches:
```bash
git merge <branch>
```

### Log

Informationen zur Historie des Repos:
```bash
git log
```

