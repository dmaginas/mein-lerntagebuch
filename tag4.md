# Was gelernt? 

Wie man mit `.gitignore` bestimmte Dateien vom Tracking ausschließt

# Welches Problem? 

Ich habe versehentlich eine Datei mit sensiblen Daten (API-Key) committed

# Wie gelöst?

Eine `.gitignore`-Datei erstellt und die Datei nachträglich aus dem Tracking entfernt:

```
echo "secrets.txt" >> .gitignore
git rm --cached secrets.txt
git commit -m "Sensible Datei aus Tracking entfernt"
```

Wichtig: Da der API-Key bereits in der Git-Historie war, musste ich den Key beim Anbieter neu erzeugen und den alten ungültig machen. Einmal gepusht, gilt ein Secret als kompromittiert!
