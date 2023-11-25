# Pull Requests
view pull requests [here](https://github.com/lukcraf/learning-git/pulls)

## PR [#1](https://github.com/lukcraf/learning-git/pull/1)
The first pattern I've learned is this:
```bash
git checkout dev && git pull && git checkout -b pr1/pr-dev-uat-prod-tag-pattern
```
There seems to be a convention in naming branches, here's an error message: (#TODO: research)
> fatal: cannot lock ref 'refs/heads/pr1/pr-dev-uat-prod-tag-pattern': 'refs/heads/pr1' exists; cannot create 'refs/heads/pr1/pr-dev-uat-prod-tag-pattern'
we can proceed with:
```bash
git switch dev && git branch -D pr1 && git checkout -b pr1/pr-dev-uat-prod-tag-pattern
```
code...
```bash
git add . && git commit -m "PR1/sample pr to tagging release"
```

