# 眼鏡網站 (Glass Website)

這是一個眼鏡品牌的官方網站，展示眼鏡產品、門市據點及相關服務資訊。

## 專案功能

### 主要頁面
- **首頁** (`index.html`) - 品牌介紹、專業服務特色、聯名鏡框展示
- **光學眼鏡** (`classic-optical.html`) - 光學眼鏡產品展示
- **太陽眼鏡** (`classic-sunglasses.html`) - 太陽眼鏡產品展示  
- **門市據點** (`location.html`) - 門市資訊與地點查詢
- **門市詳情** (`store-page.html`) - 個別門市詳細資訊
- **常見問題** (`faq.html`) - 客戶服務與問題解答
- **部落格** (`blog.html`) - 品牌文章與最新資訊

### 主要特色
- 專業眼鏡服務（單一價格、20分鐘取件、售後保固）
- 多樣化產品系列展示
- 完整門市據點資訊
- 響應式網頁設計

## 技術架構

- **Vite** - 前端建置工具
- **EJS** - 模板引擎
- **SCSS** - CSS 預處理器
- **響應式設計** - 支援不同裝置螢幕

## Node.js 版本
  - 專案的 Node.js 版本需為 v16 以上
  - 查看自己版本指令：`node -v`

## 指令列表
- `npm install` - 初次下載該專案後，需要使用 npm install 來安裝套件
- `npm run dev` - 執行開發模式
  - 若沒有自動開啟瀏覽器，可嘗試手動在瀏覽器上輸入
    `http://localhost:5173/glass_website/pages/index.html`
- `npm run build` - 執行編譯模式（不會開啟瀏覽器）
- `npm run deploy` - 自動化部署

## 資料夾結構
```
glass_website/
├── assets/                 # 靜態資源放置處
│   ├── images/             # 圖片資源
│   └── scss/               # SCSS 樣式檔案
├── layout/                 # EJS 模板放置處
│   ├── header.ejs          # 網站標頭
│   ├── footer.ejs          # 網站頁尾
│   ├── subheader.ejs       # 子標頁
│   ├── city-select.ejs     # 城市選擇器
│   ├── store-select.ejs    # 門市選擇器
│   └── pagelink.ejs        # 頁面連結
├── pages/                  # 網站頁面
│   ├── index.html          # 首頁
│   ├── classic-optical.html     # 光學眼鏡
│   ├── classic-sunglasses.html  # 太陽眼鏡
│   ├── location.html       # 門市據點
│   ├── store-page.html     # 門市詳情
│   ├── faq.html           # 常見問題
│   └── blog.html          # 部落格
├── main.js                 # JavaScript 程式碼
├── package.json           # 專案設定
└── vite.config.js         # Vite 設定檔
```

### 注意事項
- 已將 pages 資料夾內的 index.html 預設為首頁，建議不要任意修改 index.html 的檔案名稱
- .gitignore 檔案是用來忽略掉不該上傳到 GitHub 的檔案（例如 node_modules），請不要移除 .gitignore

## 開發模式的監聽
vite 專案執行開發模式 `npm run dev` 後即會自動監聽，不需要使用 `Live Sass Compiler` 的 `Watch SCSS` 功能

## 部署 gh-pages 流程說明
### Windows 版本
1. 在 GitHub 建立一個新的 Repository

2. 部署前請務必先將原始碼上傳到 GitHub Repository 也就是初始化 GitHub，因此通常第一步驟會在專案終端機輸入以下指令
```cmd
git init # 若已經初始化過就可以不用輸入
git add .
git commit -m 'first commit'
git branch -M main
git remote add origin [GitHub Repositories Url]
git push -u origin main // 僅限第一次輸入，往後只需要輸入 git push
```

3. 初始化完畢後，執行 `npm run deploy` 指令進行自動化部署
