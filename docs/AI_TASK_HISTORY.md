# AI Task History

運用規約（保持ルール・書き方・アーカイブ手順）は [`docs/task-history.md`](task-history.md) を参照。
古い履歴は [`docs/history-archive/<YYYY>.md`](history-archive/) を参照。

---

## 2026-07-28 Codex 指摘の積み残しを修正

共有ドキュメントは consumer の複製を直接編集すると同期で上書きされるため、ops-sync 正本へ届く `shared-file` 提案にした。タスク消化は作業の完了条件と検証の成功をともに確認してから行い、片側だけの共通マーカーは初回配線とみなさず不正として扱う必要がある。

## 2026-07-27 Codex 指摘の積み残し対応


同期配布物の欠陥は consumer 側の複製を直しても再同期で戻るため、request ID の出力境界、競合再構築時の retention、揮発スライス境界の修正を ops-sync 正本へ届ける shared-file 提案にした。既存の履歴フラグメントは日付と汎用名だけでは並行ブランチ間で衝突するため、時刻とランダム ID を持つ一意なパスへ移した。公開リポジトリの review inbox 撤去前に読む側の fallback を更新する指摘は、後続同期で現在の共通ルールと設計文書に反映済みであることを確認した。
