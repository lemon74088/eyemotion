# EyeMotion · 眼球運動與視覺放鬆訓練

單檔 HTML 的互動練習工具，用光點帶動視線移動、定點注視與遠近休息，讓眼睛從近距離工作中退出來。非醫療診斷或治療方案。

## 打開方式

- 直接用瀏覽器開啟 `EyeMotion 眼球運動訓練.html`
- 音樂檔在 `assets/light-piano.mp3`，需與 HTML 放在同一層目錄
- 線上版：<https://4mfsh2uyphqg7.doubao.link/app/app_17hvczckt8p>

## 內容

- 九個模組：水平、垂直、斜向、圓形、折線追蹤，定點注視、目標辨識、遠近休息、眨眼休息
- 四週課表，依權重自動配時並插入短休息
- 課程長度 3–5 分鐘可調（首頁或設定頁）
- 速度 0.6–1.6、目標尺寸 12–34px、提示音、輕音樂、減少動態
- 狀態機：準備 → 倒數 → 進行 → 暫停 → 休息 → 報告
- 訓練紀錄、本週統計、JSON 匯出備份（localStorage，不上傳）

## 技術

- 單檔自包含，原生 HTML/CSS/JS，無建置、無相依套件
- Canvas 2D 繪製訓練視窗，位置由經過時間計算，不受螢幕刷新率影響
- 資料存於 `localStorage`，key `eyemotion.v1`（`file://` 下 IndexedDB 不可靠）

## 音樂

`Satie – Gymnopédie No.1`，Kevin MacLeod 演奏，CC BY 3.0，來源 [incompetech.com](https://incompetech.com/music/royalty-free/index.html?isrc=USUAN1100787)。

## 注意

本工具不提供醫療建議。若練習中出現不適，請停止並休息；不適持續請尋求眼科評估。
