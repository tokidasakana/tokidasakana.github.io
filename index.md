<script type="text/x-mathjax-config">MathJax.Hub.Config({tex2jax:{inlineMath:[['\$','\$'],['\\(','\\)']],processEscapes:true},CommonHTML: {matchFontHeight:false}});</script>
<script type="text/javascript" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML"></script>

# C++

## 準備

`a.cpp`を作成し，次のコードを書く．

```cpp
#include<iostream>
using namespace std;
int main(){
  cout<<"Hello World"<<'\n';
}

```

次にコンパイルして，実行する．

```bash
$ g++ a.cpp

$ ./a.out
Hello World

$ 
```

エラーが出たら，コードを修正する．

## 入出力

入力は`cin`，出力は`cout`で表す．次のコードは文字列 $S$ を受け取り，そのまま出力するコードである．

```cpp
#include<iostream>
using namespace std;
int main(){
  string S;cin>>S;
  cout<<S<<'\n';
}

```

C++で表現される変数は以下の通りである．

|`int`|整数|
|----|----|
|`double`|実数|
|`char`|文字|
|`string`|文字列|

### 1.1

整数 $a,b$ を受け取り， $a+b$ を出力するコードを書こう．

- [解答例](ans01/01.md)