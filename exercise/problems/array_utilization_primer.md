# [配列活用メニュー](https://paiza.jp/works/mondai/array_utilization_primer/problem_index?language_uid=javascript)

## 【配列を参照する操作】全ての要素に対する操作

### [STEP: 1 指定の要素のカウント](https://paiza.jp/works/mondai/array_utilization_primer/array_utilization_primer__count/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const f = a => b => a === b
  const [[N, K], ...rest] = toList(split(' ', toInt))(args)
  return rest.flat().filter(f(K)).length
}
```


### [STEP: 2 全ての要素の和](https://paiza.jp/works/mondai/array_utilization_primer/array_utilization_primer__sum/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const f = (a, b) => a + b
  const [N, ...rest] = toList(toInt)(args)
  return rest.reduce(f)
}
```

### [STEP: 3 配列の最大値](https://paiza.jp/works/mondai/array_utilization_primer/array_utilization_primer__max/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [N, ...rest] = toList(toInt)(args)
  return Math.max(...rest)
}
```

### [STEP: 4 配列の最小値](https://paiza.jp/works/mondai/array_utilization_primer/array_utilization_primer__min?language_uid=javascript)

```js
const fun = (...args) => {
  const [N, ...rest] = toList(toInt)(args)
  return Math.min(...rest)
}
```

### [STEP: 5 指定要素があるかの判定](https://paiza.jp/works/mondai/array_utilization_primer/array_utilization_primer__exist/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, K], ...rest] = toList(split(' ', toInt))(args)
  return rest.flat().includes(K)
    ? 'Yes'
    : 'No'
}
```
### [STEP: 6 指定要素の先頭位置](https://paiza.jp/works/mondai/array_utilization_primer/array_utilization_primer__find/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [[N, K], ...rest] = toList(split(' ', toInt))(args)
  return rest.flat().indexOf(K)
}
```

### [STEP: 7 要素の種類数](https://paiza.jp/works/mondai/array_utilization_primer/array_utilization_primer__kind/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [N, ...rest] = toList(toInt)(args)
  return [...new Set(rest)].length
}
```

## []()
