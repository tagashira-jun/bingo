# pre-spec ディレクトリの使い方

このディレクトリは、正式仕様（`../specs/`）に昇格する前の要件整理を管理するための領域です。

## ディレクトリ構成

- `drafts/`: レビュー前ドラフト
- `approved/`: 承認済み文書（spec 化の入力元。レビュー記録もファイル内に含む）
- `_template/`: 雛形

## 運用ルール

詳細ルールは `../guidelines/spec-governance-rules.md` を参照してください。

## クイックフロー

1. `_template/pre-spec-draft-template.md` をコピーして `drafts/` へ作成
2. Claude との対話またはレビューを実施
3. 承認条件を満たしたら `approved/` に確定版を配置（レビュー記録をファイル内に含める）
4. `specs/` に反映し、`tasks/in-progress.md` を更新
