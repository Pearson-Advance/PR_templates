## PR Template Updater

This repository contains a GitHub Actions workflow that automatically updates a target repository’s Pull Request (PR) template using a local Markdown file. By running this workflow, you can keep your PR template consistent across multiple repositories without manually copying and pasting the content each time.

## How It Works

- The workflow reads your PR template content from a Markdown file (for example, plugin_template.md) in this repository.
- It uses the GitHub CLI (gh) to clone the target repository where you want the updated PR template.
- The workflow creates (or updates) a branch in the target repository, writes your Markdown content to .github/PULL_REQUEST_TEMPLATE.md, and pushes the changes.
- Finally, the workflow opens a PR in the target repository, letting you review and merge the updated template.
