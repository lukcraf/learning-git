# Pull Requests
view pull requests [here](https://github.com/lukcraf/learning-git/pulls)

## PR [#4](https://github.com/lukcraf/learning-git/pull/4)
The first pattern I've learned is this:
```bash
git checkout dev && git pull && git checkout -b pr4/pr-dev-uat-prod-tag-pattern
```
There seems to be a convention in naming branches, here's an error message: (#TODO: research)
> fatal: cannot lock ref 'refs/heads/pr4/pr-dev-uat-prod-tag-pattern': 'refs/heads/pr4' exists; cannot create 'refs/heads/pr4/pr-dev-uat-prod-tag-pattern'
we can proceed with:
```bash
git switch dev && git branch -D pr4 && git checkout -b pr4/pr-dev-uat-prod-tag-pattern
````
code...
```bash
git add . && git commit -m "PR4/sample pr to tagging release" && git push --set-upstream origin pr4/pr-dev-uat-prod-tag-pattern
```
