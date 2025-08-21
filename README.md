# 眼鏡官方網站 (Glass Website)

一個現代化、響應式的眼鏡電商網站，提供完整的產品展示、門市資訊、客戶服務等功能。

## 📖 專案介紹

這是一個專業的眼鏡品牌官方網站，包含以下主要功能：

### 🏠 首頁
- 品牌形象展示
- 最新產品系列介紹
- 專業服務特色說明
- 聯名設計鏡框展示
- 顧客評價與推薦
- 聯絡表單

### 🕶️ 產品系列
- **OPTICAL** - 光學眼鏡系列
- **SUNGLASSES** - 太陽眼鏡系列  
- **FUNCTIONAL** - 功能性眼鏡系列
- 產品詳細資訊與價格展示
- 分頁瀏覽功能

### 📍 門市據點
- 全台門市位置資訊
- 地區篩選功能
- 門市詳細資訊（電話、營業時間、地址）
- 個別門市詳細頁面

### ❓ 客服支援
- 常見問題 FAQ
- 部落格文章
- 線上客服聯絡

## 🛠️ 技術架構

### 前端技術
- **Vite** - 現代化前端建置工具
- **EJS** - 模板引擎
- **SCSS** - CSS 預處理器
- **響應式設計** - 支援各種裝置螢幕

### 開發工具
- **Live Reload** - 即時重載功能
- **GitHub Pages** - 自動化部署
- **ESLint/Prettier** - 程式碼品質管理

## 🚀 環境需求

### Node.js 版本
- 專案需要 Node.js v16 以上版本
- 查看版本指令：`node -v`

## 📋 指令列表

### 安裝與啟動
```bash
# 安裝相依套件
npm install

# 啟動開發伺服器
npm run dev
# 開發伺服器會在 http://localhost:5173/glass_website/ 啟動
# 首頁位址：http://localhost:5173/glass_website/pages/index.html

# 建置生產版本
npm run build

# 預覽生產版本
npm run preview

# 部署到 GitHub Pages
npm run deploy
```

## 📁 專案結構

```
glass_website/
├── assets/                 # 靜態資源
│   ├── images/             # 圖片資源
│   │   ├── home-*.png      # 首頁相關圖片
│   │   ├── product-*.png   # 產品圖片
│   │   ├── store-*.png     # 門市圖片
│   │   └── ...
│   └── scss/               # 樣式檔案
│       ├── all.scss        # 主要樣式入口
│       ├── base/           # 基礎樣式
│       ├── layout/         # 佈局樣式
│       └── pages/          # 頁面專用樣式
├── layout/                 # EJS 模板
│   ├── header.ejs          # 網站標頭
│   ├── footer.ejs          # 網站頁尾
│   └── ...
├── pages/                  # 網站頁面
│   ├── index.html          # 首頁
│   ├── classic-optical.html    # 光學眼鏡頁面
│   ├── classic-sunglasses.html # 太陽眼鏡頁面
│   ├── location.html       # 門市據點
│   ├── faq.html           # 常見問題
│   ├── blog.html          # 部落格
│   └── store-page.html    # 門市詳細頁面
├── main.js                 # JavaScript 入口檔案
├── vite.config.js         # Vite 設定檔
└── package.json           # 專案設定
```

## 🌐 網站頁面

| 頁面 | 檔案 | 說明 |
|------|------|------|
| 首頁 | `index.html` | 品牌介紹、產品展示、服務特色 |
| 光學眼鏡 | `classic-optical.html` | 光學眼鏡產品目錄 |
| 太陽眼鏡 | `classic-sunglasses.html` | 太陽眼鏡產品目錄 |
| 門市據點 | `location.html` | 全台門市資訊 |
| 門市詳情 | `store-page.html` | 個別門市詳細資訊 |
| 常見問題 | `faq.html` | 客戶常見問題解答 |
| 部落格 | `blog.html` | 品牌文章與資訊 |

## 🎨 設計特色

- **響應式設計** - 適配桌面、平板、手機各種裝置
- **現代化介面** - 簡潔優雅的視覺設計
- **品牌一致性** - 統一的色彩與字型系統
- **使用者體驗** - 直觀的導覽與互動設計

## 📱 響應式支援

網站針對以下裝置進行最佳化：
- 桌面電腦 (1200px+)
- 平板電腦 (768px - 1199px)
- 手機 (576px - 767px)

## 🚀 部署流程

### GitHub Pages 部署
1. 確保專案已推送到 GitHub Repository
2. 執行部署指令：
```bash
npm run deploy
```

### 手動部署流程
```bash
# 1. 初始化 Git (如果尚未初始化)
git init
git add .
git commit -m 'first commit'
git branch -M main
git remote add origin [GitHub Repository URL]
git push -u origin main

# 2. 執行自動化部署
npm run deploy
```

## 📝 開發注意事項

- **首頁重要性**：`pages/index.html` 為預設首頁，建議不要修改檔案名稱
- **熱重載**：開發模式下已啟用自動重載，無需額外設定
- **樣式開發**：使用 SCSS，主入口為 `assets/scss/all.scss`
- **圖片資源**：放置於 `assets/images/` 目錄下
- **模板復用**：共用元件使用 EJS 模板，放置於 `layout/` 目錄

## 🤝 專案維護

此專案為眼鏡品牌官方網站，如需新增功能或修改內容，請遵循現有的程式碼風格和資料夾結構。

## 📞 聯絡資訊

- **客服專線**：0800-000-00
- **服務信箱**：glasses@business.co
- **官方網站**：透過 GitHub Pages 部署

---

© 2024 Glasses. All rights reserved.
