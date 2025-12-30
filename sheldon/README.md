# Sheldon

Zsh用の高速なプラグインマネージャー。

## 使い方

```bash
# プラグインを読み込み（.zshrcに記載済み）
eval "$(sheldon source)"

# プラグインを追加
sheldon add <name> --github <user/repo>

# 設定ファイルを編集
sheldon edit

# プラグインを削除
sheldon remove <name>
```

## インストール済みプラグイン

| プラグイン | 説明 |
|-----------|------|
| `zsh-autosuggestions` | コマンド履歴から自動補完候補を表示 |
| `zsh-syntax-highlighting` | コマンドラインのシンタックスハイライト |
| `zsh-completions` | 追加の補完定義 |
| `zsh-abbr` | 略語展開（Fish風） |

## 設定ファイル

- `plugins.toml` - プラグイン定義

## 参考

- [Sheldon公式ドキュメント](https://github.com/rossmacarthur/sheldon)
