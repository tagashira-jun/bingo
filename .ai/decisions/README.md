# Architecture Decision Records (ADR)

設計上の重要な判断を時系列で記録する。後から「なぜこう作ったか」を追えるようにするのが目的。

---

## 命名規則

```
ADR-{連番}_{kebab-case-title}.md
```

- 例: `ADR-001_card-handling.md`
- 連番はゼロパディング（3 桁）。順序は提案日時に従う。

## ステータス遷移

| Status | 意味 |
|--------|------|
| `Proposed` | 提案中。レビュー待ち |
| `Accepted` | 採用。実装の根拠として参照される |
| `Deprecated` | 廃止予定。後継 ADR が用意される予定 |
| `Superseded by ADR-NNN` | 後継 ADR で置き換えられた。履歴目的のみ残す |

**遷移ルール**:
- `Proposed → Accepted`: ユーザー承認をもって遷移
- `Accepted → Superseded`: 後継 ADR の `Accepted` と同時に旧 ADR を更新

---

## 起票が必要なケース

1. **アプリの構成を決めるとき**（静的サイトか、サーバ・DB を持つか）
2. **公開方法を決めるとき**（GitHub Pages / Vercel / Firebase Hosting など）
3. **依存ライブラリ・フレームワーク・外部サービスの導入**（`package.json` への追加、Firebase 等）
4. **データの保存方法を決める・変えるとき**（ブラウザ内保存、DB など）
5. **A/B/C 案からユーザーが C 案（スコープ縮小・別タスク化）以外を選んだとき**

---

## 索引（INDEX）

新しい ADR を起票したら、以下の表に追記する。

| ADR | タイトル | Status | Date |
|-----|---------|--------|------|
| ADR-001 | 参加者カードは紙にし、アプリは主催者の抽選画面だけにする | Accepted | 2026-10-23 |

---

## 関連ドキュメント

- テンプレート: `_template-adr.md`
- 三選択肢提示ルール: `CLAUDE.md` の DO セクション
