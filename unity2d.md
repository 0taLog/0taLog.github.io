# unity2Dメモ

## Cs
## const(定数)について
+ 書き換えない項目を設定しておくと便利
+ 数値にしておくと処理がしやすいものを設定しておくと便利
+ 数値で扱いたいデータをプログラミング時にはわかりやすい変数名にしておくと便利
+ たとえば、スワイプで変更したい(++)向きなど
例）
~~~
public const int WALL_FRONT = 1; 
public const int WALL_RIGHT = 2; 
public const int WALL_BACK = 3; 
public const int WALL_LEFT = 4; 
~~~
## publicについて
+ ゲームオブジェクトで使いたいものはpublicにしておくといい
+ ソース内でしか使わない関数などはつけなくて voidからでいい
例)
~~~

  //ゲームオブジェクトをタップした時の動作
	public void PushButtonSample(){
		DisplayMessage ("Sample message!");
	}
  
	//ソース内でしか使わない関数
	void ClearMessage (){
  buttonMessage.SetActive (false);	
	}
  
  //ソース内でしか使わない関数
	void DisplayMessage(string mes){
  
  buttonMessage.SetActive (true);
  buttonMessageText.GetComponent<Text> ().text = mes;
  
  }
~~~


## GameObjectについて
+ プログラムで宣言しておくと、unityのインスペクタでいじれるようになる
+ 宣言名はヒエラルキービューのオブジェクトと名前揃えておくと、設定する時わかりいい！
たとえば ボタンA
~~~
public GameObject buttonA;
~~~
UI>Button で作成後 -> 名前変更:ButtonA



## ゲームオブジェクト注意事項
+ クリックして動作させたいものは ボタン で作成(たとえ画像でも)
+ 親と子の属性が違っても・同じでも大丈夫 (親がUI>imageに子をUI>imageでもUI>Buttonで作成しても大丈夫)
### 画像をボタン化したい時
+ 子属性のTextをdeleteして、ButtonにSourceImageを設定する

## プログラム注意事項
## using で読み込むファイル

### UnityEngine
+ デフォルトで大体必要
+ 作成しても何故か書いてないときある(特に設定アイコンのやつGameManager)
~~~
using UnityEngine;
~~~

### UnityEngine.UI
Create>UI>... で作成したゲームオブジェクトをC#で操作する時に必要
~~~
using UnityEngine.UI;
~~~
+ public GameObject 変数名;で書いたのに
+ Inspectorで表示されない時ここがない場合が多い

### System
+ 時間計算のために.NET FrameworkのDateTime,TimeSpanを使う時などに必要
~~~
using System;
~~~
呼び出し
~~~
//宣言
private DateTime sampleDateTime;
//使う時:現在時刻取得
sampleDateTime = DateTime.UtcNow;
~~~

