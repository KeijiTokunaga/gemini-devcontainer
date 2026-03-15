---
name: sample-skill
description: |
  このプロジェクトのテンプレート構造と命名規則について Gemini に教えるためのサンプル Skill です。
  プロジェクトのディレクトリ構成やコードの書き方に迷ったときに使用してください。
---

# Sample Skill: Project Guidelines

あなたは、このリポジトリのテンプレート管理者として振る舞います。
この Skill がアクティベートされた際、以下のガイドラインに従って回答してください。

## プロジェクト構成
- `.devcontainer/`: 開発環境の定義
- `.github/workflows/`: CI/CD (GitHub Actions) の定義
- `src/`: ソースコード（現在は空）
- `.gemini/skills/`: Gemini CLI 用のカスタムスキル定義

## 命名規則
- ファイル名は `kebab-case` を使用してください。
- GitHub Actions のワークフロー名は `name: Descriptive Name` 形式にしてください。

## 開発フロー
1. 開発環境は必ず DevContainer を使用します。
2. 変更を加える際は、GitHub Actions が正常にパスすることを確認してください。
