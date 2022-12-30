# ros2_ws/src/mypkg
## 概要
* このmypkgというリポジトリはros2のパッケージでtalker、listenerコマンド（ノードが互いに通信するコマンド）が含まれる
* ロボットシステム学の練習用のリポジトリとして作成

## インストール方法
* https://ryuichiueda.github.io/my_slides/robosys_2022/lesson8.html#/11 を参照し
```
$ git clone https://github.com/ryuichiueda/ros2_setup_scripts
$ cd ros2_setup_scripts
```
を実行

## talkerコマンド
## listenerコマンド
![test](https://github.com/shuma-300/robosys202x/actions/workflows/test.yml/badge.svg)
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
* python 3.7 ~ 3.10
  * テスト済み

## 動作確認済み環境
* Ubuntu 22.04.1LTS

## 著作権とライセンス
* このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．
* このパッケージのコードは，下記のスライド（CC-BY-SA 4.0 by Ryuichi Ueda）のものを，本人の許可を得て自身の著作としたものです．

https://github.com/ryuichiueda/my_slides/tree/master/robosys_2022

* © 2022 Shuma Ito
