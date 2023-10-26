# キッズセーフ 〇〇市 〇〇地区 / KidsSafe

- 〇〇市〇〇地区の地域安全マップを作成して、スマホやパソコンで見られる形で共有するツールです
- ExcelやNumbersを使ってCSVデータを編集しアップロードすることで更新できます
- [キッズセーフ by Code for FUKUI](https://github.com/code4fukui/kidssafe/) を使って作られています

## ソースコード

- [index.html](index.html) - アプリ設定（都市名、地域名、ソースコード）を設定する
- [index.csv](index.csv) - 地図に表示するCSVデータを設定する

## 利用方法

1. リポジトリ [kidssafe-template](https://github.com/code4fukui/kidssafe-template/) で、「Use this template」「Create a new repository」する
2. [README.md](README.md)、[アプリ設定](index.html)、[データ](index.csv)を地区に合わせて変更する
3. GitHub Pages(SettingsのPages)を設定し公開する

## データの更新方法

1. 変更したいデータを確認する (例、[aed.csv](aed.csv))
2. ダウンロードボタンを押し、ダウンロードする

<img width="306" alt="image" src="https://github.com/code4fukui/kidssafe-template/assets/1715217/053db2b7-1931-4b7c-b369-326523190d64">

3. Excelで編集する
4. 位置情報は、「[緯度経度地図](https://fukuno.jig.jp/app/map/latlng/#%E8%B6%8A%E5%89%8D%E5%B8%82)」から該当場所に動かして、Geo3x3欄に表示された文字列を項目Geo3x3にコピーする

<img width="511" alt="image" src="https://user-images.githubusercontent.com/1715217/219602296-2d3b72ce-581a-4ba8-8c69-edbe1b95ee76.png">

5. Excelで保存する
6. [./](./) に編集したファイルをドロップし、アップロード(Upload)する

<img width="306" alt="image" src="https://github.com/code4fukui/kidssafe-template/assets/1715217/53bdf652-f38a-47dc-8b3e-defa62f989ce">

7. 1分ほど待つと更新される（しばらくはキャッシュが使われることがあるので、プライベートモードなどで開いて確認するといい）

## データ種の追加方法

1. [template.csv](template.csv)をダウンロードし、Excelで開く
2. 2行目以降に地図に設定したい情報を記述する（項目は自由に増やせます）
3. Excelの「ファイル」「名前を付けて保存」を選び「ファイル形式」を「CSV UTF-8(コンマ区切り)(.csv)」に変更して、データ種類がわかるような英数ファイル名で保存する
4. [index.csv](index.csv)をダウンロードし、Excelで開く
5. 3で保存したファイル名とデータ種類名、アイコンファイル名を記述する
6. [./](./) にindex.csvと3で保存したファイルをドロップし、アップロード(Upload)する
7. 1分ほど待つと更新される（しばらくはキャッシュが使われることがあるので、プライベートモードなどで開いて確認するといい）

## アイコン追加方法

1. 大きさ100x100程度の画像を用意し、PNG形式、半角英数名で保存する（JPEGだと背景が透けません）
2. [icon](icon)フォルダを表示し、エクスプローラーなどからドロップし、アップロード(Upload)する
3. [index.csv](index.csv)や各データをダウンロードし、Excelで開き、icon項目を該当ファイル名に変更する
4. 編集したファイルを [./](./) へアップロードする
5. 1分ほど待つと更新される（しばらくはキャッシュが使われることがあるので、プライベートモードなどで開いて確認するといい）
