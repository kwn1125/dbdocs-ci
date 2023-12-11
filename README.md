# dbdocs CI
Sample of GitHub Actions to execute CI for [dbdocs](https://dbdocs.io).

## Workflow
When a pull request to the main branch is opened, synchronized, reopened, or closed, dbdocs is built using sample.dbml.
- If closed, the main branch is checked out for the build.
- If not closed, the pull request's branch is checked out for the build.

## Requirements
Adding DBDOCS_TOKEN to the [repository secrets](https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions#creating-secrets-for-a-repository) is required for dbdocs login. The method for generating this token can be found in the [official documentation](https://dbdocs.io/docs/ci-integration).

## Remarks
The content of sample.dbml is the same as that used in the Getting Started section of the [official documentation](https://dbdocs.io/docs).