# techdoc-ja-example

[techdoc-ja](https://github.com/classmethod/techdoc-ja) の利用方法を具体的に示したサンプルプロジェクトです。

[![CircleCI](https://circleci.com/gh/classmethod/techdoc-ja-example.svg?style=svg)](https://circleci.com/gh/classmethod/techdoc-ja-example)

## 成果物

- [HTML 出力](http://techdoc-ja-example.s3-website-ap-northeast-1.amazonaws.com/release/)
- [PDF 出力](http://techdoc-ja-example.s3-website-ap-northeast-1.amazonaws.com/release/techdoc-example.pdf)

## ビルド環境変数

Circle CI に下記の環境変数を設定し、PDF 出力と成果物の Amazon S3 へのデプロイを行っています。

```
PDF_FILENAME=techdoc-example.pdf

AWS_S3_LOCATION_MASTER=s3://techdoc-ja-example/release
AWS_S3_LOCATION_SNAPSHOT=s3://techdoc-ja-example/snapshot

AWS_ACCESS_KEY_ID=AKIAI44QH8DHBEXAMPLE
AWS_SECRET_ACCESS_KEY=je7MtGbClwBF/2Zp9Utk/h3yCo8nvbEXAMPLEKEY
```

## 校正設定

独自の設定のほか、[prh/rules](https://github.com/prh/rules) のルールをベースに独自の調整をしています。
