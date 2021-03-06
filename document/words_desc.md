# Words_desc
重要単語の説明です


## Python
プログラミング言語の一つ。機械学習などに強くライブラリも豊富。今回はサーバー側（Raspberry Pi）で使用する。学習しやすい、共同開発する時に扱いやすいため今回はPythonを選択した。バージョンはPython3.7を使用。理由は最新の中でも3.10は大きく変わるし2.xは論外だから。


## Arduino言語
**C/C++言語がベース**となったプログラミング言語。処理が早い。今回は機体側（esp32）で使用する。MicroPythonも使用できるが主に開発は一人であることやサンプルが多いこと、**処理速度重視**のため選択した。


## Raspberry Pi 4B
マイコンの一つ。OSが入っており性能が高くwebサーバー等に使用できる。今回は**交差点の一元管理**や**最短経路探索**においてサーバーとして使用する。


## esp32
マイコンの一つ。デフォルトでWiFi、Bluetoothを使用できるのが特徴。今回使用した**Lolin D32**はバッテリーインターフェースもついている。今回は車体の**直接制御用**で使用する。


## RC522
NFCタグを検知するモジュール。NFCの規格の一つであるMifareに対応している。Mifareに対してFelicaがある。タグもモジュールもFelicaより**安価**なため選んだ。


## A*アルゴリズム
最短経路探索で使用されるアルゴリズムの一つ。**ダイクストラ法**が基本となっていて、目的地とそのノード（分岐点）の直線距離などを比較して次に探索するノードを決める。


## TCP通信
通信方法の一つ。TCPというプロトコルを使用した通信。同様なものに**UDP通信**がある。
TCPは通信を確立した後にデータを送信するため**信頼性が高い**一方、UDPは一方的に送り付けるため**送信速度は早い**が信頼性は低い。

## Socket通信（不確実）
Socketを使用した通信方法。Socketとは通信の出入り口のことで通信したい互いのSocketを接続することで通信ができる。Socket通信にはTCPやUDPを使用したものがある。今回はSocket通信（特にTCP通信）を使用する。

## Flask
Pythonでwebサーバーを立てられるフレームワーク。今回は機体に最短経路を返すwebAPIとして返す。
