# [配列メニュー](https://paiza.jp/works/mondai/array_primer/problem_index?language_uid=javascript)

## 【次元配列の入出力】i番目の出力 Boss

### [STEP: 1 要素数の出力](https://paiza.jp/works/mondai/array_primer/array_primer__1dmatrix_output_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return split(' ')('5 1 3 4 5 12 6 8 1 3').length
}
// 入力がないため書き換え
const lines = []
```
### [STEP: 2 全要素の出力]()
```js
const fun = (...args) => {
  return split(' ')('5 1 3 4 5 12 6 8 1 3')
}
// 入力がないため書き換え
const lines = []
print(join('\n'))(fun(...lines))
```

### [STEP: 3 i 番目の出力](https://paiza.jp/works/mondai/array_primer/array_primer__1dmatrix_output_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return split(' ')('5 1 3 4 5 12 6 8 1 3')[4 - 1]
}
// 入力がないため書き換え
const lines = []
```

### [STEP: 4 配列の入力 1](https://paiza.jp/works/mondai/array_primer/array_primer__1dmatrix_input_step1/edit?language_uid=javascript)
```js
const fun = (...args) => {
  return split(' ')('8 1 3 3 8 1 1 3 8 8')
}
// 入力がないため書き換え
const lines = []
print(join('\n'))(fun(...lines))
```

### [STEP: 5 配列の入力 2](https://paiza.jp/works/mondai/array_primer/array_primer__1dmatrix_input_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return split(' ')(args[0])
}

print(join('\n'))(fun(...lines))
```

### [STEP: 6 配列の入力 3](https://paiza.jp/works/mondai/array_primer/array_primer__1dmatrix_input_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [N, AS] = toList(split(' '))(args)
  return AS.flat(())
}

print(join('\n'))(fun(...lines))
```

### [STEP: 7 i番目の出力 1](https://paiza.jp/works/mondai/array_primer/array_primer__1dmatrix_i-thoutput_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const K = toInt(args)
  return split(' ')('1 3 5 4 6 2 1 7 1 5')[K - 1]
}
```

### [STEP: 8 i番目の出力 2](https://paiza.jp/works/mondai/array_primer/array_primer__1dmatrix_i-thoutput_step2/edit?language_uid=javascript)
```js
const fun = (...args) => {
  const [K, AS] = toList(split(' ', toInt))(args)
  return AS.flat()[K - 1]
}
```

### [final 次元配列の入出力】i番目の出力 Boss](https://paiza.jp/works/mondai/array_primer/array_primer__1dmatrix_i-thoutput_boss/edit?language_uid=javascript)
```js
const fun = (...args) => {
  const [[N, K], AS] = toList(split(' ', toInt))(args)
  return AS.flat()[K - 1]
}
```

## 【二次元配列の入出力】i番目の出力 Boss

### [STEP: 1 要素数の出力](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_output_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const matrix = toList(split(' '))(['1 2 3 4 5 6','8 1 3 3 1 8'])
  return matrix.flat().length
}
// 入力がないため書き換え
const lines = []
```

### [STEP: 2 全要素の出力](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_output_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const matrix = toList(split(' '))(['6 5 4 3 2 1', '3 1 8 8 1 3'])
  return toList(join(' '))(matrix)
}
// 入力がないため書き換え
const lines = []
print(join('\n'))(fun(...lines))
```

### [STEP: 3 行数の出力](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_output_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const matrix = toList(split(' '))(['1 2 3', '4 5 6', '8 1 3'])
  return matrix.length
}

const lines = []
```

### [STEP: 4 列数の出力](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_output_step4/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const matrix = toList(split(' '))([
    '1 2 3 4',
    '6 5 4 3',
    '3 1 8 1'
  ])
  return matrix[0].length
}
const lines = []
```

### [STEP: 5 各行の要素数の出力](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_output_step5/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const matrix = toList(split(' '))([
    '1',
    '2 3',
    '4 5 6'
  ])
  return matrix.map(v => v.length)
}
const lines = []
print(join('\n'))(fun(...lines))
```
### [STEP: 6 i 行目 j 列目の出力](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_output_step6/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const matrix = toList(split(' '))([
    '1 2 3',
    '8 1 3',
    '10 100 1'
  ])
  return matrix[2 - 1][3 - 1]
}
const lines = []

```

### [STEP: 7 二次元配列の入力 1](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_input_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [M, matrix] = toList(split(' '))([
    '1 3 5 7',
    '8 1 3 8'
  ])
  return toList(join(' '))(matrix)
}
const lines = []
print(join('\n'))(fun(...lines))

```


