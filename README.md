# Mobile Term — Releases

**PC で動かしている Claude Code を、スマホのチャット UI から操作できる連動ターミナル。**

このリポジトリは Mobile Term の**配布専用**です（ソースコードは非公開）。
最新のバイナリは [Releases](https://github.com/kogasura/mobile-term-releases/releases) からダウンロードしてください。

- 利用条件: [EULA](EULA.md) / [プライバシーポリシー](PRIVACY.md)（テレメトリなし・通信は LAN 内のみ）
- バグ報告・要望: [Issues](https://github.com/kogasura/mobile-term-releases/issues)

## 前提条件

- PC に [Claude Code CLI](https://docs.claude.com/ja/docs/claude-code/setup) がインストール・ログイン済みであること
- PC とスマホが同一 Wi-Fi (LAN) に接続されていること

## インストール

### Windows (PC 側・必須)

`Mobile.Term_<version>_x64-setup.exe` をダウンロードして実行。

- Windows 10 (build 1809) 以降 / Windows 11
- 未署名のため SmartScreen 警告が出たら「詳細情報」→「実行」
- インストール後は自動アップデートが有効になります

### スマホ (iPhone / Android)

アプリのインストールは不要です。PC の設定画面の QR をカメラで読み、ブラウザで開いて
「ホーム画面に追加」してください。

## 使い方

1. PC の Mobile Term → 設定 (⚙) → 「スマホ連携」→ **有効にする**
2. 表示された QR コードをスマホアプリでスキャン（同一 Wi-Fi 内）
3. Claude セッション一覧 → チャット画面から指示

## 制約

- 通信は同一 LAN 内のみ（外出先からは [Tailscale](https://tailscale.com) 等の VPN を併用）
- スマホ通知はアプリがフォアグラウンド〜直近バックグラウンドの間のみ
