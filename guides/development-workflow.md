# How to gitflow with us?

## 1. Check and switch branch you are

`git branch`

To be sure that you are on `dev` branch, if not please switch to `dev`:

`git checkout dev`

## 2. Create `feature` or `hotfix` branch

`git checkout -b feature/1-link-to-demo`

> feature - All non-trivial changes should be done on feature branches and undergo code review before being merged into the master branch

> hotfix - Hotfix branches would branch off of the dev branch, and be used for minor post-release bugfixes

### Naming convention

* feature/xxx-some-short-description
* hotfix/xxx-some-short-description

where `xxx` is an issue ID from GitHub repository

## 3. Commit changes

## 4. Push feature branch to remote

`git push -u origin feature/xxx-some-short-description`

## 5. Create pull request on GitHub by visiting the url like below

`https://github.com/EscrowX/landing-page/compare/dev...feature/xxx-some-short-description`

## 6. Match [tkowalczyk](https://github.com/tkowalczyk) as reviewer and assign pull request to him

## 7. Link pull request with an issue by typing in pull request description

`close #XXX`, where `xxx` is an issue ID from GitHub repository

If pull request is from feature branch to dev branch use `squash and merge`, if pull request is from dev branch to main use `merge` commit

## 9. Delete feature branch