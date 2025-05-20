# 電装新歓2025
電装班に興味を持ってくれてありがとう！  
えっ？もう作業体験を終えたのかい？じゃあもう君は立派な電装班員だ！
ぜひ[秋葉原ツアー](otherContents/AkihabaraTour2025.md)にも参加してくれ！

## 電装班とは
鳥人間コンテストの滑空機に搭載する以下のような装置を開発しています．
- 高度測定装置
- 機速測定装置
- 測定データ収集・保存装置
- 操縦装置

## 作業体験
### [AtCorder](https://atcoder.jp/contests/apg4b)
電装班ではArduinoIDEを用いてプログラムの作成をします．
その際，C言語（正確にはC++も含む）と呼ばれるプログラミング言語を使用します．
今後使えるようになるために，[AtCorder](https://atcoder.jp/contests/apg4b)という競技プログラミングサイトで練習をしましょう！
電装班では1章まで進めてもらえば、鳥科で使うプログミングの基礎としては十分です。

### [鳥科電装勉強](https://geode-kicker-e37.notion.site/f4303f1da5d94d21af8da94cfff05153)
作成したプログラムはマイコンと呼ばれるものに書き込むことができます．
マイコンによって，プログラムした動作を実現することができます．
[こちら](https://geode-kicker-e37.notion.site/f4303f1da5d94d21af8da94cfff05153)は電装班の先輩方が作ってくださったマイコンの基礎を学べるサイトです．
「[実践編！](https://geode-kicker-e37.notion.site/1d0f665803ce807fb891f5df901ba133)」などを参考に実際にマイコンを動かしてみましょう！

参考ページは以下
- [ラズパイPico/Pico2/PicoWのArduinoIDE2のインストール方法や使い方紹介｜ロジカラブログ](https://logikara.blog/raspi-pico-arduinoide/)
- [Arduino日本語リファレンス｜株式会社武蔵野電波](http://www.musashinodenpa.com/arduino/ref/)
- [Download Arduino IDE](https://www.arduino.cc/en/software/)

<img src="images/download_arduino_ide.png" width=600px>

- 追加のボードマネージャーのURL  
  ```
  https://github.com/earlephilhower/arduino-pico/releases/download/global/package_rp2040_index.json
  ```

<img src="images/pico_pin_assign.jpg" width=600px>

### Lチカ基盤のPCB作成
電装班では，マイコンなどを搭載するプリント基盤を外部の業者に発注しています．
発注するためにはプリント基板のデータを作成する必要があります．
そこで使用するのが「[Kicad](https://www.kicad.org/download/)」です．
実際にダウンロードして使ってみましょう！

> 新歓対応をする26代へ

> 手順は以下の通りです．
> - GitHubからZIPファイルをダウンロードし展開してもらいます．
> - 回路図エディターを開き，配置と配線をしてもらいます．（フットプリントの割り当ては完了しています）
> - 配線が完了したら，PCBエディターで基板設計をしてもらいます．（70mmx35mmの外形を設定してあります）
> - 実際の基盤を渡してあげるとイメージしやすいかもしれません．

下の画像はクリックすると開くことができます．

<img src="images/SCH_Astable_Multivibrator.png" style="height:300px;"><img src="images/PCB_Astable_Multivibrator.png" style="height:300px;">

### Lチカ基盤のはんだ付け
実際に動く装置を作るにはプリント基板に部品をつけなくてはなりません．
その際には「はんだ付け」という作業が必要になります．
ちょっとコツがいりますが，きっとうまくできるはずです！
先程の回路図を見てはんだ付けをし，LEDを光らせましょう！


必要部品は以下の通り (4/9時点での在庫)
- LED x2 (48個)
- 抵抗 x4
  - R1,R4 1kΩ (50個以上)
  - R2,R3 10kΩ (50個以上)
- NPN型トランジスタ x2 (20個以上)
- コンデンサ x2 (80個以上)
  - 容量は任意．点滅スピードが変わって面白いぞ．
- ボタン電池取り付け用ホルダー (13個)
- CR2032 (3個)


はんだ付けはとにかくやけどに注意してください！

[こちら](https://fujimoostudios.org/?p=66)のページでははんだ付けについて詳しく解説してくれていますので，目を通しておいてください！
