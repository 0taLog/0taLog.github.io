# C#

## 文法
### 型
+ 
+ 
+ 
+


### 四則演算
~~~
+
-
*
/
%
~~~
#### 変数に代入計算
~~~
hensu = hensu + 1;
hensu += 1;
hensu -= 1;
hensu *= 1;
hensu /= 1;
~~~

#### インクリメント演算子
~~~
hensu++;
hensu--;
~~~

#### 文字・数値の連結（足し算）
~~~
string str1 = "hello";
string str2 = "world";
int num = 123;
string message;

// 文字列＋文字列
message = str1 + str2;
//もしくは
str1 += str2;

//文字列＋数値 = 文字列
srring message = str1 + num; 

~~~

### 条件分岐
#### 注意点
~~~
        int hp = 120;
        if (hp > 100){
            Debug.Log("100以上");
        }else if (hp > 110) {
            Debug.Log("110以上
        }else{
            Debug.Log("そのほか");
        }
~~~
+ 状況の時、先に真になったhp > 100の方の処理が実行される。
+ visual studioだと注意してくれる


## unity C# memo
## debug
#### unity consoleに出力
~~~
Debug.Log(hensu);
~~~

   
