# JavaScript 入門

## Summary

プログラムの基礎をPaizaを併用して学習します。

## Contents

### 1st day

- Paizaコンテンツとエディタ(vscode)を用いてプログラムで演算をする手法を学習する
- Nodeとvscodeの環境設定を行い，vscode上でプログラムを実行する

#### 学習コンテンツ

- [はじめてのプログラミング](https://paiza.jp/works/javascript/trial/javascript-trial-1/63001)
- [間違いやすいポイント](https://paiza.jp/works/javascript/trial/javascript-trial-1/63002)
- [コメントを書く](https://paiza.jp/works/javascript/trial/javascript-trial-1/63003 )
- [数値を扱う](https://paiza.jp/works/javascript/trial/javascript-trial-1/63004)
- [プログラムで計算する](https://paiza.jp/works/javascript/trial/javascript-trial-1/63005)
- [変数にデータを入れる](https://paiza.jp/works/javascript/trial/javascript-trial-1/63006)
- [データを受け取る](https://paiza.jp/works/javascript/trial/javascript-trial-1/63007)
- [標準入力と標準出力](https://paiza.jp/works/javascript/trial/javascript-trial-1/63008)

#### references

- [環境設定](./docs/environment.md)
- p2 - p15 教科書(JavaScriptモダンプログラミングガイド) 
- p15 - p31 教科書(基礎から学ぶ React/React Hooks)

### 2nd day

- 配列と分割代入, 関数について軽く学ぶ
- Node環境上の外部からのデータ受け取りのプログラムを書いて実行する

#### 学習コンテンツ

- p16 - p28 教科書(JavaScriptモダンプログラミングガイド) 
- p56 - p59, p71 教科書(JavaScriptモダンプログラミングガイド)
- p32 - p35 教科書(基礎から学ぶ React/React Hooks)
- p61 - p61 教科書(基礎から学ぶ React/React Hooks)

#### 演習

- [標準入力メニュー](https://paiza.jp/works/mondai/stdin_primer/problem_index?language_uid=javascript)
- [標準入力サンプル問題セット](https://paiza.jp/works/mondai/stdin/problem_index?language_uid=javascript)

#### 解答例

- [標準入力メニュー・標準入力サンプル問題セット](./exercise/problems/stdin.md)

### 3rd day 

- 標準入力・算術・代入演算の演習を行う
- 関数について学ぶ

#### 学習コンテンツ

- [関数](./docs/function.md)

#### 演習

- [Dランク早解きセット](./exercise/problems/drankfast.problems.md)
- [算術・代入演算メニュー](https://paiza.jp/works/mondai/arithmetic_substitution_op/problem_index?language_uid=javascript)

#### 解答例

- [Dランク早解きセット](./exercise/problems/drankfast.md)
- [算術・代入演算メニュー](./exercise/problems/arthmetic.md)

### 4th day

String(文字列)のプロパティ(フィールド)とメソッド(関数)を学ぶ

#### 学習コンテンツ

- p130 - p135 教科書(JavaScriptモダンプログラミングガイド 第6章 文字列) 
 
#### references

- [String](https://developer.mozilla.org/ja/docs/Web/JavaScript/Reference/Global_Objects/String)

#### 演習

- [CodingBat WarmUP(String)](./codingbatJS/docs/warmup.string.md)
- [文字列処理メニュー](https://paiza.jp/works/mondai/string_primer/problem_index?language_uid=javascript)

#### 解答例

- [CodingBat WarmUP(String)](./codingbatJS/docs/warmup.string.solution.md)
- [文字列処理メニュー](./exercise/problems/string_primer.md)

### 5th - 6th day

配列を学習する，文字列のメソッドと共通している

#### 学習コンテンツ

- p159 - p177 教科書(JavaScriptモダンプログラミングガイド 第7章 配列)
- p47 - p61 教科書(基礎から学ぶ React/React Hooks)
- [JavaScript入門編4: 配列の基礎](https://paiza.jp/works/js/primer/beginner-js4)
 
#### references

- [Array](https://developer.mozilla.org/ja/docs/Web/JavaScript/Reference/Global_Objects/Array)

#### 演習

- [CodingBat WarmUP(Array)](./codingbatJS/docs/warmup.array.md)
- [CodingBat WarmUP(logic)](./codingbatJS/docs/warmup.logic.md)
- [配列メニュー](https://paiza.jp/works/mondai/array_primer/problem_index?language_uid=javascript)
- [配列活用メニュー](https://paiza.jp/works/mondai/array_utilization_primer/problem_index?language_uid=javascript)

#### 解答例

- [CodingBat WarmUP(Array)](./codingbatJS/docs/warmup.array.solution.md)
- [CodingBat WarmUP(logic)](./codingbatJS/docs/warmup.logic.solution.md)


### 7th - 8th day

プログラミングにおける条件分岐を学習しIF文を使ったプログラムを書いて実行する

#### 学習コンテンツ

- p30 - p44 教科書(JavaScriptモダンプログラミングガイド)
- p39 - p42 教科書(基礎から学ぶ React/React Hooks)
- [条件に一致したら処理を実行する](https://paiza.jp/works/javascript/trial/javascript-trial-1/63009)
- [条件に合わせて処理を変える ](https://paiza.jp/works/javascript/trial/javascript-trial-1/63010)
- [数値を分類する](https://paiza.jp/works/javascript/trial/javascript-trial-1/63011)
- [JavaScript入門編2: 条件によって処理を変えてみよう](https://paiza.jp/works/js/primer/beginner-js2)


#### 演習

- [条件分岐メニュー](https://paiza.jp/works/mondai/conditions_branch/problem_index?language_uid=javascript)

#### 解答例

- [条件分岐メニュー](./exercise/problems/conditions_branch.md)

#### references

- なし

### 9th - 10th day

基本的なLoop処理を学習する，JavaScriptは様々なLoop処理があり
for-of文とmap/Array.from関数が後々重要になるので基礎的なLoop文はここでしっかりと抑えておくこと

#### 学習コンテンツ

- [同じ処理を何度も繰り返す](https://paiza.jp/works/javascript/trial/javascript-trial-1/63012)
- [複数のデータを受け取る](https://paiza.jp/works/javascript/trial/javascript-trial-1/63013)
- [複数のデータを分類する](https://paiza.jp/works/javascript/trial/javascript-trial-1/63014)

#### 演習

- [JavaScript入門編3: ループ処理を学ぶ](https://paiza.jp/works/js/primer/beginner-js3)
- [Cランクレベルアップメニュー](https://paiza.jp/works/mondai/c_rank_level_up_problems/problem_index?language_uid=javascript)
- [二重ループメニュー](https://paiza.jp/works/mondai/double_roop_problems/problem_index?language_uid=javascript)


#### references

- p44 - p51 教科書(JavaScriptモダンプログラミングガイド) 
- p42 - p46 教科書(基礎から学ぶ React/React Hooks)


### Challenge

これまで学習したことを活かして演習問題にチャレンジしよう。
これらの演習問題が自力で解けるようになれば，プログラムの基礎はクリアしている。


- [条件分岐メニュー](https://paiza.jp/works/mondai/conditions_branch/problem_index?language_uid=javascript)
- [配列メニュー](https://paiza.jp/works/mondai/array_primer/problem_index?language_uid=javascript)
- [配列活用メニュー](https://paiza.jp/works/mondai/array_utilization_primer/problem_index?language_uid=javascript)
- [二重ループメニュー](https://paiza.jp/works/mondai/double_roop_problems/problem_index?language_uid=javascript)
- [標準出力メニュー](https://paiza.jp/works/mondai/stdout_primer/problem_index?language_uid=javascript)
- [Dランク早解きセット](https://paiza.jp/works/mondai/drankfast/problem_index?language_uid=javascript)
- [Cランクレベルアップメニュー](https://paiza.jp/works/mondai/c_rank_level_up_problems/problem_index?language_uid=javascript)
- [データセット選択メニュー](https://paiza.jp/works/mondai/data_structure/problem_index?language_uid=javascript) 
- [スキルチェック見本問題セット](https://paiza.jp/works/mondai/skillcheck_sample/problem_index?language_uid=javascript)

### 演習解答例

- [条件分岐メニュー](./exercise/problems/conditions_branch.md)
- [二重ループメニュー](./exercise/problems/double_roop_probrems.md)
- [Dランク早解きセット](./exercise/problems/drankfast.md)

