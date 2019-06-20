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
#### Environment
Ubuntu 16.04 (Dual OS with Windows)
GPU： GTX1060 3GB




安裝套件
+ `sudo apt-get install python-opencv python-matplotlib python-numpy`
+ `sudo apt-get install mxnet`
  + 如果你有獨顯
  + `sudo apt-get install mxnet-cu92`
  + https://mxnet.incubator.apache.org/versions/master/install/ubuntu_setup.html#cuda-dependencies
  + 版本要對哦！

+ 下載 pretrained models
  + <a href=https://github.com/zhreshold/mxnet-ssd/releases/download/v0.6/resnet50_ssd_512_voc0712_trainval.zip>pretrained model</a>
  + 解壓縮放在 data/ 裏面
  
+ 執行demo 
  + `python demo.py` (default settings)
  + `python demo.py --images ./data/demo/dog.jpg --thresh 0.5`
  + `python demo.py --cpu --network resnet50 --data-shape 512`

#### Training
+ 


#### 可辨識的物品
+ Aeroplane
+ bicycle
+ bird
+ boat
+ bottle
+ bus
+ car
+ cat
+ chair
+ cow
+ diningtable
+ dog
+ horse
+ motorbike
+ person
+ pottedplant
+ sheep
+ sofa
+ train 
+ tvmonitor







### 參考資料
+ https://blog.csdn.net/u014380165/article/details/72824889
+ https://blog.csdn.net/u014380165/article/details/78219584
+ https://github.com/zhreshold/mxnet-ssd
