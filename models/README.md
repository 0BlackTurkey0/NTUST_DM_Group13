## 單元模型訓練
1. 下載 [Mammal45](https://www.kaggle.com/datasets/asaniczka/mammals-image-classification-dataset-45-animals) 資料集壓縮檔 (mammals.zip)
2. 在 Kaggle 平台中新增以下檔案
    1. 上傳 mammals.zip 並將 Dataset 名稱設定為 `mammal`
    2. 上傳 `test_loader.plk`, `val_loader.plk`, `train_loader.plk` 並將 Dataset 名稱設定為 `usedata`
3. 在 Kaggle 平台中匯入 `mammal_45_classification_final.ipynb`
4. 等待資料建立完成後，將 Accelerator 設定為 GPU ，即可開始進行模型訓練