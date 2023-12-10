# dbdocs CI
Sample of GitHub Actions to execute CI for dbdocs.

## Workflow
- For pull requests to the main branch that are opened, synchronized, or closed, dbdocs is built using sample.dbml. 
  - If closed, the main branch is checked out for the build.
  - If not closed, the pull request's branch is checked out for the build.

## Requirements
Adding DBDOCS_TOKEN to the Repository secrets is required for dbdocs login. The method for generating this token can be found in the [official documentation](https://dbdocs.io/docs/ci-integration).

## Remarks
sample.dbml mirrors the content used in the [Getting Started section of the official documentation](https://dbdocs.io/docs).