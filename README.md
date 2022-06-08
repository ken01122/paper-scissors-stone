# 應用OpenCV功能完成與AI猜拳功能

### 開發環境
* 使用平台： Visual Studio Code、GitHub
* 使用語言：Python3.9
* 使用套件：OpenCV、MediaPipe、math、random
### 執行方法及步驟
使用Mediapipe手掌偵測，每隻手指有4個節點加上手腕1個共21個節點，再將偵測到的節點座標利用math函式庫，帶入分別計算五隻手指與手掌的餘弦相似度
，取得角度後再根據自訂的角度範圍判斷手指是彎曲還是伸直，如果偵測的角度如果小於50度，表示手指伸直，大於等於50 度表示手指彎曲，
最後回傳手掌每個手指彎曲或伸直所代表的手勢，再去跟電腦所隨機產生的猜拳手勢比對，判斷使用者是贏、輸或是平手。







### 預期成果
先於電腦方使用 Random函式從三個猜拳手勢中隨機選取一個，之後利用Webcam根據使用者手勢偵測出拳內容，偵測完後判斷電腦預先出拳內容決定使用者是贏、輸抑或是平手。

### 參考文獻
Steam教育學習網MediaPipe手勢偵測:https://steam.oxxostudio.tw/category/python/ai/ai-mediapipe-gesture.html

MediaPipe:https://google.github.io/mediapipe/ 
 
Cosine Similarity (餘弦相似度) 的計算方法:https://clay-atlas.com/blog/2020/03/26/cosine-similarity-text-count/


  
 
