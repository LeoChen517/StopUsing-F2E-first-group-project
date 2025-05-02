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
## 😎本地第一次存專案Repo
![image](https://hackmd.io/_uploads/HkjBdufegl.png)

👉進入[專案Repo](https://github.com/LeoChen517/F2E-first-group-project) → Open with GitHub Desktop
![image](https://hackmd.io/_uploads/rJ1QtOGgll.png)
👉Clone
![image](https://hackmd.io/_uploads/HyoOYOMexl.png)
👉Open in VScode


    
## ⭐開發流程：
1. 抓遠端最新dev
    ```bash
    git checkout dev
    git pull origin dev
    ```
2. 到[專案Repo](https://github.com/LeoChen517/F2E-first-group-project/issues)認領issue。
![image](https://hackmd.io/_uploads/BkjG5DGlgl.png)
3. Assignees：Assign yourself
4. Development：Create a branch
![image](https://hackmd.io/_uploads/SJtrjwfgge.png)
5. Branch source : dev *(其他選項不變)*
6. Create branch
![image](https://hackmd.io/_uploads/Syq73vMegg.png)
7. 複製到終端機即可開始製作。
8. 製作完成後，執行以下指令提交
*（依據實際修改內容替換 type、summary)*
    ```bash
    git add .
    git commit -m"type: summary"
    git push
    ``` 
9. 到[專案PR](https://github.com/LeoChen517/F2E-first-group-project/pulls)。
![image](https://hackmd.io/_uploads/Hy0f0wGggg.png)
10. Compare & pull request
![image](https://hackmd.io/_uploads/HkM8y_zxeg.png)
11. base : dev
12. Create pull request

## ⭐審核組員PR流程：
1. 到[專案PR](https://github.com/LeoChen517/F2E-first-group-project/pulls)選擇Open中的PR。 
![image](https://hackmd.io/_uploads/r1ijzdGlgl.png)
2. Files changes *(在畫面中上方)*
 ![image](https://hackmd.io/_uploads/r1XMbdMgxe.png)
3. Reviews changes
4. Approve
5. Submit reviews
6. PR合併之後關閉issue、刪除分支。