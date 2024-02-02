# Conventions

This repository contains guidelines for developing any future Horace Greeley robotics. The repository contains structural and architectural guidelines as well as linting preferences. If any formatting and/or guideline changes in the future, please update this repository.

## Version control

Horace Greeley High School Robotics uses ``git`` as its primary version manager.

Each unique codebase should have a separate repository.

#### Branching

We use primarily branching instead of tags.
Each production codebase should have a developer (``dev``) a testing (``test``) and a stable (``stable``) branch.
Always set the default branch to ``dev``.
You should always use the ``dev`` branch to update, push or modify code. Never push into higher level (``test`` or ``stable``) branches. The only way to update such branches is with a reviewed merge.
You can move up semi-stable code from the ``dev`` to ``test`` but never two steps at a time. You can only move up well-tested code from ``test`` to ``stable``.
Any new branch can only be merged into the ``dev`` branch.
Branch names have to be lower case and hyphen separated. Do not have trailing or continuous hyphens. The branch name should only include alphanumeric characters and have a descriptive name.

#### CI/CD

For any CI/CD operation we use Github's built-in Actions.

### Commit conventions

A commit message should be a maximum of 72 characters.
It should be always in imperative.
Always capitalize and start the commit message with a verb (e.g. Add, Change, Fix, Remove)
Describe what you changed/added.

#### Merge reviews

Every branch should be protected by rules through Github.
A pull request is required for every merge attempt.
At least one review is required to merge a branch.