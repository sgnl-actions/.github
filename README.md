# .github

Shared GitHub configuration for the `sgnl-actions` organization.

## Reusable Workflows

### CI (`ci.yml`)

Full CI pipeline for SGNL action repos: install, package-lock sync check, validate metadata, lint, test, build, verify dist.

```yaml
# In your repo's .github/workflows/ci.yml:
name: CI

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]
  workflow_call:

jobs:
  ci:
    uses: sgnl-actions/.github/.github/workflows/ci.yml@main
```

### Release (`release.yml`)

Manual release workflow: runs CI gate, computes next semver from tags, creates annotated tag and GitHub Release.

```yaml
# In your repo's .github/workflows/release.yml:
name: Release

on:
  workflow_dispatch:
    inputs:
      bump:
        description: 'Version bump type'
        required: true
        type: choice
        options:
          - patch
          - minor
          - major

jobs:
  ci:
    uses: sgnl-actions/.github/.github/workflows/ci.yml@main

  release:
    needs: ci
    uses: sgnl-actions/.github/.github/workflows/release.yml@main
    with:
      bump: ${{ inputs.bump }}
    permissions:
      contents: write
```