### [STEP: 8 二次元配列の入力 2](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_input_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[M], ...matrix] = toList(split(' '))(args)
  return toList(join(' '))(matrix)
}
print(join('\n'))(fun(...lines))
```

### [STEP: 9 二次元配列の入力 3](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_input_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N], ...matrix] = toList(split(' ', toInt))(args)
  return toList(join(' '))(matrix)
}
print(join('\n'))(fun(...lines))
```
### [STEP: 10 二次元配列の入力 4](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_input_step4/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M], ...matrix] = toList(split(' '))(args)
  return toList(join(' '))(matrix)
}
print(join('\n'))(fun(...lines))
```

### [STEP: 11 i番目の出力 1](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_i-thoutput_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [K, L] = split(' ', toInt)(args[0])
  const a = toList(split(' ', toInt))([
    '1 2 3 4',
    '10 100 0 5',
    '8 1 3 8',
    '15 34 94 25'
  ])
  return a[K - 1][L - 1]
}
```

### [STEP: 12 i番目の出力 2](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_i-thoutput_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[K, L], ...matrix] = toList(split(' ', toInt))(args)
  return matrix[K - 1][L - 1]
}
```

### [final 二次元配列の入出力】i番目の出力 Boss](https://paiza.jp/works/mondai/array_primer/array_primer__2dmatrix_i-thoutput_boss/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M, K, L], ...matrix] = toList(split(' ',toInt))(args)
  return matrix[K - 1][L - 1]
}
```


## 【配列の検索】何個ある? Boss

### [STEP: 1 配列に含まれている? 1](https://paiza.jp/works/mondai/array_primer/array_primer__search_include_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return split(' ')('10 13 21 1 6 51 10 8 15 6').includes('6')
    ? 'Yes'
    : 'No'
}

// 入力がないため書き換え
const lines = []
```


### [STEP: 2 配列に含まれている? 2](https://paiza.jp/works/mondai/array_primer/array_primer__search_include_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const N = toInt(args[0])
  return split(' ', toInt)('5 12 6 84 14 25 44 3 7 20').includes(N)
    ? 'Yes'
    : 'No'
}

```
### [STEP: 3 配列に含まれている? 3](https://paiza.jp/works/mondai/array_primer/array_primer__search_include_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M], AS] = toList(split(' ', toInt))(args)
  return AS.flat().includes(M)
    ? 'Yes'
    : 'No'
}
```

### [STEP: 4 何番目にある? 1](https://paiza.jp/works/mondai/array_primer/array_primer__search_i-th_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return split(' ')('1 10 2 9 3 8 4 7 5 6').indexOf('8') + 1
}

// 入力がないため書き換え
const lines = []
```
### [STEP: 5 何番目にある? 2](https://paiza.jp/works/mondai/array_primer/array_primer__search_i-th_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const N = toInt(args[0])
  return split(' ', toInt)('1 5 9 7 3 2 4 8 6 10').indexOf(N) + 1
}
```

### [STEP: 6 何番目にある? 3](https://paiza.jp/works/mondai/array_primer/array_primer__search_i-th_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M], AS] = toList(split(' ', toInt))(args)
  return AS.indexOf(N) + 1
}
```

### [STEP: 7 何個ある? 1](https://paiza.jp/works/mondai/array_primer/array_primer__search_count_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return split(' ')('1 2 2 1 2 1 2 1 1 1')
    .filter(v => v === '1').length
}
// 入力がないため書き換え
const lines = []
//  別解
//  return split('1')('1 2 2 1 2 1 2 1 1 1').length - 1
//  return '1 2 2 1 2 1 2 1 1 1'.match(/1/g).length
```
### [STEP: 8 何個ある? 2](https://paiza.jp/works/mondai/array_primer/array_primer__search_count_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const N = toInt(args[0])
  return split(' ')('1 2 5 1 4 3 2 5 1 4')
    .filter(v => v === N).length
}
```

### [final【配列の検索】何個ある? Boss](https://paiza.jp/works/mondai/array_primer/array_primer__search_count_boss/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M], AS] = toList(split(' ', toInt))(args)
  return AS.filter(v => v === N).length
}
```

## 【文字列の配列】辞書順に出力 Boss

### [STEP: 1 配列の書き換え](https://paiza.jp/works/mondai/array_primer/array_primer__elm_rewrite/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[A, B, N], AS] = toList(split(' ', toInt))(args)
  return AS.map(v => v === A ? B : v)
}
```

