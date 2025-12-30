# Dotfiles

個人的な開発環境設定ファイルの管理リポジトリです。

## 含まれる設定

| ファイル/ディレクトリ | 説明 | リンク先 | 詳細 |
|-------------------|------|----------|------|
| `.zshrc` | Zsh設定 | `~/.zshrc` | - |
| `.gitconfig` | Git設定（delta含む） | `~/.gitconfig` | - |
| `.tmux.conf` | Tmux設定 | `~/.tmux.conf` | - |
| `starship.toml` | Starshipプロンプト設定 | `~/.config/starship.toml` | - |
| `nvim/` | Neovim設定 | `~/.config/nvim` | [README](nvim/README.md) |
| `wezterm/` | WezTerm設定 | `~/.config/wezterm` | [README](wezterm/README.md) |
| `yazi/` | Yaziファイルマネージャー設定 | `~/.config/yazi` | [README](yazi/README.md) |
| `sheldon/` | Sheldonプラグイン設定 | `~/.config/sheldon` | [README](sheldon/README.md) |
| `lazygit/` | Lazygit設定 | `~/.config/lazygit` | [README](lazygit/README.md) |
| `aerospace/` | Aerospaceウィンドウマネージャー設定 | `~/.config/aerospace` | [README](aerospace/README.md) |
| `borders/` | Bordersウィンドウボーダー設定 | `~/.config/borders` | [README](borders/README.md) |
| `sketchybar/` | Sketchybarステータスバー設定 | `~/.config/sketchybar` | [README](sketchybar/README.md) |
| `commitlint.config.js` | コミットメッセージ検証設定 | `~/commitlint.config.js` | - |
| `Brewfile` | Homebrewパッケージ管理 | - | - |

## 必要要件

以下のツールがインストールされていることを推奨します：

- **Git** - リポジトリのクローン
- **Zsh** - シェル
- **Homebrew** - パッケージマネージャー

## インストール

### 1. リポジトリのクローン

```bash
cd ~
git clone git@github.com:TetraTechAi/dotfiles.git
```

### 2. セットアップ実行

```bash
cd ~/dotfiles
./setup.sh
```

これにより以下が実行されます：
1. Brewfileからパッケージをインストール
2. シンボリックリンクを作成
3. sketchybarをセットアップ

### オプション

```bash
# Dry-run（事前確認）
./setup.sh -d

# Brewパッケージのみ
./setup.sh -b

# シンボリックリンクのみ
./setup.sh -l
```

### 3. 設定の反映

```bash
source ~/.zshrc
```

## 別のマシンへの展開

```bash
git clone git@github.com:TetraTechAi/dotfiles.git ~/dotfiles
cd ~/dotfiles
./setup.sh
source ~/.zshrc
```

## 設定の更新

```bash
cd ~/dotfiles
git add .
git commit -m "Update configuration"
git push origin develop
```
