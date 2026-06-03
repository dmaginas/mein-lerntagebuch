# Was gelernt? 

Wie man mit `git log` und `git diff` die Commit-Historie durchsucht

# Welches Problem? 

Ich wusste nicht mehr, in welchem Commit ich eine bestimmte Änderung gemacht hatte

# Wie gelöst?

Mit `git log --oneline` eine kompakte Übersicht geholt und dann mit `git diff` den Unterschied zwischen zwei Commits verglichen:

```
git log --oneline
git diff abc1234 def5678
```

Zusätzlich `git log --grep="Suchbegriff"` verwendet, um gezielt nach Commit-Nachrichten zu suchen.
