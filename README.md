# 🏠 房價儀表板（TWINKLE）

查詢台灣實價登錄成交資料，用列表或地圖瀏覽，並可用自然語言請 AI 幫忙篩選與總結。

**線上使用**：https://kftseng2oo1.github.io/twinkle/

## 主要功能
- 選擇縣市、行政區查詢（台北、新北、台中、高雄等）
- KPI 卡片：成交筆數、平均總價、平均單價（每坪）等
- ☰ 列表／🗺️ 地圖 兩種檢視，可排序與篩選，顯示屋齡
- ⭐ 收藏物件
- **問 AI**：用一句話描述條件（例如「北屯三房 2000 萬內」），AI 轉成篩選條件並總結結果

## 技術與依賴
- 單檔 HTML PWA（`index.html` 內含全部 HTML/CSS/JS），`manifest.json` + `sw.js` 提供安裝到主畫面與離線快取。
- 後端：`twinklehub.kftseng2oo1.workers.dev`（成交資料與 Gemini AI）
- 地圖：Leaflet（cdnjs）
