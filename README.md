# Workflows

GitHub Actions のレシピと Reusable Workflow の置き場。

## Recipes

[.github/recipes](/.github/recipes)

## Reusable workflows

[ワークフローの再利用 \- GitHub Docs](https://docs.github.com/ja/actions/using-workflows/reusing-workflows)

### 使い方

```yaml
name: test

on:
  pull_request:
  push:
    branches:
      - main

jobs:
  test:
    uses: x7ddf74479jn5/workflows/.github/workflows/label.yaml@main
```

[.github/workflows](/.github/workflows)
