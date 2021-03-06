# Override GitHub Merge

This repository demonstrates the use of a GitHub Actions workflow to override the merge options as provided by GitHub. Refer to the Medium article https://medium.com/@_samkitjain/override-githubs-merge-strategies-cea7eb789e23 to know more.

## Prerequisites

1. Create a personal access token with the `public_repo` and `repo:status` permissions.
2. Create a repository secret by the name `GH_TOKEN` and add the token created above as the value.

## How to use?

1. Copy-paste the [merge.yml](.github/workflows/merge.yml) file into your repository.
2. Open a pull request.
3. Type in `/merge` as a comment in the pull request.

# Troubleshooting

1. If the workflow is not triggering, it could be because the workflow YAML file hasn't been merged into the default branch.
2. If you want to customise the validation checks or the merge strategy, edit the workflow YAML at will.
