==========================================================
USB Vendor-ID 申請方法 (メモ書き)
==========================================================

- 公式サイト: https://www.usb.org/getting-vendor-id



USBのベンダーIDを取得するための方法
------------------------------------------------------------

1. USB-IFのメンバーになる

    規約と申込書:https://www.usb.org/sites/default/files/usb-if_member_agreement_080618_1.pdf

    翻訳:https://github.com/nonNoise/USB-Getting-a-Vendor-ID/blob/master/USB-IF.rst


2. USB-IF非会員でロゴのライセンシーを払う

    別途、ロゴ利用契約が必要らしい（詳細まで調べてない）

3. ベンダーIDだけ取得する

    規約と申込書:https://www.usb.org/sites/default/files/vid_only_form_070119.pdf

    翻訳:https://github.com/nonNoise/USB-Getting-a-Vendor-ID/blob/master/VendorID.rst


ベンダーIDだけを取得する
------------------------------------------------------------


申込書しか記載がない為、著名したPDFをメールで送信すると良いのかな？

Email: admin@usb.org

１ベンダーIDで32ビット幅(65535台)分のプロダクトを管理して良いらしい


支払い方法
------------------------------------------------------------

USB-IF曰く:

    US $ 6,000.00の1回限りの処理料金が必要です。 
    Visa、MasterCard、American Express、会社の小切手、電信送金でのお支払いを受け付けています。 

惜しくも2020年に確認したところ、6000ドル（約66万円）になってて悲しい。

ベンダーが増えれば価格も増えるギミックでもあるのかな。


登録済みベンダーIDリスト
------------------------------------------------------------

https://www.usb.org/sites/default/files/vendor_ids052019.pdf


プロダクトIDの割当案
------------------------------------------------------------

禁止番号 (なんとなく禁止する)

::
    0x0000
    0x1111
    0x2222
    0x3333
    0x4444
    0x5555
    0x6666
    0x7777
    0x8888
    0x9999
    0xAAAA
    0xBBBB
    0xCCCC
    0xDDDD
    0xEEEE
    0xFFFF

開発用番号　（販売せずパートナーのみで使用)

::
    0x1234
    0x5678
    0xABCD
    0x5A5A
    0xA5A5

AN利用配布用ID　(HIDドライバ)　4095台分

::
    0x1000
      |
    0x1FFF

AN利用配布用ID　(その他ドライバ)　　4095台分

::
    0x2000
      |
    0x2FFF

その他配布用ID

    0x3000
      |
    0x3FFF
