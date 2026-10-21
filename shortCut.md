# CLion ショートカットメモ（Ubuntu）

※デフォルトのキーマップを想定。

## 1. 編集

| ショートカット | 機能 |
|---|---|
| `Alt + J` | 同じ文字列を順番に複数選択 |
| `Ctrl + R` | 置換・一括削除 |
| `Ctrl + Z` | 元に戻す |
| `Ctrl + Shift + Z` | やり直す |
| `Ctrl + /` | コメントアウト・解除 |
| `Ctrl + Alt + L` | コード整形 |

### 一括編集
- **複数選択**：文字列を選択 → `Alt + J` を繰り返す → 一括編集
- **一括置換**：`Ctrl + R` → 置換元・置換先を入力 → `Replace All`（`Alt + A`）
    - 置換先を空欄にすれば一括削除

## 2. 実行・デバッグ

| ショートカット | 機能 |
|---|---|
| `Shift + F10` | 実行（Run） |
| `Shift + F9` | デバッグ実行（Debug） |
| `F8` | 1行進める（Step Over） |
| `F7` | 関数内部に入る（Step Into） |
| `F9` | 次のブレークポイントまで続行 |
| `Ctrl + F2` | 実行停止 |
| `Alt + F12` | ターミナルを開く・閉じる |

### 実行方法
- **通常実行**：`Shift + F10`
- **デバッグ**：ブレークポイントを設置 → `Shift + F9`
- **ファイル入力**：`Run → Edit Configurations → Redirect input from` で `input.txt` を指定

### ターミナルから実行

```bash
g++ -std=gnu++17 -O2 main.cpp -o main && ./main < input.txt
```

## 3. Git・GitHub

| ショートカット | 機能 |
|---|---|
| `Ctrl + K` | Commit |
| `Ctrl + Shift + K` | Push |

### 通常の手順
1. `Ctrl + K` → メッセージ入力 → `Commit`
2. `Ctrl + Shift + K` → `Push`

### CommitとPushを一括実行
`Ctrl + K` → Commitボタン右側の `∨` → `Commit and Push...`