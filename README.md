# 🏺 浮雲遊子手捏陶學習進度

> 從「器」到「氣」的蛻變 — 一方天地計畫

[![GitHub Pages](https://img.shields.io/badge/Demo-GitHub%20Pages-blue)](https://paullsn93.github.io/Hand-shaped_pottery/)

## 📸 預覽

單頁式應用（SPA），追蹤手捏陶的學習歷程，包含創作維度分析、作品圖庫、尺寸規格表與進階學習資源。

## 🧱 技術架構

| 項目 | 技術 |
|------|------|
| 結構 | 純 HTML5 單檔 SPA |
| 樣式 | Tailwind CSS（CDN） |
| 圖表 | Chart.js（CDN） |
| 字型 | Noto Sans TC / Noto Serif TC（Google Fonts） |
| 部署 | GitHub Pages（`main` branch / root） |

## 📂 檔案結構

```
.
└── index.html    # 所有 HTML、CSS、JS 皆內聯
```

## 🎯 功能區塊

### 1. 四大創作維度探索
- 雷達圖視覺化學習重心分佈
- 點擊維度卡片查看詳細說明
- 維度：造型語言 → 肌理質感 → 空間構成 → 釉色表現

### 2. 一方天地（圖庫）
- 分頁式圖庫：全景主圖 / 茶壺與杯 / 山水茶盤 / 山水屏風 / 茶則配件
- 點擊圖片開啟 Lightbox 大圖檢視
- 席位尺寸與設計邏輯對照表

### 3. 陶藝進階學習資源
經 YouTube oembed API 驗證的教學連結：

| 類型 | 資源 |
|------|------|
| 🎬 影片 | Advanced Pinch Pot Making（David Hughes） |
| 🎬 影片 | Kurinuki Teapot（Blank Earth Ceramics） |
| 🎬 影片 | Kurinuki 杯入門（TA-DAAN） |
| 🎬 影片 | 手捏陶杯（Lolita Olympia） |
| 🌐 網站 | [The Ceramic School](https://ceramic.school) |
| 🌐 網站 | [Ceramic Arts Network](https://ceramicartsnetwork.org) |
| 🎨 頻道 | [Blank Earth Ceramics](https://www.youtube.com/@BlankEarthCeramics/videos) |
| 🔍 搜尋 | YouTube 手捏陶茶壺教學合集 |

### 4. 開學首日啟動方案
- Checklist 形式的行動方案

## 📱 響應式設計

支援手機與桌面瀏覽：
- Header / Main padding 自適應（`py-8 md:py-16`）
- 雷達圖容器高度：手機 280px / 桌面 350px
- 圖庫 min-height：手機 200px / 桌面 400px
- Lightbox 關閉按鈕固定右上角（`z-10`）
- 表格支援水平捲動（`overflow-x-auto`）

## 🚀 本地開發

```bash
# 任意 HTTP 伺服器皆可，例如：
npx -y http-server . -p 8765
# 然後打開 http://127.0.0.1:8765/index.html
```

## 🌐 部署

GitHub Pages 設定：
- **Source**: Deploy from a branch
- **Branch**: `main` / `/ (root)`
- **URL**: https://paullsn93.github.io/Hand-shaped_pottery/

```bash
git add -A
git commit -m "你的 commit message"
git push origin main
# 推送後 GitHub Pages 自動部署
```

## 🎨 設計語言

- **色系**: 陶土色調（`clay-50` ~ `clay-900`）
- **風格**: 毛玻璃面板（`backdrop-filter: blur`）+ 圓角卡片
- **動畫**: 淡入效果（`fadeIn`）、hover 放大（`scale(1.02)`）、emoji bounce

## 📝 更新記錄

- **2026-03-05**: 修正 Doughnut Chart JS 錯誤、更新學習資源連結（oembed 驗證）、響應式設計優化、部署至 GitHub Pages
