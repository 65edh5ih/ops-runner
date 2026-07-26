## 2026-07-26 公開 Codex review inbox スライスの撤去

ops-runner の `main` も pull request 必須の運用へ移り、定期処理による public repo への直接 push を避ける必要がある。
Codex review の走査対象には ops-runner を残す一方、結果は private リポジトリ側の全体一覧へ集約し、ops-runner 固有の公開スライスは維持しない。
