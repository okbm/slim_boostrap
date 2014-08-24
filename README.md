# phpのかるいフレームワーク

## メモ
- PHPのマイクロフレームワーク
- 気軽にRESTなAPI作れる
- 1ファイルのPHPでAPIが作れる
- 1ファイルだからこそ、ファイルが結構大きくなるとゴチャゴチャして読みにくい
- フォルダの配置しようにもフォルダ配置ルールがないので各自よろしく作ってるみたい
- なのでオレオレルールで作ってみた

## フォルダ構成

```
.
├── README.md
├── composer.json
├── config      # DBの設定とか
│   ├── config.php.sample
│   └── db      # sqlファイルを置く
├── lib         # ライブラリ的なもの
│   ├── bootstrap.php
│   └── helper.php
├── public      # webディレクトリ
│   ├── css
│   ├── img
│   ├── index.php  # 基本いじるファイル(MVCのコントローラーとモデルをガシガシ書いてく感じ)
│   └── js
├── templates   # viewファイルを置くとこ(header.phpとfooter.phpは共通化)
│   ├── footer.php
│   ├── header.php
│   ├── index.php
└── vendor      # slimのコアファイルなのでいじらない
```

## slimのセットアップ

```
# composerはPATHを通しておく
$ composer install
```

### 参考リンク
- [h5bp/html5-boilerplate](https://github.com/h5bp/html5-boilerplate)
- [Slim Framework Documentation](http://docs.slimframework.com/)
- [Slim マイクロフレームワークで REST アプリケーションを作成する](http://www.ibm.com/developerworks/jp/xml/library/x-slim-rest/)
