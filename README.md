# dev_mmaTrainer_agent

プロ MMA 選手向けの情報収集スキル群を Claude Code 上で動かすリポジトリ。

| 置き場所 | 内容 |
|---|---|
| `REQUIREMENTS.md` | 要求ドキュメント |
| `docs/DECISIONS.md` | 設計上の確定事項 |
| `docs/SKILL_TEMPLATE.md` | スキル雛形 |
| `profile.md` | 選手コンテキスト（全スキルが読む） |
| `.claude/skills/<skill-name>/SKILL.md` | スキル本体 |
| `inputs/<skill-name>/` | 有料ソース・映像から人手で起こしたメモ |
| `outputs/<skill-name>/` | スキルの実行結果 |

## 使い方
1. `profile.md` を埋める。
2. このリポジトリを Claude Code で開く。`.claude/skills/` 配下のスキルが自動で有効になる。
3. `/weight-cut`、`/opponent-scouting [相手名]` のように呼ぶか、依頼内容に応じて Claude が選ぶ。
4. 結果は `outputs/` に保存される。commit して履歴を残す。

## 実装状況
| 優先 | スキル | 状態 |
|---|---|---|
| 1 | `weight-cut` | 実装済み |
| 2 | `opponent-scouting` | 実装済み |
| 3 | `matchmaking` / `fighter-tracker` | 実装済み |
| 4 | `contracts-pay` | 実装済み |
| 5 | その他 21 本 | 未着手 |
