## 原始方法
* 論文: [Boosting Deep Ensemble Performance with
Hierarchical Pruning](https://ieeexplore.ieee.org/document/9679166)
* 程式碼: [HQ-Ensemble](https://github.com/git-disl/HQ-Ensemble), [EnsembleBench](https://github.com/git-disl/EnsembleBench)

## 改善方法
* 原始方法中各別使用四個指標 `F-CK`, `F-BD`, `F-KW`, `F-GD` 來進行 Hierarchical Pruning 的判斷。而改善後的方法較為嚴謹，以 `F-GD` 作為主要指標，其餘為次要指標，且僅在主要指標中的候選對象也位於所有次要指標中的候選對象時才會進行 Pruning 的動作，其有以下優點:
    1. 由於改善方法較為嚴謹，因此建構出的集成集合能保留到較高準確度的集成
    2. 相較於原始方法只專注於單一高準確度模型所建構出的集成集合，改善方法能在集成集合中保留住較多變的集成以提供更多有用資訊

## 實驗環境
* `Windows 10 or 11`
* `Python 3.10` with `Pytorch` on `CPU`

## 資料集來源
* Mammal45: [Mammals Image Classification Dataset (45 Animals)](https://www.kaggle.com/datasets/asaniczka/mammals-image-classification-dataset-45-animals)

## 程式碼執行
1. 安裝函式庫: `pip install -r requirements.txt`
2. 執行原始方法: `python HQ-Ensemble_mammal.py`
3. 執行改善方法: `python HQ-Ensemble_mammal_enhance.py`

## 組員分配
|  組員  | 工作項目 | 貢獻比例 |
| :----: | :----: | :----: |
| 林均彥 | 原始方法與改善方法實作 | 20% |
| 劉政彥 | 集成中的單元模型訓練 (1) | 20% |
| 金保睿 | 集成中的單元模型訓練 (2) | 20% |
| 張朋楫 | 書面報告撰寫 (1) | 20% |
| 謝尚恆 | 書面報告撰寫 (2) | 20% |