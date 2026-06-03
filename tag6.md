# Was gelernt? 

Wie man mit `git reset` und `git revert` Änderungen rückgängig macht

# Welches Problem? 

Ich habe einen fehlerhaften Commit gepusht und wollte ihn rückgängig machen

# Wie gelöst?

Da der Commit bereits auf GitHub lag, habe ich `git revert` statt `git reset` benutzt, um einen neuen Gegen-Commit zu erzeugen:

```
git revert HEAD
git push
```

Merke: `git reset` eignet sich nur für lokale, noch nicht gepushte Commits. Bei gepushten Commits immer `git revert` verwenden, um die Historie nicht zu zerstören.
