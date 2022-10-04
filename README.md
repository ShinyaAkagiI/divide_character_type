# 概要

文字列をひらがな、片仮名、漢字、数字、アルファベットごとに分割するツールです。
英日両文に適用可能ですが、ピリオドを含む一部の用語は適切に分割できない場合があります。
詳しくは、実行サンプルをご確認ください。


# 使い方

"""
from divide_char_type import divide_char_type

data = divide_char_type("今日の天気は晴れです。")

print(data[0])
"""


# 実行サンプル

"""
['1.0', ' ', 'is', ' ', 'number', '.']
['1,000', ' ', 'is', ' ', 'number', '.']
['u.s.a.', ' ', 'is', ' ', 'state', '.']
['u.k', '.', ' ', 'is', ' ', 'state', '.']
['e.g.', ',', ' ', 'th', ',', ' ', 'ch', ',', ' ', 'sh', ',', ' ', 'ph', ',', ' ', 'gh', ',', ' ', 'ng', ',', ' ', 'qu']
['state', ' ', 'include', ' ', 'u.s.', ' ', 'u.s.', ' ', 'is', ' ', 'state', '.']
['state', ' ', 'include', ' ', 'u.k', '.', ' ', 'u.k', '.', ' ', 'is', ' ', 'state', '.']
['u.s.', 'は', '国', 'です', '。']
['u.s', '.', 'は', '国', 'です', '。']
['あいうえおーかきくけこ']
['アイウエオーカキクケコ']
['今日', 'の', '天気', 'は', '晴', 'れです', '。', '\n', '明日', 'の', '天気', 'は', '曇', 'りです', '。', '\n']
"""