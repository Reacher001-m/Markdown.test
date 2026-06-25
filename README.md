# 左右反画像 生成プログラム flip.py



## 1. 概要
引数で指定した画像の左右判定画像を作成するpython3で動作するプログラムです。


## 2. ソースコード
```python
# このプログラムはpython3用です。
# あらかじめ pip install pillow で pillow をインストールしておきます。
from PIL import Image
import sys

# コマンドライン引用から入力画像と出力画像のファイルを取得
input=image = sys.argv[1]
output_image = sys.argv[2]

# 画像の読み込み
img_flip = img.transpose(Image.FLIP_LEFT_RIGHT)

# 画像の保存
img_flip.save{output_image}
```


## 3. 使い方


### 3.1.実行例
- コマンドラインフォーマット
```python
python3 flip.py <input_image_path> <output_image_path>
```
- 利用例
```python
python3 flip.py input.jpg output.jpg
```

### 3.2.出力結果
- 以下のように入力画像を左右反転画像が出力されます。

以上