### [STEP: 2 2 変数の入れ替え](https://paiza.jp/works/mondai/array_primer/array_primer__elm_change/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [A, B] = split(' ')(args)
  return [A, B].reverse()
}

print(join(' '))(fun(...lines))
```

### [STEP: 3 配列の要素の入れ替え](https://paiza.jp/works/mondai/array_primer/array_primer__array_elm_change/edit?language_uid=javascript)
```js
const fun = (...args) => {
  const [[A, B, N], AS] = toList(split(' ', toInt))(args)
  ;[AS[A - 1], AS[B - 1]] = [AS[B - 1], AS[A - 1]]
  return AS
}
print(join(' '))(fun(...lines))
```

### [STEP: 4 部分配列](https://paiza.jp/works/mondai/array_primer/array_primer__partical_array/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[A, B, N], AS] = toList(split(' ', toInt))(args)
  return slice(A - 1, B)(AS)
}
print(join(' '))(fun(...lines))
```

### [STEP: 5 配列の連結](https://paiza.jp/works/mondai/array_primer/array_primer__array_join/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M], AS, BS] = toList(split(' ', toInt))(args)
  return [...AS, ...BS]
}
print(join(' '))(fun(...lines))
```


### [STEP: 6 配列のソート](https://paiza.jp/works/mondai/array_primer/array_primer__array_sort/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N], AS] = toList(split(' ', toInt))(args)
  return [...AS].sort((a, b) => a - b)
}
```

### [STEP: 7 配列の反転](https://paiza.jp/works/mondai/array_primer/array_primer__array_reverse/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N], AS] = toList(split(' ', toInt))(args)
  return [...AS].reverse()
}
```
### [STEP: 8 要素のカウント](https://paiza.jp/works/mondai/array_primer/array_primer__elm_count/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M], AS] = toList(split(' ', toInt))(args)
  return AS.filter(v => v === M).length
}

print(join('\n'))(fun(...lines))
```

### [STEP: 9 配列末尾への追加](https://paiza.jp/works/mondai/array_primer/array_primer__push_back/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M], AS] = toList(split(' ', toInt))(args)
  return [...AS, M]
}

print(join('\n'))(fun(...lines))
```

### [STEP: 10 要素の削除](https://paiza.jp/works/mondai/array_primer/array_primer__elm_erase/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M], AS] = toList(split(' ', toInt))(args)
  const clone = [...AS]
  clone.splice(M - 1, 1)
  return clone
}
print(join('\n'))(fun(...lines))
// 別解
// return [...slice(0, M - 1)(AS), ...slice(M)(AS)]
```


### [STEP: 11 要素の挿入](https://paiza.jp/works/mondai/array_primer/array_primer__elm_insert/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M, K], AS] = toList(split(' ', toInt))(args)
  const clone = [...AS]
  clone.splice(M - 1, 0, K)
  return clone
}
print(join('\n'))(fun(...lines))
// 別解
// return [...slice(0, M)(AS), K, ...slice(M)(AS)]
```

### [STEP: 12 要素数の出力](https://paiza.jp/works/mondai/array_primer/array_primer__string_output_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return [
    'Hello',
    'paiza',
    '1234',
    'pa13'
  ].length
}

const lines = []
```


### [STEP: 13 全要素の出力](https://paiza.jp/works/mondai/array_primer/array_primer__string_output_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return [
    'good',
    'morning',
    'paiza',
    '813',
    'pa13'
  ]
}
const lines = []
```


### [STEP: 14 i 番目の出力](https://paiza.jp/works/mondai/array_primer/array_primer__string_output_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return [
    'good',
    'morning',
    'paiza',
    '813',
    'pa13'
  ][3 - 1]
}
const lines = []
```

### [STEP: 15 文字列の配列の入力 1](https://paiza.jp/works/mondai/array_primer/array_primer__string_input_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return [
    'eight',
    'one',
    'three',
    'paiza',
    'pa13',
    '813'
  ]
}
print(join('\n'))(fun(...lines))
```


### [STEP: 16 文字列の配列の入力 2](https://paiza.jp/works/mondai/array_primer/array_primer__string_input_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const SS = split(' ')(args[0])
  return SS
}
print(join('\n'))(fun(...lines))
```

### [STEP: 17 文字列の配列の入力 3](https://paiza.jp/works/mondai/array_primer/array_primer__string_input_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N], SS] = toList(split(' '))(args)
  return SS
}
print(join('\n'))(fun(...lines))
```
### [STEP: 18 i 番目の出力 1](https://paiza.jp/works/mondai/array_primer/array_primer__string_i-thinput_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const N = toInt(args[0])
  return [
    'good',
    'morning',
    'paiza',
    '813',
    'pa13',
  ][N - 1]
}
```


