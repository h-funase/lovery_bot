# lovery_bot
Pythonの機械学習用ライブラリを利用して、アップロードされた画像に写っているのが犬と猫どちらかを判定ができるアプリケーションを作成しました。
フレームワークはDjangoを利用しています。
アップロードされる画像は一切データベースに保存されません。
またCertificate ManagerとALBを利用し、常時SSL通信化を行っています。

# リンク
https://lovery-bot.com/

# 説明
まずFlickrAPIを使って、５００枚ほどの画像をweb上から収集をしました。その画像をKeras(Google社の機械学習用Pythonライブラリ『TensorFlow』に内蔵された簡易な機械学習ライブラリ)を利用し機械学習を行わせました。
またVGG16という様々な大量の画像を予め学習しているニューラルネットワークモデルを機械学習の過程で利用し、精度の向上に成功しました。
# 画像
![demo](https://user-images.githubusercontent.com/58463973/75023138-a8cf8f00-54da-11ea-804b-e66f839dbf0e.gif)
# 使用技術

## 言語
Python,HTML,CSS

## webアプリケーションフレームワーク
Django

##  Python用ライブラリ
TensorFlow,Keras,numpy,Pillow

## サーバ関連
AWS(EC2,Route53,ALB,Certificate Manager)

# 補足
また、LOVERY DRAWというリンクをクリックすると、もう一つの二枚の画像を合成するアプリケーションに跳べるようになっています(https://github.com/h-funase/h-funase.github.io)
