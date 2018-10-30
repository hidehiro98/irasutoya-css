# いらすとやCSSライブラリ / CSS Library for Irastora

<img src="http://imgur.com/SZ8Cm.jpg">

[日本語](#日本語) / [English](#English)

## 日本語
### 概要
[いらすとや](https://www.irasutoya.com/)の画像をクラス追加だけで使えるようにするCSSライブラリです。
CSSのcontent:url("image.jpg")を使っているので、対応していないブラウザでは動かないかもしれません（[参考](https://stackoverflow.com/questions/2182716/is-it-possible-to-set-the-equivalent-of-a-src-attribute-of-an-img-tag-in-css)）。

### 使い方
1. CSSをリンクする<br/>
`<link rel="stylesheet" href="https://thiscss">`
2. imgタグにクラスを追加する（[画像](https://www.irasutoya.com/2018/10/blog-post_699.html)）<br/>
`<img class="irasutoya-2018-10-699">`
`<img class="irasutoya-pet-dog-thirsty">`

### クールな使い方募集中！

## English
### About this library
This is the library for using [Irasutora](https://www.irasutoya.com/) images only with CSS.
For non commercial use, these illustration are free ([Terms of use](https://translate.google.com/translate?sl=auto&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=https%3A%2F%2Fwww.irasutoya.com%2Fp%2Fterms.html&edit-text=)).
This library uses content:url("image.jpg"), so it may not work with unsupported browsers. ([reference](https://stackoverflow.com/questions/2182716/is-it-possible-to-set-the-equivalent-of-a-src-attribute-of-an-img-tag-in-css))

### How to use
1. Link this CSS<br/>
`<link rel="stylesheet" href="https://thiscss">`
2. Add the class to `img` tag. ([this image link](https://www.irasutoya.com/2018/10/blog-post_699.html))<br/>
`<img class="irasutoya-2018-10-699">`
`<img class="irasutoya-pet-dog-thirsty">`

## メモ
### スクレイピングの方針
時系列のURL（ https://www.irasutoya.com/search?updated-max=2012-01-01T20:15:00%2B09:00&max-results=24 みたいな）を使って、そこから次のページボタン（前の投稿）を辿って取って行く。
#### 次へリンクの構造

- updated-max: 2012-01-01T20:15:00%2B09:00 (2012-01-01T20:15:00 09:00)
- max-results: 24

最古のリンク
https://www.irasutoya.com/search?updated-max=2010-06-12T10:00:00%2B09:00&max-results=24&reverse-paginate=true&start=7&by-date=false

最古の絵？
https://www.irasutoya.com/2012/05/africa.html

このリンクより古いと大体複数
https://www.irasutoya.com/search?updated-max=2012-02-02T18:15:00%2B09:00&max-results=24&reverse-paginate=true

上記のみたいに複数の画像入っているリスト
https://www.irasutoya.com/2012/05/africa.html
https://www.irasutoya.com/2012/05/northamerica.html
https://www.irasutoya.com/2012/05/europe.html
https://www.irasutoya.com/2012/05/antarctica.html
https://www.irasutoya.com/2012/05/asia.html

