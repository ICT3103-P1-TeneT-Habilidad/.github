# TeneT Workflow

This document describes the management and structure of branches.

## Branch Stucture

- [Regular branches](#regular-branch) must always build without failure.
- Every branch serves a single purpose.

## Regular Branch

### `main`

Main branch for this repository. Do not commit directly to this branch.

### `dev`

Default branch for development. Do not commit directly to this branch.

## Branch Semantics

Aside from regular branches like Main and Dev, all branches shall follow semantics below in creating a new branch.

### Branch Type

The followings are types of branch.

- `feat`: refers to feature branch
- `bug`: refers to bug fix and improvement branch

### Create a new branch

All new branch should be branch off from `dev` branch. Every new branch shall follow rules and the naming convention as stated below.

- `<type>/<server/client>/<name>`
- all texts should be in lowercase
- `type` block refers to type of branch and `name` block refers to **name of the feature** or **issue number**
- Separate words with `_` for blocks with more than one word

Examples:

- `feat/client/login_ui`
- `feat/server/login_api`
- `bug/20`

## Branch Commit

## Commit Message Type

- `feat` - new feature
- `fix` - a bug fix
- `refactor` - changes that is not related to feature or fix
- `style` - changes that does not affect the codes, related to code formatting
- `test` - including new or correcting previous tests

## Commit Messages

Adapted from [FreeCodeCamp](https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/).

Team members are required to commit messages using this pattern.
`<Commit Type>: <Description>`

Examples:

- `feat: added login function`
- `fix: fixed #<issues number>`
- `style: removed whitespaces and empty lines`

## Branch Merging

The followings are requirements for merging a branch.
Branches must

- pull lattest changes from the branches they make merge request to.
- not merge directly into Main or Dev branches. Instead, create pull request for merging branches
