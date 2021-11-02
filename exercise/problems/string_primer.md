# [文字列処理メニュー](https://paiza.jp/works/mondai/string_primer/problem_index?language_uid=javascript)

## [文字列の出力](https://paiza.jp/works/mondai/string_primer/basic_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return 'paiza'
}

// 入力がないので直接書き換え
const lines = ['']
```

## [文字列の受け取り](https://paiza.jp/works/mondai/string_primer/basic_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  return args[0]
}
```

## [i 文字目の出力](https://paiza.jp/works/mondai/string_primer/basic_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [S, i] = args
  return S.charAt(toInt(i) - 1)
}
```

## [文字列の条件判定](https://paiza.jp/works/mondai/string_primer/basic_step4/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const S = args
  return S === 'paiza'
    ? 'YES'
    : 'NO'
}
```

[文字列の文字数](https://paiza.jp/works/mondai/string_primer/basic_step5/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const S = args
  return S.length
}
```

## [文字の検索](https://paiza.jp/works/mondai/string_primer/basic_step6/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [S, c] = args
  return S.indexOf(c) + 1
}
```

## [文字列の連結](https://paiza.jp/works/mondai/string_primer/basic_step7/edit?language_uid=javascript)


```js
const fun = (...args) => {
  const [N, ...rest] = args
  return slice(0, toInt(n))(rest).join('')
}
// return rest.join('') でも良い
```

## [部分文字列](https://paiza.jp/works/mondai/string_primer/normal_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[S], ij] = toList(split(' '))(args)
  const [i, j] = toList(toInt)(ij)
  return slice(i - 1, j - 1)(S)
}
```

## [文字列の挿入](https://paiza.jp/works/mondai/string_primer/normal_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [S, T, N] = args
  const [front, back] = [slice(0, toInt(N))(S), slice(toInt(N))(S)]
  return [front, T, back].join('')
}
```

## [文字列の書き換え](https://paiza.jp/works/mondai/string_primer/normal_step3?language_uid=javascript)

```js
const fun = (...args) => {
  const [[S], [i, c]] = toList(split(' '))(args)
  const [front, back] = [slice(0, toInt(i) - 1)(S), slice(toInt(i))(S)]
  return [front, c, back].join('')
}

// 別解
  const acc = Array.from(S)
  acc[toInt(i) - 1] = c
  return array.join('')
```

## [文字列から数値への変換](https://paiza.jp/works/mondai/string_primer/normal_step4?language_uid=javascript)

```js
const fun = (...args) => {
  const [S] = args
  return toInt(S) - 813
}
```

## [数値から文字列への変換](https://paiza.jp/works/mondai/string_primer/normal_step5?language_uid=javascript)

```js
const fun = (...args) => {
  const [X, Y, N] = toList(toInt)(args)
  return toStr(X + Y).charAt(N - 1)
}

```

## [大文字から小文字への変換](https://paiza.jp/works/mondai/string_primer/normal_step6?language_uid=javascript)

```js
const fun = (...args) => {
  const [S] = args
  return S.toLowerCase()
}
```

## [小文字から大文字への変換](https://paiza.jp/works/mondai/string_primer/normal_step7?language_uid=javascript)

```js
const fun = (...args) => {
  const [S] = args
  return S.toUpperCase()
}
```

## [大文字小文字の反転](https://paiza.jp/works/mondai/string_primer/normal_step8?language_uid=javascript)

```js
const fun = (...args) => {
  const f = c => /[A-Z]/.test(c) ? c.toLowerCase() : c.toUpperCase() 
  const [S] = args
  return S.replace(/[A-Z]/ig, f)
}
```

## [文字列の検索 ](https://paiza.jp/works/mondai/string_primer/normal_step9?language_uid=javascript)

```js
const fun = (...args) => {
  const [S, T] = args
  return S.includes(T)
    ? 'YES'
    : 'NO'
}
```

## [文字列の反転](https://paiza.jp/works/mondai/string_primer/normal_step10/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [S] = args
  return Array.from(S).reverse().join('')
}
```

## [回文判定](https://paiza.jp/works/mondai/string_primer/normal_step11?language_uid=javascript)

```js
const fun = (...args) => {
  const f = s => Array.from(s).reverse().join('')
  const [S] = args
  return S === f(S)
    ? 'YES'
    : 'NO'
}
```

## [文字列の分割](https://paiza.jp/works/mondai/string_primer/advance_step1?language_uid=javascript)

```js
const fun = (...args) => {
  const [S] = args
  return split(',')(S)
}

print(join('\n'))(fun(...lines))
```

## [日時データの変換その1](https://paiza.jp/works/mondai/string_primer/advance_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [yyyy, MM, dd, hhmm] = split('/', args[0])
  const [hh, mm] = split(':')(hhmm)
  return [yyyy, MM, dd, hh, mm]
}

print(join('\n'))(fun(...lines))
```

## [日時データの変換その2](https://paiza.jp/works/mondai/string_primer/advance_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [yyyyMMdd, hhmm] = split(' ', args[0])
  const [yyyy, MM, dd] = split('/')(yyyyMMdd)
  const [hh, mm] = split(':')(hhmm)
  return [yyyy, MM, dd, hh, mm]
}

print(join('\n'))(fun(...lines))

```

## [数値判定](https://paiza.jp/works/mondai/string_primer/advance_step4/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [S] = args
  return isNaN(S)
    ? 'NO'
    : 'YES' 
}
```
別解

```js
const fun = (...args) => {
  const [S] = args
  return /^\d*$/.test(S)
    ? 'YES'
    : 'NO' 
}
```


## [重複の削除](https://paiza.jp/works/mondai/string_primer/advance_step5?language_uid=javascript)

```js
const fun = (...args) => {
  const [S] = args
  const set = new Set(S)
  return [...set].join('')
}
```

## [パスワード作成](https://paiza.jp/works/mondai/string_primer/advance_step6?language_uid=javascript)

```js

const fun = (...args) => {
  const [N, Q, ...rest] = args
  const [matrix, [m]] = split(' ')(rest)

}
```

## [表記の訂正](https://paiza.jp/works/mondai/string_primer/advance_step7/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [S] = args

}
```

## [数式の計算（1 桁）](https://paiza.jp/works/mondai/string_primer/advance_step8/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const add = (a, b) => a + b
  const sub = (a, b) => a - b
  const f = (acc, v) => {
    const table = new Map([['+', add], ['-', sub]])
    const [op, n] = Array.from(v)
    return table.get(op)(acc, toInt(n))
  }
  const [S] = args
  const [initial, pairs] = [toInt(S[0]), slice(1)(S).match(/../g)]
  return pairs.reduce(f, initial)
}
別解
//  return eval(S)
```

## [数式の計算](https://paiza.jp/works/mondai/string_primer/advance_step9/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const add = (a, b) => a + b
  const sub = (a, b) => a - b
  const f = (acc, v) => {
    const table = new Map([['+', add], ['-', sub]])
    const [op, n] = Array.from(v)
    return table.get(op)(acc, toInt(n))
  }
  const [S] = args
  const [initial, ...rest] = S.match(/[+-]?\d+/g)
  return rest.reduce(f, toInt(initial))
}
```
## [巨大な数の足し算(繰り上がりなし)](https://paiza.jp/works/mondai/string_primer/advance_step10/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [S, T] = args
}
```

## [巨大な数のかけ算](https://paiza.jp/works/mondai/string_primer/advance_step12/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [S, T] = args
}
```