# ビンゴ Web アプリ

ブラウザで遊べるビンゴアプリ。**現在は仕様整理中**で、まだ動くものはありません。

## 進め方

```
Phase 0 準備 ✅ → Phase 1 仕様整理 ← いまここ → Phase 2 技術選定・雛形 → Phase 3 MVP 実装 → Phase 4 公開
```

仕様は「事前要件整理（pre-spec）→ 承認 → 正式仕様（spec）」の順に固めてから実装に入ります。

## フォルダ構成

```
.
├── CLAUDE.md               # AI（Claude Code）向けの作業ルール
├── .claude/commands/       # Claude Code のスラッシュコマンド（/spec-next）
├── .ai/
│   ├── pre-spec/           # 事前要件整理（drafts → approved）
│   ├── specs/              # 正式仕様（pre-spec から昇格）
│   ├── decisions/          # 設計判断の記録（ADR）
│   ├── context/            # 用語集・技術スタック・学びの記録
│   └── guidelines/         # 仕様の運用ルール
└── tasks/                  # 現在地（in-progress）とバックログ
```

## 仕様整理の始め方

Claude Code でこのフォルダを開き、次を実行します。

```
/spec-next
```

未決の論点を 1 つ選んで対話で決め、要件ドラフトに書き込みます。

## 主なドキュメント

- 現在地: [tasks/in-progress.md](tasks/in-progress.md)
- 要件ドラフト: [.ai/pre-spec/drafts/BIZ-BINGO-001_overview.md](.ai/pre-spec/drafts/BIZ-BINGO-001_overview.md)
- 用語集: [.ai/context/domain-glossary.md](.ai/context/domain-glossary.md)
