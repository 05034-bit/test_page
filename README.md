# 左右反転画像 生成プログラムflip.py

## 1\. 概要

引数で指定した画像の左右反転画像を生成する python3で動作するプログラムです。

## 2\. ソースコード

``` # このプログラムは python3用です。
# あらかじめ pip install pillow で pillow をインストールしておきます。
form PIL import Image
import sys

# コマンドライン引用から入力画像のファイル名を取得
input\_image = sys.argv\[1]
output\_image = sys.srgv\[2]

# 画像の読み込み
img = Image.open(input\_image)

# 画像の左右反転
img\_flip = img.transpose(Image.FLIP\_LEFI\_RIGHT)

# 画像の保存
img\_flip.save(output\_image)
```

## 3\. 使い方

**3.1. 実行例**

* コマンドラインフォーマット

`　python3 flip.py <input\_image\_path> <output\_image\_path>`

* 利用例

`　python3 flip.py input.jpg output.jpg`

**3.2. 出力結果**

* 以下のように入力画像の左右反転画像が出力されます。

|  入力画像(input.jpg) | 出力画像(output.jpg) |
| --- | --- |
| ![入力画像](input.jpg) | ![出力画像](output.jpg) |





