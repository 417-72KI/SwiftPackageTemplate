# 基本
応答は日本語と英語を併記してください。
ただし、1文単位ではなく1応答単位で日本語と英語を併記してください。
例:　OK
```
日本語の文章1。
日本語の文章2。

English sentence1.
English sentence2.
```

例: NG
```
日本語の文章1。/ English sentence1.
日本語の文章2。/ English sentence2.
```

# Instructions
## .github/matrix.jsonについて
workflowsのmatrixに関する設定ファイルです。
`.github/workflows/test.yml`のmatrixに読み込まれます。

- `versions`: `test-macos`で使用する情報のリスト
  - `macos_runner`: 使うランナーのバージョン
  - `xcode`: そのランナーで使用するXcodeのバージョン
  - `destination`: テストに使用するシミュレーターの情報
- `swift_version`: `test-linux`で使用するSwiftのバージョン

`versions`について、各バージョンの詳細は
https://github.com/actions/runner-images/blob/main/images/macos/macos-{version}-Readme.md
を参照してください。
