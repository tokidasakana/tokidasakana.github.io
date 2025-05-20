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

整数 $a, b$ を受け取り， $a$ を $b$ で割った商とあまりを"空白区切り"で出力せよ．商は`a / b`，あまりは`a % b`で表す．

- [解説](ans01/01.md)

## 2. 条件式

`if`文を扱う．

### 例

整数 $a,b$ を受け取り， $a+b$ が $0$ 以上なら`Yes`，そうでなければ`No`を出力するプログラム．

```cpp
#include<iostream>
using namespace std;
int main(){
  int a,b;cin>>a>>b;
  if(a+b>=0)cout<<"Yes"<<'\n';
  else cout<<"No"<<'\n';
}

```

### 練習2.1

文字列 $S$ が与えられるので，文字列の長さが5以上ならば`Yes`，そうでなければ`No`を出力せよ．
文字列 $S$ のサイズは`S.size()`で取得できる．

- [解答例1](ans02/01.md)
- [解答例2](ans02/02.md)

### 練習2.2(応用)

整数 $N$ がうるう年か判定せよ．

- ヒント： $N$ が $4$ の倍数である上， $N$ が $100$ の倍数でないか， $N$ が $400$ の倍数であればうるう年である．
- [解答例](ans02/03.md)

## 3. 繰り返し
`for`文を扱う．

### 例

与えられた整数 $x$ に対して， $x+0,x+1,...,x+9$ を出力するプログラム．
このプログラムの場合， $i$ は $0$ から $9$ まで動く．

```cpp
#include<iostream>
using namespace std;
int main(){
  int x;cin>>x;
  for (int i=0;i<10;i++)cout<<x+i<<" \n"[i+1==10];
}

```

最後の`" \n"[i+1==10]`は`[]`内の条件式を満たさない間は空白，満たすと改行となる．

### 練習3.1

整数 $N$ と文字列 $S$ が与えられるので，改行区切りで $N$ 回 $S$ を出力せよ．

- [解答例](ans03/01.md)

## 4. 繰り返し2

`while`文を扱う．

### 例

与えられた整数 $x$ に対し， $x+1,x+2,...,10$ を出力する．

```cpp
#include<iostream>
using namespace std;
int main(){
  int x;cin>>x;
  while(x++<10)cout<<x<<'\n';
}

```

### 練習4.1

整数 $N$ が与えられるので， $2^N$ を出力せよ．
ただし， $N \leq 30$ で試すこと(プログラムが正しく動作しない場合がある)．

- ヒント: $a=1$ とし， $a$ に $2$ を $N$ 回かければよい．
- [解答例1](ans04/01.md)
- [解答例2](ans04/02.md)