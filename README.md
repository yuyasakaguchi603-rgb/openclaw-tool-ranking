# OpenClaw向けツール人気ランキング

更新日: 2026-04-24

OpenClawで使うと強い周辺ツールを、GitHub人気度と実用性で並べたランキングです。

## 評価基準

- GitHubスター数
- 更新頻度
- OpenClawとの相性
- 実作業での効果
- 導入しやすさ

## 総合ランキング

| 順位 | ツール | GitHub | スター | OpenClawでの用途 | コメント |
|---:|---|---|---:|---|---|
| 1 | Agent Skills | `anthropics/skills` | 123,257 | スキル資産 | OpenClawのスキル運用と相性がかなり良い。まず見るべき。 |
| 2 | Gemini CLI | `google-gemini/gemini-cli` | 102,296 | 追加コーディングエージェント | 端末型エージェントとして強い。調査や実装の別働隊に向く。 |
| 3 | MCP Servers | `modelcontextprotocol/servers` | 84,445 | 外部ツール接続 | MCP系の基礎カタログ。OpenClawの工具箱を広げる用途。 |
| 4 | Codex | `openai/codex` | 77,544 | コーディングエージェント | OpenClawから委任する開発タスク向け。大きめの修正に強い。 |
| 5 | Context7 | `upstash/context7` | 53,618 | 最新ドキュメント取得 | ライブラリ調査の精度が上がる。古い知識事故を減らせる。 |
| 6 | tmux | `tmux/tmux` | 44,841 | 対話CLI制御 | 長時間動くCLI、サーバー、対話ツールの監視に便利。 |
| 7 | GitHub CLI | `cli/cli` | 44,019 | GitHub操作 | Issue、PR、CI確認をOpenClawから安全に回せる。必須級。 |
| 8 | Playwright MCP | `microsoft/playwright-mcp` | 31,344 | ブラウザ操作 | Web画面確認、スクショ、フォーム操作に強い。実務効果が高い。 |
| 9 | Tailscale | `tailscale/tailscale` | 30,903 | 安全な遠隔接続 | 自宅MacやPiを安全に触る基盤。OpenClaw常駐運用向け。 |
| 10 | Vercel Agent Skills | `vercel-labs/agent-skills` | 25,638 | デプロイ・Web開発スキル | Vercel系やフロントエンド開発と相性が良い。 |
| 11 | skills CLI | `vercel-labs/skills` | 15,894 | スキル管理 | スキル配布・導入の参考になる。OpenClawスキル整理にも使える。 |
| 12 | Firebase Tools | `firebase/firebase-tools` | 4,397 | Firebase運用 | Firestore、Hosting、バックアップ確認に必須。今回の復旧でも重要。 |
| 13 | Browserbase MCP | `browserbase/mcp-server-browserbase` | 3,284 | クラウドブラウザ操作 | ローカルブラウザを使いたくない時の選択肢。業務自動化向け。 |

## 用途別おすすめ

### まず入れる

1. GitHub CLI
2. Context7
3. Playwright MCP
4. Firebase Tools
5. tmux

### 開発を強くする

1. Codex
2. Gemini CLI
3. Agent Skills
4. Vercel Agent Skills

### 自宅サーバー・常駐運用

1. Tailscale
2. tmux
3. GitHub CLI
4. Firebase Tools

## ポチの結論

OpenClawを実用で強くするなら、スター数だけでなく「作業事故を減らすツール」を優先した方がいいです。

優先度はこの順番。

1. GitHub CLI
2. Firebase Tools
3. Playwright MCP
4. Context7
5. tmux
6. Codex / Gemini CLI

派手さより、復旧・確認・自動化に効くものが本当に強いです。

## データ取得メモ

GitHubスター数は2026-04-24時点で確認しました。スター数は変動します。
