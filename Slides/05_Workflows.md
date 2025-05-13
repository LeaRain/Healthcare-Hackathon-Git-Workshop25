# Übliche Workflows

## Repository von Remote(server) lokal klonen

```bash
git clone <repo>
```

## Git Initial Einrichten

```bash
git config --global user.name "<name>"
git config --global user.email "<email>"
```

Testen der Einstellungen mit:
```bash
git config list
```

## Featureentwicklung auf eigenem Branch entwickeln

1. Update der Informationen des Repos auf den neusten Stand:
```bash
git checkout main
git fetch
```
2. Status des Repos überprüfen (`git log --graph`, `git status`)
3. Repo updaten:
```bash
git pull
```
4. Dann einen neuen Branch erstellen und daran arbeiten:
```bash
git branch "<branch>"
git checkout "<branch>"
```
5. Status des Branches überprüfen (`git log --graph`, `git status`)
6. Arbeiten und Committen (`git add`, `git commit`, `git push`)
7. Neuen Pull-Request erstellen (auf GitHub)
    1. Review von Branch (auf GitHub, am besten durch Kollegen)
    2. Wenn passt: Merge auf Branch `main` (auf GitHub)

## Merge-Konflikte

- Ursachen
    - Zusammenführen von Branches mit konkurrierende Commits
    - 2 Commits auf demselben Branch mit demselben Parent
- Anzeige im File mithilfe von Konfliktmarkern
```
lorem ipsum
<<<<<< HEAD
Version A
=======
Version B
>>>>>> <branch>
lorem ipsum
```
- Editieren der Änderungen und entfernen der Konfliktmarker
- Neuen Stand committen

## Code analysieren

Übersicht über alle Commits und Branches:
```bash
git log --graph --all
```
