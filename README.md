# SportPress 體育新聞產稿系統

體育新聞自動產稿平台，整合 Google Sheet、Perplexity、Claude AI，可一鍵發布到 Threads、Facebook、Instagram。

## 功能特色

- 🏀 支援棒球（投手/野手）、籃球數據
- 🤖 AI 自動產生正式體育新聞稿
- 🔍 Perplexity 搜尋最新相關新聞
- 📱 一鍵發布到 Threads / FB / IG
- 👥 支援 50 個獨立帳號

## 線上使用

👉 [點此開啟系統](https://你的帳號.github.io/sportpress/)

## 測試帳號

| 帳號 | 密碼 |
|------|------|
| reporter01 | sp2025r01 |
| reporter02 | sp2025r02 |
| ... | ... |
| reporter50 | sp2025r50 |
| admin | admin2025! |

> 密碼規則：`sp2025r` + 編號

## 技術架構

```
前端網頁 (GitHub Pages)
    │
    ▼
Make.com Webhook
    │
    ├── Google Sheet（資料庫）
    ├── Perplexity API（搜新聞）
    ├── Claude API（產生新聞稿）
    └── Meta API（發布社群）
```

## 設定說明

1. 部署網頁到 GitHub Pages
2. 在 Make.com 建立 Webhook
3. 進入系統設定頁面，填入 Webhook URL
4. 開始使用！

## 檔案說明

- `index.html` - 主要網頁應用程式
- `accounts.csv` - 帳號清單（可匯入 Google Sheet）
