# Was gelernt? 

Wie man mit GitHub Issues und Commit-Referenzen seinen Workflow organisiert

# Welches Problem? 

Meine Commits hatten keine klare Verbindung zu den Aufgaben, die ich bearbeitet habe

# Wie gelöst?

Auf GitHub ein Issue erstellt und in der Commit-Nachricht darauf verwiesen. Dadurch wird der Commit automatisch mit dem Issue verknüpft:

```
git commit -m "Fix: Tippfehler in README behoben, closes #1"
```

Mit dem Schlüsselwort `closes` wird das Issue beim Merge automatisch geschlossen. So bleibt der Überblick, welcher Commit welches Problem gelöst hat.
