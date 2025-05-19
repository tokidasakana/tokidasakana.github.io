<script type="text/x-mathjax-config">MathJax.Hub.Config({tex2jax:{inlineMath:[['\$','\$'],['\\(','\\)']],processEscapes:true},CommonHTML: {matchFontHeight:false}});</script>
<script type="text/javascript" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# C++

## 0. 準備

`a.cpp`というファイルを作成して，次のコードを書く．

```cpp
#include<iostream>
using namespace std;
int main(){
  cout<<"Hello World"<<'\n';
}

```

コンパイルして，実行する．
```bash
$ g++ a.cpp

$ ./a.out
Hello World

$ 
```

エラーが出たら修正する．

## 1. 入出力
入力は`cin`，出力は`cout`で表す．

|変数名|意味|
|----|----|
|`int`|整数|
|`double`|実数|
|`char`|文字|
|`string`|文字列|

### 例

整数 $a,b$ を受け取り， $a+b$ を出力するプログラム

```cpp
#include<iostream>
using namespace std;
int main(){
  int a,b;cin>>a>>b;
  cout<<a+b<<'\n';
}

```

### 練習1.1

整数 $a, b$ を受け取り， $a$ を $b$ で割った商とあまりを"空白区切り"で出力しよう．商は`a / b`，あまりは`a % b`で表す．

- [解説](ans01/01.md)

## 条件式