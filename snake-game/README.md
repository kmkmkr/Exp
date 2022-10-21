# snake-game

YOLOを表現学習として使いsnake gameを強化学習で解く

snake-game:https://www.google.com/search?q=snake+game

手順

- ゲーム画面->YOLO->DQN->行動
- ゲーム画面をスクリーンショットでデータを集める（get_data.ipynb)
- ゲーム画面をVOTTでアノテーションし、PascalVOC形式で出力
- PascalVOC形式->YOLO形式に変換（get_data.ipynb)
- YOLOv5を使って学習（<-精度がよくなかったためここで頓挫中
- リアルタイムでゲーム画面を読み取りYOLOの出力結果の物体の位置情報をDQNの入力とし、DQNを学習
- 

YOLO　結果

![image](https://user-images.githubusercontent.com/75050667/197116779-cac56554-5a66-447f-afdc-3166eacacd80.png)

