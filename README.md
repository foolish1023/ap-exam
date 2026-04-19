# 応用情報技術者試験 (AP) Practice

応用情報技術者試験（AP）の合格を目指す学習アプリ。午前問題150問と教科書40トピックをブラウザで完結。オフライン動作対応（PWA）。

## 使い方

ブラウザで開くだけ。

**公開版:** https://foolish1023.github.io/ap-exam/

**ローカル実行:**

```bash
git clone https://github.com/foolish1023/ap-exam.git
cd ap-exam
python3 -m http.server 8767
```

その後 `http://localhost:8767/` を開く。

## 機能

- **午前問題 150問** — 6章構成（基礎理論・アルゴリズム / コンピュータシステム / データベース・ネットワーク / セキュリティ・システム構成 / 開発・プロジェクトマネジメント / システム戦略・経営戦略・法務）
- **教科書 40トピック** — 章ごとに重要テーマを解説。FEより1段深い計算・判断・比較を問う内容
- **PWA** — スマホにインストール可能。完全オフライン動作
- **ダークモード** — 自動切替 + 手動トグル
- **進捗保存** — 正誤・復習フラグを localStorage に永続化
- **アクセシビリティ** — WCAG AA準拠、キーボードナビゲーション対応

## 関連アプリ

- [基本情報技術者試験 (FE)](https://github.com/foolish1023/fe-exam) — 同じフレームで構築したFE版
- [Java Silver (SE 11)](https://github.com/foolish1023/java-silver) — Java Silver練習アプリ

## 構成

| ファイル | 役割 |
|---|---|
| `index.html` | SPA本体。UIと状態管理 |
| `questions.js` | 午前問題150問 |
| `lessons.js` | 教科書40トピック |
| `sw.js` | Service Worker（オフライン対応） |
| `manifest.webmanifest` | PWAマニフェスト |

## ライセンス

私的学習用。問題は学習目的で自作。
