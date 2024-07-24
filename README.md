# PIDDatabase
To use the database, you'll need SQLite3 and Git installed.

Commands to set it up (ignore "not a database" errors, it's fixing that):
```
git clone https://github.com/UMSKT/PIDDatabase
git config --local include.path ../.gitconfig
git stash save -u
rm .git/index
git checkout HEAD -- "$(git rev-parse --show-toplevel)"
git stash pop
```

Commits made to the repository will be converted back into plain text automatically.
