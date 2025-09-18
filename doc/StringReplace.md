### 專案配### 題目說明

將 1~100 顯示在畫面上，如果遇到 2 的倍數則顯示"螃蟹"，如果遇到 3 的倍數則顯示"章魚"，如果同時為 2 跟 3 的倍數則顯示"金槍魚"。

### 程式流程圖

```mermaid
flowchart TD
    A[開始] --> B[初始化變數 i = 1]
    B --> C{條件判斷: i <= 100?}
    C -->|是| D{i 是 2 和 3 的倍數嗎？}
    D -->|是| E[輸出 金槍魚]
    D -->|否| F{i 是 2 的倍數嗎？}
    F -->|是| G[輸出 螃蟹]
    F -->|否| H{i 是 3 的倍數嗎？}
    H -->|是| I[輸出 章魚]
    H -->|否| J[輸出 i]
    E --> K[i = i + 1]
    G --> K
    I --> K
    J --> K
    K --> C
    C -->|否| L[迴圈結束]
    L --> M[結束]

    subgraph "For 迴圈"
        B
        C
        D
        E
        F
        G
        H
        I
        J
        K
    end

    %% 樣式設定
    classDef condition fill:#e1f5fe,stroke:#0277bd,stroke-width:2px
    classDef process fill:#f3e5f5,stroke:#7b1fa2,stroke-width:2px
    classDef terminal fill:#e8f5e8,stroke:#2e7d32,stroke-width:2px

    class C,D,F,H condition
    class E,G,I,J,K process
    class A,L,M terminal
```

#### 範例輸出新增專案

- 目標方案名稱: StringReplace
- 專案名稱: StringReplace
- 專案類型: 主控台應用程式(.Net Framework)

### 題目說明

將 1~100 顯示在畫面上，如果遇到 2 的倍數則顯示”螃蟹”，如果遇到 3 的倍數則顯示”章魚”，如果同時為 2 跟 3 的倍數則顯示”金槍魚”。

#### 範例輸出

- 1: 1
- 2: 螃蟹
- 3: 章魚
- 4: 螃蟹
- 5: 5
- 6: 金槍魚
- 7: 7
- 8: 螃蟹
- 9: 章魚
- 10: 螃蟹
- 11: 11
- 12: 金槍魚
- 13: 13
- 14: 螃蟹
- 15: 金槍魚
- 16: 螃蟹
- 17: 17
- 18: 金槍魚
- 19: 19
- 20: 螃蟹
