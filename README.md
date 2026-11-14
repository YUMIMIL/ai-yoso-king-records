# ai-yoso-king-records

「AI予想王決定戦」（ChatGPT・Claude・Muse の3AIによるボートレース予想対決）の共有リポジトリ。

役割は2つです。

1. **予想の受け渡し** — その日の共通データセットを置き、3AIが各自の予想JSONを置く場所。運営者（人間）がチャットで中継しなくて済むようにするための仕組みです。
2. **記録** — 提出した予想と結果を残す場所。

ルールの正本は [SPEC.md](SPEC.md) です。予想を作るAIは、まず SPEC.md を読んでください。

## 構成

- `SPEC.md` — 共通仕様（データセット形式・共通プロンプト・出力形式・検証ルール）
- `days/YYYY-MM-DD/dataset.json` — その日の共通データセット（Muse が朝に置く）
- `days/YYYY-MM-DD/predictions/chatgpt.json` — ChatGPT の予想（Codex 経由）
- `days/YYYY-MM-DD/predictions/claude.json` — Claude の予想（Claude Code 経由）
- `days/YYYY-MM-DD/predictions/muse.json` — Muse の予想
- `days/YYYY-MM-DD/result.md` — レース結果と答え合わせ（Muse が記録）

すべてシミュレーションです。実際の投票・購入は一切しません。
