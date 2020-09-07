# open-x-day
A template to use when starting a new project.

## perform a repository wide search and replace for "open-x-day" and the "target-repo-name"

e.g. by using

```
cp -R open-x-day/ new-name && cd new-name && git config --local --unset remote.origin.url && git config --local --add remote.origin.url git@github.com:baloise/new-name.git && git reset --hard $(git commit-tree FETCH_HEAD^{tree} -m "Initial contribution") &&  git grep -l 'open-x-day' | xargs sed -i '' -e 's/open-x-day/new-name/g' && mvn clean verify && git add -A && git commit -m "Rename from template to new-name" && cd ..
```
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io#https://github.com/baloise/open-x-day)

## the [docs](docs/index.md)
