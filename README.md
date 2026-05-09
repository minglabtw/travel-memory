# 銘旅隨記 · 銘於心 (MING)

> 每一趟旅行，都是一本用腳寫的日記。  
> 在京都吃過的那碗拉麵，在淺草寺前買的御守，在機場匆忙登機前的一杯咖啡⋯⋯  
> 花出去的每一塊錢，都是一段故事的開端。  
>
> **銘旅隨記** 是一個輕量的旅行日記帳本 — 記下花費、拍張照片、寫幾句話。  
> 不囉嗦，不上傳雲端，所有回憶只留在你的手機裡。
>
> 它適合這樣用：
> - 🍜 吃完一碗拉麵 → 拍張照，記下多少錢
> - 🏨 晚上回旅館 → 看看今天花了多少、分類佔比
> - 📤 旅程結束 → 一鍵匯出 Markdown 當作回憶錄
>
> **開發用意：**
> 旅行中的花費不只是數字 — 每一筆都是一段回憶的起點。
> 銘旅隨記的設計很簡單：打開就記，記完就關。不需要帳號、不需要研究功能、不需要擔心資料外洩。把力氣留給旅行，而不是記帳。
>
> 這也是一個「人機協作」的實驗作品 — 從一行 HTML 出發，透過 AI 與開發者的反覆迭代，長成 Android App + PWA。程式碼完全開源，所有資料存在本機，你的旅行回憶只屬於你。

[![PWA](https://img.shields.io/badge/PWA-%E2%9E%A1%EF%B8%8F%20%E9%96%8B%E5%95%9F-orange?style=flat-square)](https://minglabtw.github.io/travel-memory/)
[![Version](https://img.shields.io/badge/version-1.0.0-blue?style=flat-square)](https://github.com/minglabtw/travel-memory/releases)
[![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)](LICENSE)

---

## 📱 快速開始

| 版本 | 使用方式 | 適用對象 |
|------|---------|---------|
| 🌐 **PWA 版** | [點擊開啟](https://minglabtw.github.io/travel-memory/)（瀏覽器直接使用，可加到主畫面） | 任何人（含 iPhone） |
| 📦 **Android APK** | [下載最新版本](https://github.com/minglabtw/travel-memory/releases) | Android 手機（需允許安裝不明來源 App） |

---

## ✨ 功能特色

- **📊 總覽儀表板** — 月度統計、分類圓餅圖、明細表，◀ ▶ 切換月份
- **➕ 快速記帳** — 日期、分類、金額、幣別、評價、隨筆、GPS 地點
- **📷 照片記錄** — 拍照或選相簿，最多 3 張，自動壓縮至約 500KB
- **💰 即時匯率** — 自動抓取最新匯率（open.er-api.com），7 天快取，離線可用
- **📍 GPS 定位** — 自動取得目前位置，或搜尋地標名稱
- **🌙 深色主題** — 一鍵切換，保護眼睛
- **📋 列表分組** — 按日期分組、每日小計、分類篩選
- **📤 完整匯出** — Markdown、JSON 備份（含照片）/還原、CSV（Excel 開啟）
- **🖼️ 照片檢視** — 點擊放大（Lightbox），支援多張
- **🔖 自訂分類** — 可新增、移除自訂分類，自動記憶上次使用
- **⚡ PWA 離線可用** — Service Worker 快取，無網路也可瀏覽

---

## 🛠️ 技術棧

| 技術 | 用途 |
|------|------|
| HTML / CSS / JS | 前端核心（單頁 App） |
| [Capacitor 8](https://capacitorjs.com/) | Android 原生包裝（相機、檔案系統、偏好設定） |
| [IndexedDB](https://developer.mozilla.org/en-US/docs/Web/API/IndexedDB_API) | 本地資料庫（含 localStorage fallback） |
| [Chart.js](https://www.chartjs.org/) | 分類圓餅圖 |
| [Service Worker](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API) | PWA 離線快取 |
| [OpenStreetMap Nominatim](https://nominatim.openstreetmap.org/) | 地標搜尋與反向地理編碼 |

---

## 🏗️ 本地建構

```bash
# 前置需求
# - Node.js + npm
# - JDK 21（JAVA_HOME 指向 jdk@21）
# - Android SDK

# 1. 安裝依賴
npm install

# 2. 同步 Web 資源到 Android
cp index.html www/ && cp manifest.json www/ && cp icon.svg www/
npx cap sync

# 3. Build APK
JAVA_HOME=/opt/homebrew/opt/openjdk@21 ./android/gradlew clean assembleDebug

# APK 產出位置：android/app/build/outputs/apk/debug/app-debug.apk
```

---

## 📄 License

MIT License © 2026 銘旅隨記 · 銘於心 (MING) · 智慧物聯架構實驗室

---

> 用腳步丈量世界，用心記錄每一瞬。
