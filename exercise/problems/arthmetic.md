# [算術・代入演算メニュー](https://paiza.jp/works/mondai/arithmetic_substitution_op/problem_index?language_uid=javascript) 

## [snippet](../../snippet/README.md)


## 累乗 2

### [STEP: 1 足し算](https://paiza.jp/works/mondai/arithmetic_substitution_op/arithmetic_substitution_op__arithmetic_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const N = toInt(args[0])
}
```

### [STEP: 2 引き算・掛け算](https://paiza.jp/works/mondai/arithmetic_substitution_op/arithmetic_substitution_op__arithmetic_step2/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [A, B] = toList(split(' ', toInt))(args[0])
  const D = A - B
  const P =  A * B
  return [D, P]
}

print(join(' '))(fun(...lines))
```

### [STEP: 3 割り算](https://paiza.jp/works/mondai/arithmetic_substitution_op/arithmetic_substitution_op__arithmetic_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [A, B] = split(' ', toInt)(args[0])
  const X = A / B
  const Y = A % B
  return [X, Y]
}

// 入力がないので直接書き換える
const lines = ['437326 9085']

print(join(' '))(fun(...lines))
```

### [STEP: 4 掛け算 2](https://paiza.jp/works/mondai/arithmetic_substitution_op/arithmetic_substitution_op__arithmetic_step4/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [A, B, C] = split(' ', toInt)(args[0])
  const X = A * A
  const Y = B * B + C * C
  return [X, Y]
}
print(join(' '))(fun(...lines))
```

### [STEP: 5 累乗](https://paiza.jp/works/mondai/arithmetic_substitution_op/arithmetic_substitution_op__arithmetic_step5/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [A, B, C] = toList(toInt)(args)
  const N = ((A + B) * C) ** 2
}
// 入力がないので直接書き換える
const lines = ['202', '134', '107']
```

### [FINAL問題 累乗 2](https://paiza.jp/works/mondai/arithmetic_substitution_op/arithmetic_substitution_op__arithmetic_step6/edit?language_uid=javascript)


```js
const fun = (...args) => {
  const [a, b, c, d] = split(' ', toInt)(args[0])
  return ((a + b) * c) ** 2 % d
}

// split(' ', toInt)(args[0])
// split(' ', toInt)('28 57 33 73') -> [28, 57, 33, 73]
// const [a, b, c, d] = [28, 57, 33, 73]
```

## 代入演算

### [代入演算 1 ](https://paiza.jp/works/mondai/arithmetic_substitution_op/arithmetic_substitution_op__substitution_step1/edit?language_uid=javascript)

```js
const fun = (...args) => {
  let  N = toInt(args[0])
  N += 3286
  N *= 4736
  N % = 12312
  return N
}

print(identity)(fun(...lines))
// 入力がないので直接書き換える
const lines = ['0']

// return ((N + 3286) * 4736) % 12312
```

### [代入演算 2](https://paiza.jp/works/mondai/arithmetic_substitution_op/arithmetic_substitution_op__substitution_step2/edit?language_uid=javascript) 

```js
const fun = (...args) => {
  const [A, B, C] = split(' ', toInt)(args[0])
  let N = 0
  N += A
  N *= B
  N %= C
  return N
}
// return (((N + A) * B) % C)
```

### [代入演算 3](https://paiza.jp/works/mondai/arithmetic_substitution_op/arithmetic_substitution_op__substitution_step3/edit?language_uid=javascript)

```js
const fun = (...args) => {
  let N = toInt(args[0])
  N = Math.trunc(N / 361)
  N %= 28
  return N
}

// 入力がないので直接書き換える
const lines = ['10000']
```

### [代入演算 4](https://paiza.jp/works/mondai/arithmetic_substitution_op/arithmetic_substitution_op__substitution_step4/edit?language_uid=javascript)

```js
const fun = (...args) => {
  const [a, b] = split(' ', toInt)(args[0])
  const N = 10000
  return toInt(N / a) % b
}

print(identity)(fun(...lines))

// let N = 10000
// N /= a
// N = toInt(N) % b
// return N

```