# 開発環境サマリー（コピペ用）

## 基本情報
- **ツール**: Claude Code（Anthropic CLI）
- **OS**: macOS
- **ディレクトリ**: `/Users/daikitakayama/code`

## 接続MCP（8種類）
1. **serena** - セマンティックコード解析・編集（最優先）
2. **memory** - ナレッジグラフによる知識管理
3. **filesystem** - ファイルシステム操作
4. **playwright** - ブラウザ自動化
5. **supabase** - Supabase管理
6. **sequential-thinking** - 段階的思考
7. **ide** - IDE統合
8. **codex** - AI駆動コード分析（自動起動）⭐️

## Codex自動起動条件
- バグ修正3回以上失敗
- アーキテクチャ設計相談
- 30分以上のデバッグ
- 複雑な技術判断

## セキュリティ
- ✅ 許可: ファイル操作、パッケージインストール、MCP操作、Web検索
- ❌ 禁止: sudo、rm、外部ネットワーク、DB直接操作、機密ファイル
- ⚠️ 要確認: Git操作、package.json変更

## 開発フロー
- **通常実装**: serena解析 → 編集 → memory記録
- **バグ修正**: 3回失敗 → Codex自動起動 → 解決
- **設計**: Codex分析 → 提案 → 実装

## 特徴
MCPを自発的に選択し、複雑な問題でCodexを自動起動。知識はmemoryに永続化。
