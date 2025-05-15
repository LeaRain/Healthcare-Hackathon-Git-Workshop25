# Konzepte

## Git-Konzepte

| Konzept      | Erklärung                                                                 |
| ------------ | ------------------------------------------------------------------------- |
| Repo(sitory) | Projekt mit Quellcode                                                     |
| Commit       | Spezifischer Stand eines Projekts                                         |
| Branch       | Separater Teil eines Projekts (häufig für einzelne Features, Issues, ...) |
| Tag/Label    | Spezifischer Commit mit Annotation                                        |
| Merge        | Zusammenführen von zwei verschiedenen Ständen                             |

## GitHub-Konzepte

| Konzept      | Erklärung                                                     |
| ------------ | ------------------------------------------------------------- |
| Issue        | Offener Punkt im Projekt (Fehler/Bug aber auch neue Features) |
| Pull Request | Vorschlag zum Zusammenführen von zwei Branches                |

## Basis Kommandos von Git

### Status

Aktuelle Status der Änderung an Dateien im Repo anzeigen.
```bash
git status
```

### Add

Hinzufügen einer neuen Datei oder eines neuen Stands einer bestehenden Datei.

```bash
git add <file>
```

### Diff

Differenzen zwischen dem aktuellen Stand des lokalen Repos und dem eingecheckten Stand anzeigen.
```bash
git diff
```

Geht auch für einzelne Files:
```bash
git diff <file>
```

### Commit

Stand aller Dateien eines Projekts mit Zeitstempel dargestellt in einem langen Wert wie der Commit `e351689decb3570c1cc2f7163cfeec24d2ac5ed3` (erster Commit dieses Projekts)

```bash
git commit -m "<message>"
```

Am besten mit der Option `-m` gleich ein Commit-Message setzen.

### Server Kommandos von Git

### Clone

Kopieren eines Repos mit ...
- allen Daten
- allen Branches
- der gesamten Historie

```bash
git clone <repo>
```

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

## Speziellere Kommandos

### Reset

De-stagen der Änderungen an einem File.
```bash
git reset <file>
```

Zurücksetzen **aller Änderungen** an einem File auch möglich, **Dateiverlust möglich!**
```bash
git reset --hard <file>
```

### Branch

Erstellen eines neuen Branches:
```bash
git branch <branch>
```

### Switch

Wechseln zu einem Branch:
```bash
git switch <branch>
```

### Merge

Zusammenführen von Branches:
```bash
git merge <branch>
```

### Config

Einstellen der Konfiguration von Git.
```bash
git config
```

### Log

Informationen zur Historie des Repos:
```bash
git log
```

