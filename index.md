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