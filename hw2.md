| 任務          | 說明             | 需時(天)    | 前置任務     |
| :-----------: | :---------------:| :----------: | :----------: |
| 1            | 研擬計畫     | 1 | - |
| 2            | 任務分配     | 4    | 1 |
| 3            | 取得硬體     | 17    | 1 |
| 4            | 程式開發     | 70    | 2 |
| 5            | 安裝硬體     | 10    | 3 |
| 6            | 程式測試     | 30    | 4 |
| 7            | 撰寫使用手冊 | 25    | 5 |
| 8            | 轉換檔案     | 20    | 5 |
| 9            | 系統測試     | 25    | 6 |
| 10           | 使用者訓練   | 20    | 7,8 |
| 11           | 使用者測試   | 25    | 9,10 |
***
```mermaid
gantt
    title A Gantt Diagram

    section 任務
    研擬計畫           :a1, 2014-01-01, 1d
    任務分配           :a2, after a1  , 4d
    取得硬體           :a3, after a1  , 17d
    程式開發           :a4, after a3  , 70d
    安裝硬體           :a5, after a3  , 10d
    程式測試           :a6, after a4  , 30d
    撰寫使用手冊       :a7, after a5  , 25d
    轉換檔案           :a8, after a6  , 20d
    系統測試           :a9, after a8  , 25d
    使用者訓練         :a10, after a9  , 20d
    使用者測試         :a11, after a10  , 25d
    section 前置任務
    任務分配    :after a1  , 1d
    取得硬體    :after a1  , 1d
    程式開發    :after a3  , 2d
    安裝硬體    :after a3  , 3d
    程式測試    :after a4  , 4d
    撰寫使用手冊    :after a5  , 5d
    轉換檔案    :after a6  , 5d
    系統測試    :after a8  , 6d
    使用者訓練(1)    :after a9  , 7d
    使用者訓練(2)    :after a9  , 8d
    使用者測試(1)    :after a10  , 9d
    使用者測試(2)    :after a10  , 10d
```
***
![PERT](PERT.jpg)
### 關鍵路徑：
### 1->3->4->6->9->11

