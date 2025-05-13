# Übliche workflows
## Repository von Remote(Server) lokal klonen
git clone "URLTOREPOSITORY"
## git initial einrichten
git config --global user.name "Your Username"
git config --global user.email "YourEmail@example.com"

testen mit:
git config list

## Feature X auf eigenem Branch entwickeln und dann via pull-request auf den branch "main" mergen
Zuerst neuesten Stand von Server holen
    git checkout main
    git fetch
    prüfen, ob alles passt (git log --graph, git status,...)
    git pull

Dann Branch "feature_x" erstellen und daran arbeiten
    git branch "feature_x"
    git checkout "feature_x"
    testen mit git status
    arbeiten und committen (git add, git commit)

Dann Pull Request erstellen (auf github)
    Review von Branch (auf github)
    wenn passt: merge auf branch "main" (auf github)

## merge-konflikte
Sobald Merge-Konflikt, wird das angezeigt.
Heißt, dass der aktuelle stand 2 parent-commits hat (A und B)
In allen Dateien mit Konflikt wird A und B wie folgt angezeigt:
    If you have questions, please
    <<<<<<< HEAD
    A open an issue
    =======
    B ask your question in IRC.
    >>>>>>> branch-a

wenn konflikt gelöst ist, datei mit "git add DATEI" adden
dann wieder git commit
fertig

## code analysieren
git log --graph --all
    zeigt Übersicht aller commits und branches


