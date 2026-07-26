# Codex レビューの未対応在庫（`ops-runner`）

ops-sync の `codex-review-inbox` workflow が生成する。**手で編集しない**（次回実行で上書きされる）。
生成元: `ops-sync/scripts/codex-review-inbox.mjs`。

**この一覧は GitHub の resolve 状態そのもの**なので、別途の管理表は無い:

1. 指摘を直す（配布 doc・共有ファイルの指摘は **ops-sync の正本で直す**。consumer 同期 PR は手編集しない）
2. GitHub でそのレビュースレッドを **resolve** する
3. 次回実行でこの一覧から消える

対応しない判断をした場合も、理由を返信してから resolve する（放置＝この一覧に残り続ける）。

## 未対応 9 件

| | 優先 | PR | ファイル | 指摘 | 経過 |
|---|---|---|---|---|---|
| 🔴 | P1 | [#1](https://github.com/65edh5ih/ops-runner/pull/1#discussion_r3651950000) | `.github/workflows/branch-cleanup.yml` | Abort cleanup when open-PR enumeration fails | 0日 |
| 🔴 | P1 | [#1](https://github.com/65edh5ih/ops-runner/pull/1#discussion_r3651950009) | `AGENTS.md` | Add the required docs structure index | 0日 |
| 🔴 | P1 | [#3](https://github.com/65edh5ih/ops-runner/pull/3#discussion_r3651987397) | `docs/cross-repo-tasks.md` | Add verifiable completion steps to the revised SOP | 0日 |
| 🔴 | P1 | [#11](https://github.com/65edh5ih/ops-runner/pull/11#discussion_r3652487825) | `.github/actions/net-fetch/net-fetch.sh` | Use the redacted request ID in the workflow summary | 0日 |
| 🔴 | P2 | [#1](https://github.com/65edh5ih/ops-runner/pull/1#discussion_r3651950004) | `.github/actions/publish-ci-logs/action.yml` | Rebuild the CI-log update after a rebase conflict | 0日 |
| 🔴 | P2 | [#1](https://github.com/65edh5ih/ops-runner/pull/1#discussion_r3651950007) | `.github/actions/publish-ephemeral/action.yml` | Remove slices whose publication marker is missing | 0日 |
| 🔴 | P2 | [#2](https://github.com/65edh5ih/ops-runner/pull/2#discussion_r3651962436) | `docs/net-fetch.md` | Update all aggregate-mode references together | 0日 |
| 🔴 | P2 | [#3](https://github.com/65edh5ih/ops-runner/pull/3#discussion_r3651987398) | `.github/workflows/branch-cleanup.yml` | Retain the legacy ai-ops cleanup prefix | 0日 |
| 🔴 | P2 | [#10](https://github.com/65edh5ih/ops-runner/pull/10#discussion_r3652458598) | `docs/cross-repo-tasks.md` | Make the outbox completion condition attainable | 0日 |

🔴 = マージ済み PR の未 resolve（配布物なら全 consumer に欠陥が残っている状態＝最優先）／🟡 = open PR。

---

これは `65edh5ih/ops-runner` の分だけを抜き出したもの。全リポジトリ分の一覧は別にある。

走査対象: `65edh5ih/nikki-san` / `65edh5ih/ops-runner` / `65edh5ih/ops-sync` / `65edh5ih/private`。直近 3 日に更新された PR に加え、**前回この一覧に載っていた PR は窓の外でも名指しで再確認する**（＝古くなったからではなく、resolve されたから消える）。

<!-- generated:2026-07-26T14:42:32Z -->
