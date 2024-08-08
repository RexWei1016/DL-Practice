# 深度學習模型

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.6%2B-blue.svg)](https://www.python.org/downloads/release/python-360/)
包含兩個 Jupyter Notebook 文件，展示了使用 TensorFlow 和 Keras 的不同深度學習模型
涵蓋的兩個模型分別是卷積神經網絡（CNN）和長短期記憶網絡（LSTM）。

## 目錄

- [深度學習模型](#深度學習模型)
  - [目錄](#目錄)
  - [文件](#文件)
  - [環境需求](#環境需求)
  - [DeepLearning CNN.ipynb](#deeplearning-cnnipynb)
    - [描述](#描述)
    - [主要組成部分](#主要組成部分)
    - [如何運行](#如何運行)
  - [DeepLearning LSTM.ipynb](#deeplearning-lstmipynb)
    - [描述](#描述-1)
    - [主要組成部分](#主要組成部分-1)
    - [如何運行](#如何運行-1)

## 文件

- **DeepLearning CNN.ipynb**：這個 Notebook 使用 MNIST 資料集進行圖像分類的卷積神經網絡（CNN）。
- **DeepLearning LSTM.ipynb**：這個 Notebook 用時間序列預測的長短期記憶網絡（LSTM）。

## 環境需求

要運行這些 Notebook，您需要安裝以下庫：

- TensorFlow
- Keras
- NumPy
- Matplotlib
- Pandas（根據您的資料集格式選擇安裝）

可以使用 pip 安裝這些庫：

```sh
pip install tensorflow keras numpy matplotlib pandas
```

## DeepLearning CNN.ipynb

### 描述

這個 Notebook 實現了一個卷積神經網絡（CNN）來分類來自 MNIST 資料集的圖像。MNIST 資料集包含 60,000 張訓練圖像和 10,000 張測試圖像，這些圖像是手寫的數字（0-9），每張圖像的大小為 28x28 像素。

### 主要組成部分

1. **資料加載**：使用 TensorFlow/Keras 工具加載 MNIST 資料集。
2. **資料預處理**：將圖像像素值標準化到 [0, 1] 範圍。
3. **模型架構**：
   - 卷積層
   - 最大池化層
   - 全連接層
   - Dropout 層
4. **訓練**：使用 Adam 優化器編譯模型並在訓練資料集上進行訓練。
5. **評估**：在測試資料集上評估模型並印出準確率。

### 如何運行

打開 Notebook 並運行所有單元格以訓練和評估 CNN 模型。

## DeepLearning LSTM.ipynb

### 描述

這個 Notebook 實現了一個長短期記憶（LSTM）網絡，用於時間序列預測。LSTM 網絡設計用於處理序列資料，常用於時間序列預測、自然語言處理等任務。

### 主要組成部分

1. **資料加載**：加載時間序列資料集（需要您提供資料集）。
2. **資料預處理**：對資料進行標準化，並創建 LSTM 輸入序列。
3. **模型架構**：
   - LSTM 層
   - 全連接層
4. **訓練**：使用 Adam 優化器編譯模型並在時間序列資料上進行訓練。
5. **評估**：在測試資料集上評估模型性能並印出相關指標。

### 如何運行

打開 Notebook，提供您的時間序列資料集，並運行所有單元格以訓練和評估 LSTM 模型。