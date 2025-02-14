# ADKB96_MZ80K
[ビット・トレード・ワン](https://bit-trade-one.co.jp/)より発売中の96キー セルフメイドキーボードキット「[ADKB96](https://bit-trade-one.co.jp/selfmadekb/adkb96/)」を使って、MZ-80Kシリーズ風USBキーボードを作ってみました。

## 必要なもの
- ADKB96
- キースイッチ(CherryMXまたは互換) 96個
- キーキャップ
  - 透明カバー式(2層またはdual layerなどと表記)
    - 1Uサイズ(標準幅) 76個
    - 2Uサイズ(倍幅) 2個
  - 一般的なもの
    - 16個

96キーのうちMZのキーとして必要なのは80キーで、残り16キーはMZ用に割り当てなかったキーに充てます。

## ファームウェア
[QMK Configurator](https://config.qmk.fm/#/adkb96/rev1/LAYOUT_ortho_6x16)を利用して制作しました。アップロードしてあるファームでのキー配列は以下のようになっています。これは、[武田氏](http://takeda-toshiya.my.coocan.jp/)制作の[MZ-80Kエミュレータ](http://takeda-toshiya.my.coocan.jp/mz80k/index.html)に対応したものです。

![key layout](/assets/layout.png)

[JSONファイル](/firmware/mz80k.json)をQMK Configuratorにアップロードすれば、お好みの配列に変更できます。特に最上段のMZ用以外のキー配列については好みの分かれるところかと思います。ただし、Num Lockされていない状態でエミュレータを使用すると(特にノートPC)、テンキーに割り当てられたキーが正常に入力されなくなりますので、Num Lockキーは配置しておくことをお勧めします。

[hexファイル](/firmware/adkb96_rev1_mz80k.hex)を[QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases)でマイコンモジュールに書き込めばその配列で使用できるようになります。QMK関連のソフトについては、ビット・トレード・ワンのサイトにある[ソフトウェア情報](https://bit-trade-one.co.jp/selfmadekb/softwaremanual/)に使用方法が説明されていますので参考にしてください。

## キーラベル
MZ-80K/Cシリーズのうち、格子状にキーが配列された次の4機種のラベルを作りました。
### MZ-80K
### MZ-80K(輸出仕様)
### MZ-80K2
### MZ-80K2E

A4の紙にカラー印刷して、切り抜いて使用してください。いずれもスキャン等ではなく見た目から手作業で作ったものなので、字形や色合いなど細かい差異があるかとは思います。
