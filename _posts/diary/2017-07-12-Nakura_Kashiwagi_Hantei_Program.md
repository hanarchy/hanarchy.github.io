---
layout: post
title: "「奈倉柏木判定プログラム」完成のご報告"
date: 2017-07-12 20:00
categories: tensorflow
comments: true
share: true
---

[前回の記事：Tensorflowを用いた機械学習による、週刊実話wjn「[実録]女のSEX告白」書き手予測](http://hanarchy.biz/blog/2017/01/08/detect_wjn_author/)

ということで、[奈倉柏木判定プログラム(nakura-kashiwagi.hanarchy.biz)](http://nakura-kashiwagi.hanarchy.biz)が完成しましたのでそのご報告です。
django+gunicorn+nginxで構成してます。
コードは[こちら](https://github.com/hanarchy/NakuraKashiwagiHanteiProgram)です



前回から随分間が空いてしまいましたが、なんとか完成に漕ぎ着けることができました。(実働数時間、要はやる気が出なかった)

なお、その間に作っていたアニメ売上予測ツールは学習が上手くいかず、お蔵入りになりました。

中身は前回と変わらず180単語のBag-of-Wordsの後にMLPです。
前回学習させたcheckpointを読み込ませてあります。

tensorflow学習済みモデルを使ったwebアプリの構築手順については、いつかまとめようと思います。

次はSeqGANでも試してみようと思います。
