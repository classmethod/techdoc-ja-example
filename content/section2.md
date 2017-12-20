# Section 2 - 標準プロジェクト構成

ドキュメントプロジェクトは、次のディレクトリ構成を標準とします。

```
.
+-- README.md            -- ドキュメントの運用・ビルド方法等
+-- .circleci
|   +-- config.yml       -- Circle CI 設定
|
+-- .gitignore           -- git 設定
+-- book.json            -- Gitbook 設定
+-- config               -- 校正ツール設定
|   +-- redpen-conf.xml  -- RedPen 設定
|   +-- redpen-dict
|       +-- stopwords.txt
|       +-- suggest.txt
|       +-- katakana.txt
|   +-- textlint.json    -- textlint 設定
|   +-- ...
|
+-- content
|   +-- README.md        -- ドキュメント本体の README
|   +-- SUMMARY.md       -- 目次等
|   +-- ...              -- その他コンテンツ
|   +-- styles
|       +-- website.css
|       +-- pdf.css
|
+-- _book                -- ビルド成果物
    +-- index.html
    +-- techdoc-example.pdf
    +-- ...
```


## Circle CI と同等の環境下に入る方法

```
$ docker run --rm -it -v $(pwd):/root/workspace -w /root/workspace classmethod/techdoc-ja:latest sh
```
