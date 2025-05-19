# 火災與煙霧辨識

本資料夾包含本專案的模型成果影片及訓練說明。

---

## 結果

![模型展示]([Work accident CNC machine catches fire720p 1, WEFIRE.gif](https://github.com/smalld14/computer-vision-project/blob/main/fire%20smoke/video/Work%20accident%20%20CNC%20machine%20catches%20fire720p%201%2C%20WEFIRE.gif))

---

## 🧠 模型訓練說明

我們使用了以下流程來訓練火災與煙霧辨識模型：

- **模型架構**：`MobileNetV2` / `ResNet50`（視需求可選）
- **訓練資料**：
  - 火災與煙霧圖片：約 2000 張
  - 正常畫面圖片：約 2000 張
  - 資料來源：自建資料集 + 公開資料集（例如 FireNet、FIRESMOKE）
- **預處理方式**：
  - 影像調整尺寸至 224x224
  - 正規化與資料增強（旋轉、亮度調整等）

- **訓練參數**：
  - 批次大小：32
  - 學習率：0.001
  - 訓練輪數（epochs）：30
  - 優化器：Adam

---

## 📁 檔案說明

- `demo.mp4`：模型展示影片
- `README.md`：本說明文件

完整訓練程式與模型參數請參考主目錄的 [`train.py`](../train.py) 或 [`notebooks/`](../notebooks/) 目錄。

---

## 📌 備註

本專案的最終目標是部署至即時攝影機或監控系統，實現早期火災預警。

