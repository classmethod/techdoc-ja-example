# 情報技術ドキュメント例

[techdoc-ja](https://github.com/classmethod/techdoc-ja) は、
日本語で情報技術ドキュメント（仕様書やドキュメント等）を記述するためのオーサリング環境を提供します。

本ドキュメントは、その利用実例です。

## 要件

- ドキュメントを Markdown 形式で記述する。
    - コードブロックのシンタックスハイライトに対応する。
    - PlantUML による作図に対応する。
    - 日本語の記述に対応する。PlantUML 画像内でも日本語が表記できる。
- GitHub でドキュメントプロジェクトを管理し、PR で編集する。
- Circle CI によって継続的に、次の処理を実行する。
    - RedPen および textlint により文章の自動校正をする。
    - Gitbook によって、HTML および PDF 出力を得る。
    - 出力結果は Amazon S3 にデプロイする。
