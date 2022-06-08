# 應用OpenCV功能完成與AI猜拳功能

### 開發環境
* 使用平台： Visual Studio Code、GitHub
* 使用語言：Python3.9
* 使用套件：OpenCV、MediaPipe、math、random
### 執行方法及步驟
使用Mediapipe手掌偵測，每隻手指有4個節點加上手腕1個共21個節點，再將偵測到的節點座標利用math函式庫帶入計算五隻手指角度的函式計算
，帶入計算五隻手指角度的函式後取得手指角度，再定義另外一個函式，由這個函式判斷角度範圍，如果偵測到手指的角度如果小於50度，
表示手指伸直，大於等於50 度表示手指捲縮，再根據自訂的角度範圍判斷傳入的角度，最後回傳該角度所代表的手勢。


### 預期成果
先於電腦方使用 Random函式從三個猜拳手勢中隨機選取一個，之後利用Webcam根據使用者手勢偵測出拳內容，偵測完後判斷電腦預先出拳內容決定使用者是贏、輸抑或是平手。

### 參考文獻
Steam教育網MediaPipe手勢偵測:https://steam.oxxostudio.tw/category/python/ai/ai-mediapipe-gesture.html

MediaPipe:https://google.github.io/mediapipe/
