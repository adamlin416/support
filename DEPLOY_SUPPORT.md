# 如何發布支援頁面 (Support Page)

您已經在 `/Users/adam/Documents/Code/support` 建立了支援頁面的原始檔案。
請依照以下步驟將其發布到 GitHub：

## 方法一：建立獨立的 `support` Repo (推薦)
這樣您的網址會是 `https://adamlin416.github.io/support`。

1. **在 GitHub 上建立新 Repo**
   - 前往 [GitHub Create Repo](https://github.com/new)
   - Repository name 輸入: `support`
   - **Public** (公開)
   - 點擊 "Create repository"

2. **上傳程式碼**
   開啟終端機 (Terminal) 並執行以下指令：

   ```bash
   cd /Users/adam/Documents/Code/support
   git add .
   git commit -m "Initial support page"
   git branch -M main
   # 將下方網址換成您剛剛建立的 repo 網址
   git remote add origin https://github.com/adamlin416/support.git
   git push -u origin main
   ```

3. **開啟 GitHub Pages**
   - 回到 GitHub 上的 `support` repo 頁面。
   - 點擊 **Settings** (設定) > 左側選單 **Pages**。
   - 在 **Build and deployment** 下的 **Source** 選擇 `Deploy from a branch`。
   - 在 **Branch** 選擇 `main`，資料夾選擇 `/(root)`，然後點擊 **Save**。

4. **完成**
   - 等待約 1-2 分鐘。
   - 您的支援頁面將會在：`https://adamlin416.github.io/support`
   - 隱私權政策頁面在：`https://adamlin416.github.io/support/privacy.html`

## 修改聯絡信箱
請打開 `index.html`，搜尋 `mailto:support@example.com` 並將其更改為您真實的信箱。
