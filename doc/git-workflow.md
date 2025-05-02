## 分支與開發規範
1. **`main`**：穩定分支，只有在準備預演時才會合併。
2. **`develop`**：開發分支，所有新功能、bug 修復應該從這裡開始。
3. **`#<num>`**：根據issue number建立的分支，完成後合併到 `develop`。

## 提交規範
Commit message 參考 [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) 規範
- 格式：`<type>: <summary>`
- **type**：變更的類型，應為以下之一：
    ```
    feat：新功能
    fix：修復錯誤
    chore：其他修改，不涉及功能或修復
    docs：文檔修改
    style：代碼風格的變更，不影響功能
    refactor：代碼重構，不涉及功能變更
    perf：性能優化
    test：測試
    ```
- **summary**：簡短描述，說明變更的目的或內容。
- **示例**：
    ```
    feat: add login functionality 
    fix: resolve button color issue
    refactor: simplify login logic 
    perf: reduce login API response time 
    test: add unit test for login API
    ```
## 操作方式參考notion
[link](https://www.notion.so/git-workflow-1e7236e4fb4580b6b61ccf17f61ae168?pvs=4)，
