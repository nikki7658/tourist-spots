# 台北一日遊推薦

一個純 HTML + CSS 的單頁網頁，介紹台北一日遊的行程、交通方式與小提醒。

線上展示：https://touristspots.pages.dev

## 專案結構

```
touristspots/
├── index.html   # 網頁本體（HTML 與 CSS 都在這一個檔案裡）
├── README.md    # 專案說明
└── .gitignore   # Git 忽略清單
```

## 本機預覽

直接用瀏覽器開啟 `index.html` 即可，不需要安裝任何東西。

## 部署到 Cloudflare Pages（連接 GitHub）

1. 把這個資料夾推到 GitHub 儲存庫
2. 登入 Cloudflare，進入 **Workers & Pages** → **Create application** → **Pages** → **Connect to Git**
3. 選擇剛剛建立的儲存庫
4. 建置設定如下：
   - **Framework preset**：None
   - **Build command**：留空
   - **Build output directory**：`/`（或留空）
5. 按 **Save and Deploy**，完成後會得到 `xxx.pages.dev` 網址

之後只要把更新推送（push）到 GitHub，Cloudflare 就會自動重新部署。

## 內容修改

- 換顏色：修改 `index.html` 中 CSS 的色碼（`#3aafa9`、`#2b7a78`）
- 換景點：複製 `<div class="card">` 區塊，修改時間與文字
- 加圖片：在卡片內加入 `<img src="圖片檔名.jpg" alt="說明">`，並把圖片放在同一個資料夾
