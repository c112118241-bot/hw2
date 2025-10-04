# hw2
```mermaid
graph TD
  A1["1. 研擬計畫 (1d)"]
  A2["2. 任務分配 (4d)"]
  A3["3. 取得硬體 (17d)"]
  A4["4. 程式開發 (70d)"]
  A5["5. 安裝硬體 (10d)"]
  A6["6. 程式測試 (30d)"]
  A7["7. 撰寫使用手冊 (25d)"]
  A8["8. 轉換檔案 (20d)"]
  A9["9. 系統測試 (25d)"]
  A10["10. 使用者訓練 (20d)"]
  A11["11. 使用者測試 (25d)"]

  A1 --> A2
  A1 --> A3
  A2 --> A4
  A3 --> A5
  A4 --> A6
  A5 --> A7
  A5 --> A8
  A6 --> A9
  A7 --> A10
  A8 --> A10
  A9 --> A11
  A10 --> A11

```
```mermaid

gantt
    title 甘特圖
    dateFormat  YYYY-MM-DD
    excludes    weekends

    %% 專案開始日期
    %% 以2025-10-06為起點


    1. 研擬計畫           :done,    t1, 2025-10-06, 1d
    2. 任務分配           :active,  t2, after t1, 4d


    3. 取得硬體           :         t3, after t1, 17d


    4. 程式開發           :         t4, after t2, 70d
    5. 安裝硬體           :         t5, after t3, 10d


    6. 程式測試           :         t6, after t4, 30d
    9. 系統測試           :         t9, after t6, 25d
    11. 使用者測試         :         t11, after t9, 25d


    7. 撰寫使用手冊       :         t7, after t5, 25d
    8. 轉換檔案           :         t8, after t5, 20d
    10. 使用者訓練         :         t10, after t7 t8, 20d

