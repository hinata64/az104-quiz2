# Azure 資格試験 練習クイズ

Azure AD / RBAC / ストレージ / 仮想マシン / ネットワーク / 監視など、Azure試験範囲の問題を収録した練習クイズアプリです。

## 使い方

`azure_quiz.html` をブラウザで開くだけで使えます（サーバー不要）。

## 機能

- **202問**収録（テキストで抽出できたもの）
- 4つのモード：全問 / シャッフル / はい・いいえ2択 / 多択問題
- 正誤フィードバックと解説表示
- 問題追加フォーム（画像問題など手動追加可能）
- JSONエクスポート / インポート（追加した問題の保存）

## カバー範囲

| カテゴリ | 内容 |
|---------|------|
| Azure AD / Entra ID | 条件付きアクセス、MFA、ゲストユーザー、管理単位 |
| RBAC / ポリシー | ロール割り当て、Azure Policy、管理グループ |
| ストレージ | 冗長性、ライフサイクル管理、AzCopy、Import/Export |
| 仮想マシン | 可用性セット/ゾーン、拡張機能、スケールセット |
| ネットワーク | VNet、NSG、ロードバランサー、VPN、DNS、Firewall |
| 監視 / バックアップ | Azure Monitor、Log Analytics、Azure Backup |

## 問題の追加方法

### 手動追加
トップ画面下部の「問題を追加する」フォームから入力できます。

### JSONインポート
以下の形式のJSONファイルをインポートできます：

```json
[
  {
    "question": "問題文",
    "options": [
      {"label": "A", "text": "選択肢A"},
      {"label": "B", "text": "選択肢B"}
    ],
    "correct": "A",
    "explanation": "解説テキスト"
  }
]
```

## GitHub Pages での公開方法

1. このリポジトリをGitHubにプッシュ
2. Settings → Pages → Branch: main / (root) → Save
3. `https://ユーザー名.github.io/リポジトリ名/azure_quiz.html` でアクセス可能

