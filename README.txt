倉儲管理系統｜專業版（手機安裝版）

【你會得到什麼】
- 可離線使用（PWA）：安裝到手機桌面像 App 一樣開
- 本機資料：紀錄存於瀏覽器 LocalStorage（不會自動同步到別台裝置）

【部署方式 A：最簡單（推薦）— 用 GitHub Pages】
1) 開一個 GitHub 帳號（若已有可略過）
2) 建立新 Repo（例如：warehouse-pro）
3) 把本資料夾內所有檔案上傳到 Repo 根目錄（index.html / sw.js / manifest.webmanifest / icons/…）
4) 到 Repo → Settings → Pages
   - Source: Deploy from a branch
   - Branch: main / (root)
5) 等待 1~2 分鐘後，開啟 Pages 網址
6) iPhone：Safari → 分享 → 加到主畫面
   Android：Chrome → 右上角 → 安裝應用程式 / 加到主畫面

【部署方式 B：本機測試（電腦）】
- 用任一個簡易靜態伺服器開啟（不要用直接點檔案 file://，PWA 會受限）
  例如：Python
  python -m http.server 8080
  然後用瀏覽器打開 http://localhost:8080

【資料搬移（舊版 → 新版）】
- 舊版如果已經有匯出的 JSON：
  新版開啟後 →【匯入（JSON）】→ 選擇檔案即可。
- 若舊版仍在同一台手機、同一瀏覽器且 STORE_KEY 不同：建議先匯出再匯入，避免 localStorage key 不一致導致看不到資料。

【重要提醒】
- 清除瀏覽器資料會清掉本機紀錄；請定期【匯出（JSON）】備份。
