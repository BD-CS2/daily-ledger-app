# 日序｜日常記帳

以 Figma「日常記帳 APP P1」為視覺參考的手機優先記帳工具，採用原生 HTML、CSS 與 JavaScript，不需付費 API、付費素材或外部資料庫。

## 功能
- 收入／支出紀錄：金額、消費／進帳項目、分類、日期、帳戶、發票號碼及備註
- 交易管理：月份檢視、類型篩選、關鍵字搜尋、編輯與刪除
- 分類管理：新增、修改及刪除收入／支出分類
- 每月收支統計：收入、支出、結餘、分類占比與排行
- 每月支出預算與理財目標進度追蹤
- CSV 匯入／匯出、JSON 完整備份／還原
- PWA：可安裝至手機主畫面，並提供基本離線快取

## 隱私與資料儲存
所有帳本資料儲存在目前瀏覽器的 `localStorage`，不會傳送到伺服器，也不會與其他使用者共享。不同裝置及不同瀏覽器的資料彼此獨立。清除網站資料或更換裝置前，請先匯出 JSON 備份。

## GitHub Pages 部署
本專案已設定 GitHub Actions 工作流程：`.github/workflows/deploy.yml`。

1. Repository 必須為 Public。
2. 開啟 **Settings → Pages → Build and deployment → Source**，選擇 **GitHub Actions**。
3. 在 **Actions** 頁面確認部署工作流程成功。
4. 網站網址：<https://BD-CS2.github.io/daily-ledger-app/>

之後每次推送至 `main` 分支，都會自動觸發部署。

## 手機安裝
- iPhone：使用 Safari 開啟網站 → 分享 → 加入主畫面。
- Android：使用 Chrome 開啟網站 → 選單 → 安裝應用程式／加入主畫面。

## 版本管理
建議使用清楚的提交訊息，例如：
- `feat: add transaction feature`
- `fix: correct monthly category totals`
- `ui: refine mobile layout`
- `docs: update deployment guide`
