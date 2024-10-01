layout: post
title: "First chapter from fluent python"
date: 2024-09-29 12:13:00 -0000
categories: python fluent-python

# Fluent Python ch1

## 練習問題 1: `__repr__` と `__str__` の違い
`__repr__` と `__str__` の違いを理解し、以下の要件を満たす Product クラスを実装してください。

要件
Product クラスは商品名（name）、価格（price）、在庫数（quantity）を保持します。
`__repr__` メソッドでは、デバッグ目的で Product クラスのオブジェクトを再現可能な形式で出力します。
`__str__` メソッドでは、ユーザーに分かりやすい形式で商品の詳細を出力します。


``` python
product1 = Product('Laptop', 150000, 10)
product2 = Product('Smartphone', 80000, 20)

# 期待する出力
# repr(product1) -> Product('Laptop', 150000, 10)
# str(product1) -> 商品名: Laptop, 価格: 150000円, 在庫数: 10個
```