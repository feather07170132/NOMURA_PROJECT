# Analysis
  > 分析
  
- 根據原始量化＆質化資料，進行處理
- 特徵工程
- 貼label

---
  
### 統計處理
> 了解【野村環球基金 - 台幣累積】基本特性

- Statistics_Analysis：對基金淨值做統計處理
  > TO DO
  >> 1. 加上時間性
  >> 2. more
  
  [👉🏻HERE👈🏻](https://github.com/vanikk06/NOMURA_PROJECT/blob/master/Analysis/Statistics_Analysis.ipynb)
  
  P.S. 博宇也有做一些，在策略的資料夾裡
  
  
### 貼label
> 解決問題：避免觸發低檔買進的頻率過高

- Labeling：以10天漲跌幅的分佈為標準去貼label
  > 取百分比

  [👉🏻HERE👈🏻](https://github.com/vanikk06/NOMURA_PROJECT/blob/master/Analysis/Labeling.ipynb)
  
  - Output Data：[Labeled_Nomura_Global_Equity_Fund.csv](https://github.com/vanikk06/NOMURA_PROJECT/blob/master/Analysis/Labeled_Nomura_Global_Equity_Fund.csv)
 
- nsort：以10天漲跌幅的資料，用半邊的分佈取標準差
  > 標準差
  
  [👉🏻HERE👈🏻](https://github.com/vanikk06/NOMURA_PROJECT/blob/master/Analysis/nsort.py)
  
  - 原始資料：[nomura_global_equity.csv](https://github.com/vanikk06/NOMURA_PROJECT/blob/master/Analysis/nomura_global_equity.csv)
  - 相關code：[Nfunction.py](https://github.com/vanikk06/NOMURA_PROJECT/blob/master/Analysis/Nfunction.py)
  
  - Output Data：[labeled_nomura.csv](https://github.com/vanikk06/NOMURA_PROJECT/blob/master/Analysis/labeled_nomura.csv)

### ML分類器
> 【基金相關】

> 【標的物相關】

- Prediction model：用基金相關的資料丟ML分類器，使用ANN，目前model訓練效果不佳
  > 基金相關

  [👉🏻HERE👈🏻](https://github.com/vanikk06/NOMURA_PROJECT/blob/master/Analysis/Prediction%20model.ipynb)
   
   - 可能原因：
       1. 特徵工程沒做好，matrix不乾淨
       2. 欄位太少
