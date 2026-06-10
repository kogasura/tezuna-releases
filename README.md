# Mobile Term — Releases

**PC で動かしている Claude Code を、スマホのチャット UI から操作できる連動ターミナル。**

このリポジトリは Mobile Term の**配布専用**です（ソースコードは非公開）。
最新のバイナリは [Releases](https://github.com/kogasura/mobile-term-releases/releases) からダウンロードしてください。

## インストール

### Windows (PC 側・必須)

`Mobile.Term_<version>_x64-setup.exe` をダウンロードして実行。

- Windows 10 (build 1809) 以降 / Windows 11
- 未署名のため SmartScreen 警告が出たら「詳細情報」→「実行」
- インストール後は自動アップデートが有効になります

### Android

`app-universal-release.apk` をスマホでダウンロードして開く。
初回は「提供元不明のアプリのインストール」をブラウザに対して許可してください。

### iOS

現在ストア配布はありません。

## 使い方

1. PC の Mobile Term → 設定 (⚙) → 「スマホ連携」→ **有効にする**
2. 表示された QR コードをスマホアプリでスキャン（同一 Wi-Fi 内）
3. Claude セッション一覧 → チャット画面から指示

## 制約

- 通信は同一 LAN 内のみ（外出先からは [Tailscale](https://tailscale.com) 等の VPN を併用）
- スマホ通知はアプリがフォアグラウンド〜直近バックグラウンドの間のみ
