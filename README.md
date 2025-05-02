# Project Name 
xxx

## 簡介
這是我們的 side-project，目的是練習並應用前端與後端技術來構建一個實用的應用。

## 開發環境
- Node.js 版本：`v14.x.x`  # 用於執行 JavaScript 伺服器端代碼
- Vite 版本：`2.x.x`  # 用於快速構建和開發 React 或 Vue 應用

## 框架
- React 版本：`17.x.x` 
- Vue 版本：`3.x.x`
- Tailwind CSS 版本：`2.x.x`  # CSS 框架
- Bootstrap 版本：`5.x.x`  # UI 框架

## 安裝步驟
1. 克隆這個專案：
    ```bash
    git clone https://github.com/mmaysu/F2E-sideproject.git
    ```
2. 進入專案資料夾：
    ```bash
    cd F2E-sideproject
    ```
3. 安裝依賴：
    ```bash
    npm install
    ```
4. 開始開發：
    ```bash
    npm run dev
    ```

## 拉取最新代碼
1. 確保當前分支是你想要更新的分支（通常是 `develop` 或你自己開發的功能分支）：
    ```bash
    git checkout develop
    ```
2. 拉取遠端倉庫的最新更改：
    ```bash
    git pull origin develop
    ```
3. 安裝任何新的依賴（如果 `package.json` 發生變更）：
    ```bash
    npm install
    ```
4. 如果你在拉取代碼後發現合併衝突，解決衝突後再次提交。

## 分支與開發規範
1. **`main`**：穩定分支，只有經過測試並且確保能部署的代碼才會合併。
2. **`develop`**：開發分支，所有新功能、bug 修復應該從這裡開始。
3. **`feature/功能名稱`**：開發新功能的分支，完成後合併到 `develop`。
4. **`bugfix/bug名稱`**：修復 bug 的分支，完成後合併回 `develop`。
5. **`hotfix/修補名稱`**：緊急修復分支，直接從 `main` 切出，完成後合併回 `main` 和 `develop`。

## 提交規範
Commit message 使用 [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) 規範
- 格式：`<type>(<scope>): <summary>`
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
- **scope**：表示變更所涉及的範圍
  - 功能模塊：
  ```
    auth: 認證相關的功能（例如，登入、註冊功能）。
    ui: 用戶界面相關的變更（例如，按鈕樣式、頁面布局）。
    api: API 相關的變更（例如，新增或修改 API 端點）。
    database: 資料庫相關的變更（例如，新增資料表或字段）。
    security: 安全性相關的修改（例如，密碼加密、漏洞修復）。
  ```
  - 範疇相關：
  ```
    frontend: 前端部分的改動。
    backend: 後端部分的改動。
    devops: CI/CD 相關的變更（例如，部署腳本、服務器配置）。
    testing: 測試相關的變更（例如，新增測試案例、修改測試邏輯）。
    build: 構建相關的變更（例如，修改打包配置、升級打包工具）。
  ```
  - 其他具體範疇：
  ```
    docs: 文檔相關的改動（例如，更新 README）。
    style: 代碼風格相關的變更（例如，格式化代碼、調整縮排）。
    chore: 其他雜項工作（例如，更新依賴包、修改配置文件）。
    config: 配置相關的變更（例如，修改配置文件，添加環境變數）。
    migration: 資料庫遷移或數據結構改動。
  ```
- **summary**：簡短描述，說明變更的目的或內容。
#### 示例：
```
feat(auth): add login functionality 
fix(button): resolve button color issue
refactor(auth): simplify login logic 
perf(auth): reduce login API response time 
test(auth): add unit test for login API
```

## 如何進行 Pull Request：
1. 創建一個新的 feature 分支(例如：新增一個登入頁面)。
    ```bash
    git checkout -b feature/add-login-page
    git add login.html
    git commit -m "feat(login): add login page HTML"
    git push origin feature/add-login-page
    ```
2. 開發完成後，提交 PR 到 `develop` 分支。
![image](https://hackmd.io/_uploads/SJghoW-leg.png)
3. 在 PR 中標註審核人員，並記得寫清楚變更的內容。
4. PR 確認後，合併到 `develop` 分支。
5. 本地更新develop
    ```bash
    git checkout develop
    git pull origin develop
    ```
