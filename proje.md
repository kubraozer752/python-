# python-
1- Bir listeyi düzleştiren (flatten) fonksiyon yazın. Elemanları birden çok katmanlı listelerden ([[3],2] gibi) oluşabileceği gibi, non-scalar verilerden de oluşabilir. Örnek olarak:

input: [[1,'a',['cat'],2],[[[3]],'dog'],4,5]

output: [1,'a','cat',2,3,'dog',4,5]

```py
def flatten(l):
  return flatten(l[0]) + (flatten(1[1:]) if len(l) > 1 else []) if type(l) is list else [1]
flatten ([[1,'a',['cat'],2],[[[3]],'dog'],4,5])
```
