# AI Task History

運用規約（保持ルール・書き方・アーカイブ手順）は [`docs/task-history.md`](task-history.md) を参照。
古い履歴は [`docs/history-archive/<YYYY>.md`](history-archive/) を参照。

---

## 2026-07-27 Codex 指摘の積み残し対応


同期配布物の欠陥は consumer 側の複製を直しても再同期で戻るため、request ID の出力境界、競合再構築時の retention、揮発スライス境界の修正を ops-sync 正本へ届ける shared-file 提案にした。既存の履歴フラグメントは日付と汎用名だけでは並行ブランチ間で衝突するため、時刻とランダム ID を持つ一意なパスへ移した。公開リポジトリの review inbox 撤去前に読む側の fallback を更新する指摘は、後続同期で現在の共通ルールと設計文書に反映済みであることを確認した。

## 2026-07-26 公開 Codex review inbox スライスの撤去

ops-runner の `main` も pull request 必須の運用へ移り、定期処理による public repo への直接 push を避ける必要がある。
Codex review の走査対象には ops-runner を残す一方、結果は private リポジトリ側の全体一覧へ集約し、ops-runner 固有の公開スライスは維持しない。

## 2026-07-26 Codex 指摘の積み残し

レビュー対象は ops-sync から同期される共通ファイルが中心であり、consumer の複製を直接直すと次回同期で失われるため、正本へ反映する shared-file 提案として修正を起票した。レビュー時点より後の同期ですでに解消済みの指摘も、現在の配布内容を根拠に区別した。
