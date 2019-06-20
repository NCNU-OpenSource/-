## What-are-you?
+ 使用Mxnet做物體辨識，外加上SSD技術讓辨識可以在一張照片上辨識出多種物品
---
### 什麽是Mxnet？
+ MXNet是一個開源深度學習軟體框架，用於訓練及部署深度神經網路。MXNet具有可延伸性，允許快速模型訓練，
並支援靈活的編程模型和多種程式語言（包括C++、Python、Julia、Matlab、JavaScript、Go、R、Scala、Perl和Wolfram語言）。

### 什麽是SSD?
+ SSD 即 Single Shot Detector
+ 最近一年比较优秀的object detection算法，主要特点在于采用了特征融合。
+ 一种直接预测bounding box的坐标和类别的object detection算法，没有生成proposal的过程
+ 架構圖
<img width="558" alt="ssd" src="https://user-images.githubusercontent.com/35098279/59819988-c4d3cd00-935c-11e9-90a0-b9a67f18e9fc.PNG">

### Demo 
安裝套件
`sudo apt-get install python-opencv python-matplotlib python-numpy`




### 參考資料
+ https://blog.csdn.net/u014380165/article/details/72824889
+ https://blog.csdn.net/u014380165/article/details/78219584
+ https://github.com/zhreshold/mxnet-ssd
