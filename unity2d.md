# unity2Dメモ

## ゲームオブジェクト注意事項
+ クリックして動作させたいものは ボタン で作成(たとえ画像でも)
+ 親と子の属性が違っても・同じでも大丈夫 (親がUI>imageに子をUI>imageでもUI>Buttonで作成しても大丈夫)
### 画像をボタン化したい時
+ 子属性のTextをdeleteして、ButtonにSourceImageを設定する

## プログラム注意事項
## UnityEngineについて

### using UnityEngine について
~~~
using UnityEngine;
~~~
デフォルトで大体必要
#### 問題発覚パターン
+ 作成しても何故か書いてないときある(特に設定アイコンのやつGameManager)
  
### using UnityEngine.UI について
~~~
using UnityEngine.UI;
~~~
Create>UI>... で作成したゲームオブジェクトをC#で操作する時に必要
#### 問題発覚パターン
+ public GameObject 変数名;で書いたのにInspectorで表示されない時
