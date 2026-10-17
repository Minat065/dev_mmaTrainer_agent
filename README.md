# dev_mmaTrainer_agent

MMA トレーナー向けの判断支援スキル群を Claude Code 上で動かすためのリポジトリ。

- 要求: `REQUIREMENTS.md`
- 設計上の確定事項: `docs/DECISIONS.md`
- スキル雛形: `.claude/skills/_template/SKILL.md`
- 実装済みスキル: `.claude/skills/`（`_template` 以外）

使い方: このリポジトリを Claude Code で開くと `.claude/skills/` 配下のスキルが自動で読み込まれる。`/skill-name` で明示的に呼ぶか、依頼内容に応じて Claude が自動で選ぶ。
