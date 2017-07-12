---
layout: post
title: "「奈倉柏木判定プログラム」完成のご報告"
date: 2017-07-12 20:00
categories: tensorflow
comments: true
share: true
---

[奈倉柏木判定プログラム](http://nakura-kashiwagi.hanarchy.biz)

ということで、上記webappが完成しましたのでそのご報告です。
django+gunicorn+nginxで構成してます。
コードは[こちら](https://github.com/hanarchy/NakuraKashiwagiHanteiProgram)です

前回から随分間が空いてしまいましたが、なんとか完成に漕ぎ着けることができました。(実働数時間、要はやる気が出なかった)

なお、その間に作っていたアニメ売上予測ツールは学習が上手くいかず、お蔵入りになりました。

中身は前回と変わらず180単語のBag-of-Wordsの後にMLPです。
前回学習させたcheckpointを読み込ませてあります。

tensorflow学習済みモデルを使ったwebアプリの構築手順については、いつかまとめようと思います。
大して難しくなかったけど。

次はSeqGANでも試してみようと思います。
