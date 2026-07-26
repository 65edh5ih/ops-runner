# Codex レビューの未対応在庫（`ops-runner`）

ops-sync の `codex-review-inbox` workflow が生成する。**手で編集しない**（次回実行で上書きされる）。
生成元: `ops-sync/scripts/codex-review-inbox.mjs`。

**この一覧は GitHub の resolve 状態そのもの**なので、別途の管理表は無い:

1. 指摘を直す（配布 doc・共有ファイルの指摘は **ops-sync の正本で直す**。consumer 同期 PR は手編集しない）
2. GitHub でそのレビュースレッドを **resolve** する
3. 次回実行でこの一覧から消える

対応しない判断をした場合も、理由を返信してから resolve する（放置＝この一覧に残り続ける）。

## 未対応 4 件

| | 優先 | PR | ファイル | 指摘 | 経過 |
|---|---|---|---|---|---|
| 🔴 | P1 | [#13](https://github.com/65edh5ih/ops-runner/pull/13#discussion_r3653514720) | `.ops-sync/outbox/2026-07-26T150000-net-fetch-safe-request-id-script.md` | Sanitize multiline request IDs before exporting outputs | 0日 |
| 🔴 | P1 | [#13](https://github.com/65edh5ih/ops-runner/pull/13#discussion_r3653514721) | `docs/history-inbox/2026-07-26-codex-review-work.md` | Give the history fragment a branch-unique filename | 0日 |
| 🔴 | P2 | [#15](https://github.com/65edh5ih/ops-runner/pull/15#discussion_r3653520487) | `.github/actions/net-fetch/net-fetch.sh` | Delimit the request ID before writing GITHUB_OUTPUT | 0日 |
| 🔴 | P2 | [#15](https://github.com/65edh5ih/ops-runner/pull/15#discussion_r3653520490) | `.github/actions/publish-ci-logs/action.yml` | Reapply retention pruning after rebuilding the update | 0日 |

🔴 = マージ済み PR の未 resolve（配布物なら全 consumer に欠陥が残っている状態＝最優先）／🟡 = open PR。

---

これは `65edh5ih/ops-runner` の分だけを抜き出したもの。全リポジトリ分の一覧は別にある。

走査対象: `65edh5ih/nikki-san` / `65edh5ih/ops-runner` / `65edh5ih/ops-sync` / `65edh5ih/private`。直近 3 日に更新された PR に加え、**前回この一覧に載っていた PR は窓の外でも名指しで再確認する**（＝古くなったからではなく、resolve されたから消える）。

<!-- generated:2026-07-26T22:06:09Z -->
