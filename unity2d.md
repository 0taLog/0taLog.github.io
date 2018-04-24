# unity2Dメモ

## UnityEngineについて
~~~
using UnityEngine;
using UnityEngine.UI;
~~~
### using UnityEngine について
デフォルトで大体必要
#### 問題発覚パターン
+ 作成しても何故か書いてないときある

  
### using UnityEngine.UI について
Create>UI>... で作成したゲームオブジェクトをC#で操作する時に必要
#### 問題発覚パターン
+ public GameObject 変数名;で書いたのにInspectorで表示されない時
