# LiveKit Sandbox Deploy Action

A reusable GitHub Action to deploy a LiveKit Sandbox instance to a target production branch. Increments the version tag if deployment is

## Inputs

- `token`: A GitHub token with permissions to push to the repository.
- `production_branch` (optional): The branch to mirror the `main` branch to. Default is `sandbox-production`.

## Versioning

The action automatically increments the version tag in the format `vX` where `X` is an integer. Each deployment to the production branch increases this integer by 1. If no such tag exists, it starts from `v1`.
