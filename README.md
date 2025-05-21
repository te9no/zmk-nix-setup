# ZMK-Nix Setup

このリポジトリは、[ZMK firmware](https://zmk.dev/) のビルド環境を [Nix](https://nixos.org/) で簡単にセットアップするためのスクリプトを提供します。

## 使い方

1. **`build.yaml` を用意**
   - キーボードの設定ファイル `build.yaml` をカレントディレクトリに配置してください。

2. **セットアップスクリプトをダウンロードして実行**
   ```sh
   curl -O https://raw.githubusercontent.com/te9no/zmk-nix-setup/main/zmk-nix-setup.sh
   bash zmk-nix-setup.sh
   ```
   - `--dry-run` オプションでビルドをスキップできます。
   - `--help` でヘルプを表示します。

3. **ビルド成果物**
   - ビルドが成功すると、`./result/` ディレクトリにファームウェアが生成されます。

## 必要要件

- bash
- git
- Nix（未インストールの場合は自動でインストールされます）

## よくある手順

1. `config/` ディレクトリでキーマップ等を編集
2. 変更をコミット・プッシュ
3. `nix build` で再ビルド

## ライセンス

MIT License
