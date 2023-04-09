## Branches

* `main` - This is the main branch only the admin maintainer can do a merge and should be from a `staging` which most pull-request are merged into except for hotfixes.
* `staging ` - This is a pre-release branch where updates after the pull-request gets aproved by QA, this version is a copy of `main` branch this is to avoid conflict when merging.
* `devel` - This contains all development updates. This is used for testing and compatibility between updates. Requires pull-request to merge with ongoing update for testing.

## Branch Prefixes
Apart from the main branches we will use branch prefix to properly organize individuals branches, this is usefull during development

* `bugfix/<issue #>-<bug short description>` - Typically used to fix Release branches.
* `hotfix/<name of hotfix>` - Used to quickly fix `main` branch without interrupting changes in the `devel` and `staging` branch.
* `feature/<name of the feature>` - Used for specific feature work or improvements. Generally branch from, and merge back into, the `staging` branch using pull requests.
* `release/<release version>` - Used for release task and long-term maintenance versions. They branch from, and merge back into, the `staging` branch.
