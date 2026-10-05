# 競賽審查用 GitHub Pages

此資料夾為競賽審查用 GitHub Pages 靜態頁面，不影響原系統。

## 本機預覽

直接以瀏覽器開啟 `index.html` 即可預覽。也可以在此資料夾啟動任意靜態檔案伺服器。

## GitHub Pages 部署

GitHub Pages 的「Deploy from a branch」只能選擇分支的 `/root` 或 `/docs`，無法直接選擇 `competition-page/`。為避免更動既有系統，建議將此資料夾獨立發布到 `gh-pages` 分支：

1. 將本專案內容提交至 GitHub。
2. 在 repository 根目錄執行 `git subtree push --prefix final_demo/competition-page origin gh-pages`；若 `competition-page/` 就位於 repository 根目錄，則將指令中的 prefix 改為 `competition-page`。
3. 進入 Repository **Settings**。
4. 選擇 **Pages**。
5. 在 **Build and deployment** 的 Source 選擇 **Deploy from a branch**。
6. Branch 選擇 `gh-pages`，資料夾選擇 `/ (root)`。
7. 儲存並等待 GitHub Pages 完成部署。

部署後網址通常為：

- 專案頁面：`https://<GitHub 使用者名稱>.github.io/<repository 名稱>/`
- 使用者或組織頁面：`https://<GitHub 使用者名稱>.github.io/`

## 檔案

- `index.html`：展示頁面
- `style.css`：頁面樣式
- `assets/taNeT(3).pdf`：研討會論文
