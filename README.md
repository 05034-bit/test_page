# 左右反転画像 生成プログラムflip.py
1.概要
引数で指定した画像の左右反転画像を生成する python3で動作するプログラムです。

2.ソースコード

# このプログラムは python3用です。
# あらかじめ pip install pillow で pillow をインストールしておきます。
form PIL import Image
import sys

# コマンドライン引用から入力画像のファイル名を取得
input_image = sys.argv[1]
output_image = sys.srgv[2]

# 画像の読み込み
img = Image.open(input_image)

# 画像の左右反転
img_flip = img.transpose(Image.FLIP_LEFI_RIGHT)

# 画像の保存
img_flip.save(output_image)