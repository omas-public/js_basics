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
  const [[S], ij] = toList(sprit(' '))(args)
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
```