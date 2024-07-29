# PIDDatabase
To use the database, you can:
* Use our neat little [web-based viewer](https://umskt.github.io/PIDDatabase-viewer/).
* Download the database/backup through the Releases tab.
* Clone the repository through the instructions below.

## Cloning
You'll need SQLite3 **3.46.0 or higher** and Git installed.

Commands to set it up (ignore "not a database" errors, it's fixing that):
```
git clone https://github.com/UMSKT/PIDDatabase
git config --local include.path ../.gitconfig
git stash save -u
rm .git/index
git checkout HEAD -- "$(git rev-parse --show-toplevel)"
git stash pop
```

To commit to the repository, run these commands:
```
git add .
git commit -m "your commit message"
git push
```
You will need to add the `git add .`, Git will yell at you otherwise.
