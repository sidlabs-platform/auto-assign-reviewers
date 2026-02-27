# Auto Assign Copilot Reviewer

A GitHub Actions workflow that automatically assigns **GitHub Copilot** as a reviewer on pull requests.

## How It Works

1. A pull request is opened or a label is added to an existing PR.
2. The workflow checks if the PR has a label called `test`.
3. If the label is present, GitHub Copilot is automatically added as a reviewer.

## Setup

No additional setup is required beyond having this workflow in your repository. The workflow uses the built-in `GITHUB_TOKEN` for authentication.

## Usage

- Open a pull request and add the `test` label to trigger an automatic Copilot review.
- When new commits are pushed to a PR with the `test` label, Copilot review is automatically re-triggered.
