# 銘旅隨記 · 專案結案摘要

> **版本：** v1.0.0 · 2026-05-09  
> **開發模式：** 人機協作（人類需求 + AI 實作）

---

## 專案成果

**銘旅隨記** — 一個輕量的旅行日記帳本，記下花費、拍張照片、寫幾句話。所有資料存在本機，不上傳雲端。

### 兩種使用方式

| 版本 | 網址/位置 | 適用對象 |
|------|----------|---------|
| 🌐 **PWA 版** | https://minglabtw.github.io/travel-memory/ | 任何人，瀏覽器直接可用（含 iPhone） |
| 📦 **Android APK** | Release v1.0.0 下載 | Android 手機，安裝後有完整原生相機 |

### 完整功能

- 記帳（日期、分類、金額、幣別、即時匯率、評價、隨筆）
- 📷 照片（相機/相簿、最多 3 張、自動壓縮、Lightbox）
- 📍 GPS 定位 + 搜尋地標（OpenStreetMap）
- 📊 月度總覽（圓餅圖、分類明細表、日/月統計）
- 📋 列表（按日期分組、每日小計、分類篩選、橫向滑動）
- 📤 匯出（Markdown、JSON 備份含照片、CSV）
- 🌙 深色主題、自訂分類、照片放大檢視

---

## 關鍵指標

| 項目 | 數字 |
|------|:----:|
| 原始碼行數 | ~1735 行（單一 `index.html`） |
| 迭代次數 | 3 次 |
| 踩坑記錄 | 14 個 |
| APK 大小 | 7.9MB |
| GitHub Commits | 10 次 |
| 學習日誌 | 7 頁 MMB |

---

## 檔案位置

| 項目 | 路徑 |
|------|------|
| 專案目錄 | `/Users/yezhiming/網頁實驗品/旅程回憶錄/` |
| GitHub Repo | https://github.com/minglabtw/travel-memory |
| PWA | https://minglabtw.github.io/travel-memory/ |
| APK | `android/app/build/outputs/apk/debug/travel-memory-v1.0.0-debug.apk` |
| RELEASE | https://github.com/minglabtw/travel-memory/releases/tag/v1.0.0 |
| 學習日誌 MMB | `/Users/yezhiming/Documents/技能庫/銘旅隨記-開發日誌/` |
| Opencode Skill | 已安裝於 superpowers/skills/銘旅隨記-開發/ |
| 建構 SOP | `02-建構SOP速查.md` （學習日誌內） |

---

## 給未來的你

這個專案證明了：一行 HTML 透過人機協作迭代，可以在一天內長成 Android App + PWA。

**下次開新作品時：**
1. 直接複製學習日誌的 SOP 結構
2. 載入 Opencode Skill 進入開發狀態
3. 邊做邊記，別等做完才寫

> 用腳步丈量世界，用心記錄每一瞬。
