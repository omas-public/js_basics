# [VS Code Snippet](./snippet)

## [simple snippet](./simple.snippet.json)

### Install 

- Open Vscode -> File -> user settings -> user snippet -> new global snippet -> paste above link
- Create new javascript file then `simple<Tab>`

code
```js
const readLines = (file = '/dev/stdin') => 
  require('fs').readFileSync(file).toString().trim().split('\n')
const identity = value => value
const join = sep => list => list.join(sep)
const split = (sep, fun = identity) => iter => Array.from(iter.split(sep), fun)
const slice = (begin, end) => iter => end === undefined ? iter.slice(begin) : iter.slice(begin, end)
const toInt = s => parseInt(s, 10)
const toStr = n => n.toString()
const toList = fun => iter => Array.from(iter, fun)
const print = fun => value => console.log(fun(value))

// define your function
const fun = (...args) => {
  // write code here
  return args
}

// if you use stdin or define your array literal
const lines =  readLines('./src/data') 
// use join('\n') or join(' ') or identity in the first parenthesis
print(identity)(fun(...lines))        
```

### function summary

|  function                  |  description                                  |
| -------------------------- | --------------------------------------------- |
| readLines()                | 外部入力を配列にして返す                      |
| identity(value)            | 入力値をそのまま返す                          |
| join(sep)(list)            | 配列をsepで結合する                           |
| split(sep, [fun])(iter)    | イテレータをsepで分割[fun]を適応して返す      |
| slice(begin, [end])(iter)  | イテレータをスライスして返す                  |
| toInt(s)                   | 文字数字を整数に変換                          |
| toStr(n)                   | 数値を文字数字に変換                          |
| toList(fun)(iter)          | イテレータを関数適用し配列を返す              |
| print(fun)(value)          | valueに関数適用し表示する                     |


### example

#### 1行1列の文字列を取り出す ['abc'] -> 'abc'           

data
```js
abc
```

code
```js
const s = args[0] // or const [s] = args 
```

#### 1行1列の数字を取り出す ['1'] -> 1

data
```js
1
```

code
```js
const n = toInt(args[0])
```

#### 空白で区切られた1行複数列の文字列を取り出す ['abc def'] -> 'abc', 'def'

data
```js
abc def
```
code
```js
const [s1, s2] = split(' ')(args[0])
```
#### 空白で区切られた1行複数列の数字を取り出す ['1 2'] -> 1, 2

data
```js
1 2
```
code
```js
const [n1, n2] = split(' ', toInt)(args[0])
```
#### 空白で区切られた1行複数列の数字を先頭と残りに分けて取り出す ['1 2 3 4'] -> 1 [2, 3, 4]

data
```js
1 2 3 4
```
code
```js
const [first, ...rest] = split(' ', toInt)(args[0])
```

#### 複数行の文字列の取得 ['abc', 'def'] -> 'abc', 'def'

data
```js
abc
def
```

code
```js
const [a, b] = args
```

#### 複数行の数字の取得 [123, 456] -> 123, 456

data
```js
123
456
```

code
```js
const [a, b] = toList(toInt)(args)
```

#### 複数行の複数列の文字列の取得 ['ab cd', 'ef gh'] -> [['ab', 'cd'], ['ef', 'gh]]

data
```js
ab cd
ef gh
```

code
```js
const [[ab, cd], [ef, gh]] = toList(split(' '))(args)
// or
const [ab, cd, ef, gh] = toList(split(' '))(args).flat()
```

#### 複数行の複数列の数字の取得 ['12 34', '56 78'] -> [[12, 34], [56, 78]]

data
```js
12 34 
56 78
```

code
```js
const [[ab, cd], [ef, gh]] = toList(split(' ', toInt))(args)
// or
const [ab, cd, ef, gh] = toList(split(' ', toInt))(args).flat()
```

#### 戻り値をそのまま出力

code
```js
print(identity)('abc')
```
output
```js
abc
```

#### 戻り値が複数行(配列)を改行して出力

code
```js
print(join('\n'))([1, 2, 3])
```

output
```js
1
2
3
```
#### 戻り値が複数行(配列)をスペース区切りで出力

code
```js
print(join(' '))([1, 2, 3])
```

