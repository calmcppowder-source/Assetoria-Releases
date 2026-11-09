# Assetoria - VRC Asset Inventory

Assetoriaは、VRChat向けに購入・入手したアセットZIPを、BOOTHの商品情報やタグと関連付けてローカルで整理するWindows用ソフトです。

> 現在はテスター向けの試験公開版です。利用前に設定データのバックアップを作成してください。

## ダウンロード

[Assetoria v1.1.11 テスター版をダウンロード](https://github.com/calmcppowder-source/Assetoria-Releases/releases/tag/v1.1.11)

Releasesページから次のファイルをダウンロードしてください。

- `Assetoria_v1.1.11_win-x64.zip`：アプリ本体
- `Assetoria_v1.1.11_win-x64.zip.sha256.txt`：改ざん・破損確認用（任意）

GitHubが自動表示する「Source code (zip)」「Source code (tar.gz)」はアプリ本体ではありません。

## 動作環境

- 64bit版 Windows 10 / 11
- [.NET 10 Desktop Runtime（Windows x64）](https://dotnet.microsoft.com/download/dotnet/10.0)

.NET 10 SDKは不要です。未導入の場合は、利用者の確認後にMicrosoft公式の.NET 10 Desktop Runtimeを自動で取得し、ハッシュとMicrosoft署名を確認してからインストールします。Windowsの管理者確認が表示される場合があります。

## 起動方法

1. ダウンロードしたZIPを任意のフォルダへすべて展開します。
2. 最上位にある `Assetoriaを起動.bat` をダブルクリックします。
3. .NET 10 Desktop Runtimeが未導入の場合は、確認画面で「Yes」を選び、Windowsの管理者確認を許可します。インストール後はAssetoriaが自動で起動します。

`App` フォルダ内のファイルは動作に必要です。個別に移動・改名・削除しないでください。

## テストで確認してほしい項目

- 起動と終了、再起動後の設定保持
- アセットフォルダの登録と再スキャン
- BOOTH商品の照合、商品情報・ショップ名・タグの検索
- 独自タグとBOOTHタグの表示・保存
- 照合済み一覧の商品単位表示と表示切り替え
- 「今回追加」フィルター
- バックアップと復元
- 管理対象の元ZIPが移動・改名・展開・削除されていないこと

## データと安全性

- 設定と照合情報は `%LOCALAPPDATA%\Assetoria` に保存されます。
- 商品検索やタグ取得にBOOTHの公開情報へアクセスしますが、BOOTHアカウントのログイン情報は要求・保存しません。
- 購入済みZIPを外部へ送信しません。
- 元ZIPは読み取り専用で扱い、移動・改名・展開・削除しません。
- 本ソフトは未署名のため、Windows SmartScreen等の警告が表示される場合があります。確認のためにセキュリティソフトを無効化したり、広い範囲を除外登録したりしないでください。

## 不具合の報告

[GitHub Issues](https://github.com/calmcppowder-source/Assetoria-Releases/issues) へ、次の内容を添えて報告してください。

- Windowsのバージョン
- 発生までの手順
- 毎回発生するか
- エラー表示やスクリーンショット

購入したアセット本体、管理対象ZIP、`settings.json` は公開しないでください。ログを載せる場合も、ユーザー名やローカルのフォルダ名など個人情報を削除してください。

## 注意事項

- 本ソフトはVRChatおよびBOOTHの非公式ツールです。
- VRChat Inc.、ピクシブ株式会社、BOOTH運営、各アセット制作者・販売者とは関係ありません。
- BOOTH側の仕様変更により、検索や商品情報取得が一時的に利用できなくなる場合があります。

利用前に [利用規約](TERMS_OF_USE.txt) を確認してください。
