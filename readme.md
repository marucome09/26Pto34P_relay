# 26Pto34P_relay

![product26_1_1](https://github.com/marucome09/26Pto34P_relay/blob/master/product26_1_1.JPG )

This is 26P FDD I/F(Mitsumi/Newtronics D357B) convert to FDD for PC(or a gotek with FlashFloppy)compatible.

(26P I/F used to Yamaha SY77/SY99/V50)

ミツミ D357B FDDの26Pinの信号線を、PC用34Pに変換するボードです。

(Yamaha SY77/SY99/V50に使用されています)

注意：この機器の取り付けによって起きたいかなるトラブルに対しても、当方は（スイッチサイエンス様で販売いただいている製品版についての製品不良交換時の製品交換以外）一切の責任を負いかねます。取り付けに際しては細心の注意を払い、慎重に取り付けてください。

※なお、写真は試作品です。実際はサイズが少し大きくなります。

FDDに直接取り付けるアダプタータイプ26Pto34P_convもあります。

# Features　おすすめポイント

Designed to be attached directly to FDD(or emulator).

FDDの後方にマージンがない場合や、FDD直接接続アダプタータイプでは取り付けられないインターフェース直上に電源コネクタがあるタイプ（ミツミD353M3Dなど）でも、比較的対応しやすいアダプタータイプです。

純正に比べて小型なので、貼り付ける場所の自由度が非常に高いです。

純正の回路(XS051)と互換性があります。通常のPC用2モードFDDのほか、HxC fot Gotek、 FlashFloppy（Gotekエミュレーターのファームウェア書き換え版）にも対応します。

注意：Usageでも説明していますが、必ず取り付け面の絶縁処理を行って取り付けてください。　スイッチサイエンス様より発売される製品版は、絶縁処理を行っておりませんので、両面テープや絶縁テープなどでしっかり絶縁を行ったうえで、脱落しないようしっかり取り付けてください。また写真にあります電源部のコネクタは製品版ではオミットされておりますのでご了承ください。同様に機器＝変換ボード、変換ボード＝FDD(FDDエミュレーター）間のケーブル（26ピンフラットケーブル、34ピンフラットケーブル）もお客様でご用意ください。製品版にはついておりません。

# Requirement 制作に必要な部品

34P(17x2) pin-header or box-header  / 34ピン　ピンヘッダもしくはボックスヘッダ（FDD側 I/Fケーブル用）

26P(13x2) box-header /　26ピン ボックスヘッダ（26P I/Fケーブル用）

26Pin Flat-Cable with connectors / 26ピンフラットケーブル（両端にコネクタのついているもの）

34Pin Flat-Cable with connectors / 34ピンフラットケーブル（両端にコネクタのついているもの）

（必要な長さは機種によって違うためそれぞれの機種で確認のこと）

2P EI pin-header / 2P EI ピンヘッダ（ボードからの電源取り出し用）※

2P EI connector housing & contact / 2P EIコネクタハウジング＆コンタクト（ボードからの電源取り出し用）※

4P EI connector housing & contact / 4P EIコネクタハウジング＆コンタクト（FDD電源用）

Power Cable(必要な長さは機種によって違うためそれぞれの機種で確認のこと)

※他のコネクタでも代用可能、また基板直付けでもOK


# Making

コネクタ類を写真のようにはんだ付けします。

写真では、34Pがピンヘッダになっています（試作品のため）。26Pも、34Pも、ボックスヘッダの場合は切り欠きが下側（奇数ピン側）になるようにしてください。

![solder1](https://github.com/marucome09/26Pto34P_relay/blob/master/product26_1_1.JPG)


電源の２Pコネクタは、コネクタ側（内側）が＋極になっています。それに合わせて2pピンヘッダをつけます。

（シルク印刷されてますが写真では見にくいので強調しました、写真は26P_convのモノを使用していますが取り付け方は同じです。）

![box_socket](https://github.com/marucome09/26Pto34P_relay/blob/master/box_socket.JPG )

![box_socket2](https://github.com/marucome09/26Pto34P_relay/blob/master/box_socket2.JPG )

もしくはケーブル直付けでも構いません。

上に合わせてケーブルを作成し取り付けて完成です。

![power_conn](https://github.com/marucome09/26Pto34P_relay/blob/master/power_conn.jpg )

なお、FDD(もしくはエミュレーター）側の電源コネクタはこのように制作します。

![fddpower](https://github.com/marucome09/26Pto34P_relay/blob/master/FDD_power.jpg )

小型なので、完成するとほぼケーブルでみえなくなります。

![adapter1](https://github.com/marucome09/26Pto34P_relay/blob/master/adapter1.JPG )

![adapter2](https://github.com/marucome09/26Pto34P_relay/blob/master/adapter2.JPG )

# Usage

使い方はXS051と同様、本体内のどこかに両面テープで、金属部分が直接接触しないように、強力両面テープや、絶縁テープなどで絶縁処理を行い、脱落しないよう強力両面テープなどで機体内に貼り付けて使用します。


# Note

・信号線はDS1固定のため、DS0で動作するFDDの場合はDS1に設定を変更する必要があります。

・絶縁処理はされていませんので（Making参照のこと）、必ず基板裏面ははんだ付けのあとはショート防止もかねて、できうる限り強力タイプの、少し厚手の両面テープを使用いただくことを推奨します。他の電気箇所、金属部分への接触をしないようにとりつけてください。

・このFDDは通常のタイプ（デスクトップ用）のFDD（PC互換機用34Pピンヘッダタイプ）を想定して制作してあります。

・一部FDDで動作しない可能性があります。

・FDDはPC用ですので、2HDには対応していますが、本体が対応していないため2DD専用として動作します。
そのため、２HDディスクは使用しないでください。

☆なお、下記のFDDでチェックはパスしています（これ以外のFDDでも現物ご送付いただければ確認します、一度ご連絡ください）

Y-E DATA YD-702D

Sumsung SFD-321B

Mitsumi D353M3D


# License

This Product is CC BY-NC-SA 4.0

[![ccbyncsa](https://komtmt.files.wordpress.com/2015/04/by-nc-sa.png?w=150&h=52)](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.ja) 



