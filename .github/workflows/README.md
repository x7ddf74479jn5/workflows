# Reusable Workflows

別のレポジトリから呼び出し可能なワークフローの置き場。

[ワークフローの再利用 \- GitHub Docs](https://docs.github.com/ja/actions/using-workflows/reusing-workflows)

## 使い方

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

## 一覧

- [delete_workflow_history.yml](./delete_workflow_history.yml): 指定したワークフローの履歴を削除する。
- [label.yaml](./label.yaml): 特定パスの変更に応じてラベル付けを行う。`labeler.yaml`の設定が必要。
