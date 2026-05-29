# Claude Agent Skills 総合ガイド

ClaudeのAgent Skills（スキル）を概要・仕組み・作り方・活用法・CLAUDE.md/MCPとの違い・利点欠点・便利なスキル例まで体系的にまとめた**単一HTMLの日本語リファレンス**です。

- 本体: [`index.html`](./index.html)（外部依存なし。そのまま静的ホスティング可能）
- 内容の根拠: 2026年5月時点の公式ドキュメント（platform.claude.com / code.claude.com / anthropic.com / anthropics/skills）の要約

## ローカルで開く

`index.html` をブラウザで開くだけ。ビルド不要です。

## GitHub + Vercel で公開する

```bash
# 1) GitHub へ
git init && git add . && git commit -m "Add Claude Skills guide"
git branch -M main
git remote add origin git@github.com:<you>/claude-skills-guide.git
git push -u origin main

# 2) Vercel CLI で（またはダッシュボードからImport）
npm i -g vercel
vercel          # プレビュー
vercel --prod   # 本番
```

Vercel側の設定: Framework = **Other**、Build/Output Command は空のままでOK（ルートの `index.html` がそのまま配信されます）。社内限定にしたい場合は Vercel の Password Protection / Vercel Authentication を利用してください。

> 仕様（ベータヘッダ名・エンドポイント・制限値など）は変更され得ます。実装時は公式ドキュメントで最新を確認してください。
