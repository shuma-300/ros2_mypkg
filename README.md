# ros2_ws/src/mypkg
[![test7](https://github.com/shuma-300/ros2_mypkg/actions/workflows/test.yml/badge.svg)](https://github.com/shuma-300/ros2_mypkg/actions/workflows/test.yml)
## 概要
* このmypkgというリポジトリはros2のパッケージでtalker、listenerコマンド（ノードが互いに通信するコマンド）が含まれる
* ロボットシステム学の練習用のリポジトリとして作成
* https://ryuichiueda.github.io/my_slides/robosys_2022/lesson8.html#/11 を参照し
* ros2のインストールがされてない方は先にインストールをお願いします
インストールが終わった方はリポジトリをワークスペースにクローンしてください
```
$ git clone https://github.com/shuma-300/ros2_mypkg.git
```
   を実行

## talkerコマンドとlistenerコマンド
* talker.pyからInt16型のメッセージを送信
* listener.pyからInt16型のメッセージを受信し表示

## 実行例
```
$ ros2 run mypkg talker
```
ここで別端末でros2を使ってサブスクライブをする
```
$ ros2 topic echo /countup
data: 16
---
data: 17
---
data: 18
（以下省略）
```

## 必要なソフトウェア
* ros2 humble

## 動作確認済み環境
* Ubuntu 22.04.1LTS

## 著作権とライセンス
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
* このパッケージのコードは，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．

https://github.com/ryuichiueda/my_slides/tree/master/robosys_2022

* © 2022 Shuma Ito
