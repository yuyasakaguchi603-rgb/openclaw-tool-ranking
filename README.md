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

## 追加で見つけたすごいリポジトリ

OpenClaw本体に直接入れるというより、周辺強化・調査対象として強いもの。

| 分類 | リポジトリ | スター | 何がすごいか | OpenClaw目線 |
|---|---|---:|---|---|
| ワークフロー自動化 | `activepieces/activepieces` | 21,849 | AI Agents + MCP + 業務自動化。Zapier/Make系のOSS版に近い | 外部サービス連携を増やすなら強い |
| ブラウザ自動化 | `vercel-labs/agent-browser` | 30,453 | AIエージェント向けブラウザ操作CLI | Playwright MCPと競合/補完。要検証 |
| コーディングエージェント | `QwenLM/qwen-code` | 23,804 | Qwen系のターミナルAIエージェント | Codex/Gemini/Claudeの別働隊候補 |
| コーディングエージェント | `plandex-ai/plandex` | 15,287 | 大規模コードベース向けAI coding agent | 長期タスク分解に良さそう |
| コーディングエージェント | `opencode-ai/opencode` | 12,184 | ターミナル型AI coding agent | OpenClawのACP/委任候補 |
| 複数エージェント管理 | `smtg-ai/claude-squad` | 7,143 | Claude Code / Codex / OpenCode等を並列管理 | たくさん走らせるなら面白い |
| MCP開発基盤 | `mcp-use/mcp-use` | 9,804 | MCPアプリ/サーバー開発フレームワーク | 自作MCPを作るなら見る価値あり |
| DB接続MCP | `googleapis/mcp-toolbox` | 14,792 | データベース向けMCPサーバー | SQL/DB分析をOpenClawに持たせる候補 |
| Figma連携 | `GLips/Figma-Context-MCP` | 14,502 | Figmaのレイアウト情報をAIに渡すMCP | UI実装をFigmaから起こすなら強い |
| PC操作MCP | `wonderwhy-er/DesktopCommanderMCP` | 5,940 | ターミナル・ファイル検索・diff編集をMCP化 | OpenClawは既に同等機能あり。HERMES側には良いかも |
| OpenClaw素材集 | `mergisi/awesome-openclaw-agents` | 3,071 | OpenClaw向けSOUL.mdテンプレ集 | エージェント人格/役割設計の参考になる |
| AIアプリ集 | `Arindam200/awesome-ai-apps` | 10,229 | RAG/Agent/Workflowの実例集 | 作りたいもの探しに良い |
| LLMリソース集 | `WangRongsheng/awesome-LLM-resources` | 8,166 | LLM/Agent/MCP資料まとめ | 調査用ブックマーク |

## 追加候補の優先度

### すぐ試す価値あり

1. `vercel-labs/agent-browser`
2. `QwenLM/qwen-code`
3. `opencode-ai/opencode`
4. `googleapis/mcp-toolbox`
5. `GLips/Figma-Context-MCP`

### 研究・ブックマーク枠

1. `activepieces/activepieces`
2. `mcp-use/mcp-use`
3. `plandex-ai/plandex`
4. `smtg-ai/claude-squad`
5. `mergisi/awesome-openclaw-agents`

## 注意

セキュリティ系・ブラウザ自動化系・PC操作系MCPは強いぶん危ないです。OpenClawに入れるなら、権限と対象ディレクトリを絞るのが安全。