### [STEP: 19 i 番目の出力 2](https://paiza.jp/works/mondai/array_primer/array_primer__string_i-thinput_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N], SS] = toList(split(' '))(args)
  return SS[toInt(N) - 1]
}
```


### [STEP: 20 i 番目の出力 3](https://paiza.jp/works/mondai/array_primer/array_primer__string_i-thinput_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M], SS] = toList(split(' '))(args)
  return SS[toInt(N) - 1]
}
```


### [STEP: 21 i 番目の出力 4](https://paiza.jp/works/mondai/array_primer/array_primer__string_i-thinput_step4/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, M, L], SS] = toList(split(' '))(args)
  return SS[toInt(N) - 1][toInt(L) - 1]
}
```


### [STEP: 22 辞書順に出力 1](https://paiza.jp/works/mondai/array_primer/array_primer__string_dictionary_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return split(' ')('zaipa izapa paiza').sort()
}
const lines = []
```

### [STEP: 23 辞書順に出力 2](https://paiza.jp/works/mondai/array_primer/array_primer__string_dictionary_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const SS = split(' ')(args[0])
  return [...SS].sort()
}
print(join('\n'))(fun(...lines))
```


### [STEP: 24 辞書順に出力 3](https://paiza.jp/works/mondai/array_primer/array_primer__string_dictionary_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N], SS] = toList(split(' '))(args)
  return [...SS].sort()
}
print(join('\n'))(fun(...lines))
```

### [final 文字列の配列】辞書順に出力 Boss](https://paiza.jp/works/mondai/array_primer/array_primer__string_dictionary_boss/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, K], SS] = toList(split(' '))(args)
  return [...SS].sort()[toInt(K) - 1]
}
```

## フィボナッチ数

### [STEP: 1 重複の削除](https://paiza.jp/works/mondai/array_primer/array_primer__deduplication/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const list = split(' ', toInt)('1 3 5 1 2 3 6 6 5 1 4')
  return [...new Set(list)].sort()
}
print(join('\n'))(fun(...lines))
```

### [STEP: 2 配列の最大最小](https://paiza.jp/works/mondai/array_primer/array_primer__array_minmax/edit?language_uid=javascript)
```js
const fun = (...args) => {
  const [[N], AS] = toList(split(' ', toInt))(args)
  return [Math.max(...AS), Math.min(...AS)]
}
print(join(' '))(fun(...lines))
```

### [STEP: 3 ある数以上以下の要素の列挙 1](https://paiza.jp/works/mondai/array_primer/array_primer__array_ave_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N], AS] = toList(split(' ', toInt))(args)
  return AS.filter(v => v >= 5)
}
print(join('\N'))(fun(...lines))
```
### [STEP: 4 ある数以上以下の要素の列挙 2](https://paiza.jp/works/mondai/array_primer/array_primer__array_ave_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, K], AS] = toList(split(' ', toInt))(args)
  return AS.filter(v => v >= K)
}
print(join('\N'))(fun(...lines))
```

### [STEP: 5 ある数以上以下の要素の列挙 3](https://paiza.jp/works/mondai/array_primer/array_primer__array_ave_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const f = a => a.reduce((a, b) => a + b) / a.length
  const [[N], AS] = toList(split(' ', toInt))(args)
  return AS.filter(v => v >= f(AS))
}
print(join('\N'))(fun(...lines))
```
### [STEP: 6 二点間の距離 1](https://paiza.jp/works/mondai/array_primer/array_primer__array_distance_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const f = (x1, y1) => ([x2, y2]) => Math.abs(x1 - x2) + Math.abs(y1 - y2)
  const [[N], ...AS] = toList(split(' ', toInt))(args)
  return AS.map(f(2, 3))
}
```

### [STEP: 7 二点間の距離 2](https://paiza.jp/works/mondai/array_primer/array_primer__array_distance_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const f = (x1, y1) => ([x2, y2]) => Math.abs(x1 - x2) + Math.abs(y1 - y2)
  const [[N, A, B], ...AS] = toList(split(' ', toInt))(args)
  return f(...AS[A - 1])(AS[B - 1])
}

```

### [final  フィボナッチ数](https://paiza.jp/works/mondai/array_primer/array_primer__fibo/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const N = toInt(args[0])
  const f = (a, b) => (acc, _) => {
    acc.push(a)
    ;[a, b] = [b, a + b]
    return acc
  }
  return range(N).reduce(f(0, 1), [])
}
```

