墾丁拍攝行程 APP｜Vercel 快取修正版

這版針對「Vercel 部署預覽已更新，但開啟正式網址仍看到舊畫面」處理：
1. 移除舊 Service Worker 註冊。
2. 第一次打開新版時自動解除舊 Service Worker。
3. 自動清除舊 Cache Storage。
4. vercel.json 對 index.html 設定 no-store / no-cache。
5. 頁面底部有 Build 2026.08.18 字樣，可確認是否為新版。

部署時請把 ZIP 解壓後的所有檔案直接放在專案根目錄。
