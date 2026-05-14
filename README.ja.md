# kidssafe-template

地域の安全マップを作成・共有するためのテンプレートです。このプロジェクトでは、ExcelやNumbersなどのツールで編集できるシンプルなCSVファイルを使って、マップデータを管理できます。Code for FUKUIによる[KidsSafeプロジェクト](https://github.com/code4fukui/kidssafe/)をベースに構築されています。

## デモ

https://code4fukui.github.io/kidssafe-template/

## 機能

- GitHub Pagesを利用して、地域の安全マップを作成・共有できます。
- ExcelやNumbersで編集可能なシンプルなCSVファイルで、マップ上のポイントを管理できます。
- [index.csv](index.csv) を編集するだけで、新しいデータレイヤーやカスタムアイコンを簡単に追加できます。
- 位置情報のエンコードには[Geo3x3](https://github.com/jigjp/geo3x3)を使用しており、シンプルな[検索ツール](https://fukuno.jig.jp/app/map/latlng/#%E8%B6%8A%E5%89%8D%E5%B8%82)も利用可能です。

## 使い方

1.  **リポジトリの作成:** 「Use this template」ボタンをクリックして、新しいリポジトリを作成します。
2.  **GitHub Pagesの有効化:** 新しいリポジトリの「Settings」から「Pages」セクションに移動します。ソースとして `main` ブランチを選択して保存します。マップは `https://<your-username>.github.io/<your-repo-name>/` で公開されます。
3.  **マップのカスタマイズ:** `index.html` ファイルを編集し、プレースホルダーとなっている市名（`〇〇市`）や地区名（`〇〇地区`）を実際の名称に変更します。

## マップデータの更新

1.  リポジトリから編集したいデータファイルをダウンロードします（例: [aed.csv](aed.csv)）。
2.  ExcelやNumbersなどのスプレッドシートアプリケーションでファイルを開き、編集します。
3.  新しい場所を追加する場合は、[緯度経度地図](https://fukuno.jig.jp/app/map/latlng/#%E8%B6%8A%E5%89%8D%E5%B8%82)を使用して正確なGeo3x3コードを取得します。
4.  編集したCSVファイルをリポジトリのルートディレクトリにアップロードします。
5.  変更内容は約1分後に公開されているマップに反映されます。

## 新しいデータレイヤーの追加

マップに新しいカテゴリのポイント（例: 「公共トイレ」）を追加することができます。

1.  データ用の新しいCSVファイルを作成します（例: `restrooms.csv`）。
2.  対応するアイコン画像を追加します（例: `restroom_icon.png`）。
3.  [index.csv](index.csv) を編集し、新しいレイヤーを登録する行を追加します: `Public Restrooms,restrooms.csv,restroom_icon.png`。
4.  新しいCSVファイルとアイコン画像をリポジトリにアップロードします。

## ライセンス

MIT License
