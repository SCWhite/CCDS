# 標準輸入(stdin)
如果有了一個裝水的容器，卻不能填滿它，那不是很可惜嗎？  
前幾章節我們提到了，一個程式需要有輸入/計算/輸出，我們現在已經能夠順利地宣告變數便將其印出，那緊接著就是把東西塞進變數裡面了。
在輸入的時候，你除了必須了解你輸入的東西是什麼**型態**，例如：10 是整數、3.14 是浮點數及 A 是字元，更要注意的是要用「多大的空間」去儲存。  

## 輸入函式
和輸出一樣，C語言提供了許多輸入的函式供大家使用，包括：
- scanf()
- getc()
- gets()
- read()
其中和 printf() 互相呼應的便是 scanf() 了，下面就來介紹這個輸入函式。  

## scanf
scanf() 的用法和 printf() 有點類似，都是透過格式控制字串來決定要怎麼輸入，舉個例子：

```C++
int num;
double fnum;
char ch;
scanf("%d", &num);
scanf("%lf", &fnum);
scanf("%c", &ch);
```

格式控制字串中帶有 %d ，代表著我要輸入一個整數，並將它存到 num 中。  
接著，讓我們再次複習一下幾個常用的格式控制字元代表的型態吧：

| 格式控制字元 |           型態           |
|:----------:|:-----------------------:|
| %d         | 整數(int)                |
| %lld       | 長整數(long long int)     |
| %u         | 無號整數(unsigned int)    |
| %f         | 單精度浮點數(float)        |
| %lf        | 倍經度浮點數(double)       |
| %Lf        | 長倍經度浮點數(long double)|
| %c         | 字元(char)               |


各位務必注意，在 scanf() 中，**不可以**使用以「\\」開頭的任何格式控制字元，例如：換行「\\n」、Tab「\\t」都不可以出現在 scanf() 中。

## 取址運算子
「&」是一個相當特殊的運算子，它的功能是「取得一個變數的地址」。  
在 scanf() 中，除了要提供要輸入的型態，同時也要指定他要存到哪裡去，但是只指定變數是不夠的，scanf()需要明確知道要寫到「哪裡去」，
因此我們需要加上取址運算子「&」，讓 scanf() 直接將輸入的東西寫到指定位置上。  
關於記憶體控制及相關概念會在之後再詳細講解，現在大家只要知道使用 scanf() 時要加上 & 即可。  

## 練習
請宣告幾個變數依序儲存以下輸入的資料，並以相同方式輸出到螢幕上。  

```C++
A
3.14159
9223372036854775807
```
