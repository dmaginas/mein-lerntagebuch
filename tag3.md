# Was gelernt? 

Den Unterschied zwischen `git merge` und `git rebase`

# Welches Problem? 

Nach dem Mergen hatte ich unübersichtliche Merge-Commits in der Historie

# Wie gelöst?

Beim nächsten Mal `git rebase main` im Feature-Branch verwendet, um eine lineare Historie zu bekommen:

```
git checkout feature-branch
git rebase main
git checkout main
git merge feature-branch
```
