# Was gelernt? 

Wie man mit `git branch` und `git checkout` zwischen Branches wechselt

# Welches Problem? 

Ich habe aus Versehen Änderungen im falschen Branch gemacht

# Wie gelöst?

Mit `git stash` die Änderungen zwischengespeichert, dann in den richtigen Branch gewechselt und mit `git stash pop` wieder eingefügt:

```
git stash
git checkout feature-branch
git stash pop
```
