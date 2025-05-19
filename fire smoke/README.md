# 火災與煙霧辨識

介紹
---
使用 YOLOv5 pre-trained model 進行 fine-tune ，再尋找模型最佳化參數。
實務上在廠房內使用火災煙霧辨識，會出現許多造成誤判的情況，像是安全帽、銀色機台、黃色欄杆等，這些物件都有可能造成模型出現誤判。本模型的優勢在於大量收集廠房內的影像，並使用生成式AI軟體在背景上生成更多不同類型的火與煙霧，以及將這些可能要造成誤判的物件排除。

![展示](https://github.com/smalld14/computer-vision-project/blob/main/fire%20smoke/video/Work%20accident%20%20CNC%20machine%20catches%20fire720p%201%2C%20WEFIRE.gif)
![展示](https://github.com/smalld14/computer-vision-project/blob/main/fire%20smoke/video/DosHermanasSevilleSpainJune22022-ezgif.com-video-to-gif-converter.gif)

---

## 模型介紹
- **資料準備**：
  收集工廠產線內火災煙霧的影像，並使用多種資料擴增的方式生成大量、多樣化的資料。
- **Evaluation**：
![image](https://github.com/smalld14/computer-vision-project/blob/main/fire%20smoke/asset/results.png)
 
- **超參數優化**：
 ![image](https://github.com/smalld14/computer-vision-project/blob/main/fire%20smoke/asset/evolve.png)