output
```js
1 2 3
```

## [paiza snippet](./paiza.snippet.json)

### Install 

- Open Vscode -> File -> user settings -> user snippet -> new global snippet -> paste above link
- Create new javascript file then `paiza<Tab>`

```js
// Global function
const readLines = (file = '/dev/stdin') =>
  require('fs').readFileSync(file).toString().trim().split('\n').map(v => v.trim())

/**
 * identity 入力値をそのまま返す
 * @param {any} value
 * @returns any
 * @example identity(42) -> 42
 */
const identity = value => value

/**
  * split 文字列(s)をセパレータ(sep)で分割した配列を返す
  * @param {string} sep
  * @param {function} fun
  * @paran {string} s
  * @returns Array
  * @example split(' ')('1 2') -> ['1', '2']
  * @example split(' ', toInt)('1 2') -> [1, 2]
  * @example split('\n', toInt)('1\n2') -> [1, 2]
  */
const split = (sep, fun = identity) => s => s.split(sep).map(fun)

/**
  * join 配列(list)を受け取りセパレータ(sep)で結合した文字列を返す
  * @param {string} sep
  * @param {Array<string>} list
  * @returns string
  * @example join(' ')(['a', 'b']) -> 'a b'
  * @example join('\n')(['a', 'b']) -> 'a\nb'
  */
const join = sep => list => list.join(sep)

/**
 * slice iterator(iter)を受け取り引数の範囲をスライスして返す
 * @param {iterator} iter
 * @param {begin} number
 * @param {end} number
 * @returns Array
 * @example slice([0,1,2,3,4,5])(1) => [1,2,3,4,5]
 * @example slice([0,1,2,3,4,5])(-1) => [5]
 * @example slice([0,1,2,3,4,5])(1, 4) => [1,2,3]
 * @example slice([0,1,2,3,4,5])(1, -1) => [1,2,3,4]
 */
const slice = (begin, end) => iter => end === undefined
  ? Array.from(iter).slice(begin)
  : Array.from(iter).slice(begin, end)

/**
  * range 範囲内の数値の配列を返す
  * @param {number} begin
  * @param {number} end
  * @returns Array<any>
  * @example range(10) -> [0,1,2,3,4,5,6,7,8,9]
  * @example range(1, 10) -> [1,2,3,4,5,6,7,8,9]
  */
const range = (begin, end) => {
  const addN = n => m => n + m
  const seq = (num, start) => Array.from(Array(num), addN(start))
  const [num, start] = (end === undefined)
    ? [0, begin]
    : [end - begin, begin]
  return seq(num, start)
}

/**
  * toStr 文字列に変換して返す
  * @param {number} n
  * @returns string
  * @example toStr(3) -> '3'
  */
const toStr = n => n.toString()

/**
  * toInt 文字列を整数に変換して返す
  * @param {string} s
  * @returns number
  * @example toInt('42') -> 42
  * @example toInt('4.2') -> 4
  */
const toInt = s => parseInt(s, 10)

/**
  * toList イテレータ(iter)をfunでList変換する
  * @param {function} fun
  * @param {iterator} iter
  * @returns Array<any>
  * @example toList(toInt)(['1','2','3']) -> [1,2,3]
  * @example toList(toStr)([1,2,3]) -> ['1','2','3']
  * @example toList(split(' '))(['1 2', '3 4']) -> [['1','2'],['3','4']]
  * @example toList(split(' ', toInt))(['1 2', '3 4']) -> [[1,2],[3,4]]
  */
const toList = fun => iter => Array.from(iter, fun)

/**
  * display 値に関数を適用して表示する
  * @param {function} fun
  * @param {any} value
  * @returns undefined
  * @example display(identity)(42) -> console.log(42)
  * @example display(join(' '))([1,2]) -> console.log('1 2')
  * @example display(join('\n'))([1,2]) -> console.log('1\n2')
  */
const display = fun => value => console.log(fun(value))

// define your function

const fun = (...args) => {
  return args[0]
}

// declair your variable

const lines = getLines()

// write maincode with call your function

const result = fun(...lines)

// display function
// use join('\n') or join(' ') or identity in the first parenthesis

display(identity)(result)
```
