# 日語貓戰士｜GitHub-only 版本

這個版本只需要 GitHub Pages，不使用 Firebase、Supabase 或其他後端。

## 可以做到
- N3 單字、文法、測驗、打卡、商店、裝備、花園對決等原本功能
- 同一台裝置開兩個分頁：使用 BroadcastChannel 即時交換對戰分數
- 不同裝置：使用「GitHub-only 同步中心」產生同步碼，再由另一方匯入
- 邀請連結仍可使用，但它只是開啟網站並帶入邀請資訊，不是真正的伺服器房間

## 不能做到
- GitHub Pages 本身不能保存兩台裝置的即時遊戲資料
- 因此不同電腦/手機之間不能像 Firebase 一樣自動即時同步
- 如果要真正的跨裝置即時對戰，仍需要後端資料庫或即時服務

## 部署
1. 建立 GitHub repository。
2. 把 `index.html` 放進 repository。
3. Settings → Pages → Deploy from a branch。
4. 選 `main` / `root`。
5. 開啟 GitHub Pages 網址即可。

## 建議玩法
每天完成學習後：
1. 按「📤 產生我的同步碼」。
2. 把同步碼傳給朋友。
3. 朋友完成自己的學習後，也產生同步碼傳回來。
4. 你按「📥 匯入朋友同步碼」，即可更新鄰居分數。

同步碼是目前遊戲資料的編碼文字，不要公開貼到 GitHub Issues 或公開網站。
