# PPT Workflow

> 完整 PPT 製作工作鏈 — 從文檔分析到終審拋光，7 階段自動化流程。
> 針對醫學簡報優化，支援中英雙語、Roche Blue 品牌色。

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## 這是什麼？

`ppt-workflow` 是一個給 AI Agent（Hermes、Claude Code 等）使用的 Skill。載入後自動引導你走完 PPT 製作的 7 個階段，每一步都有對應的 AI Skills 支援。

## 7 階段工作鏈

```
📖 Phase 1: 文檔分析 ─→ 提取核心訊息、受眾分析、關鍵數據標記
🏗️ Phase 2: 框架搭建 ─→ 目錄結構、每頁「一句話」、節奏感設計
🎨 Phase 3: 設計系統 ─→ Roche Blue+白底、Inter 字體、圖表配色方案
📝 Phase 4: 內容排版 ─→ 文案撰寫、大字報法則、中英雙語、留白法則
📊 Phase 5: 圖表製作 ─→ infographic、架構圖、流程圖、數據大字報
🎬 Phase 6: 多媒體   ─→ 圖片/影片嵌入、動畫演示、來源引用
✨ Phase 7: 終審拋光 ─→ 一致性檢查、匯出 PDF/PPTX
```

## 特色

- 🎨 **Roche Blue 品牌系統** — 內建 Jeremy 標配配色、字體、排版 Token
- 📊 **圖表自動匹配** — 根據數據類型自動選擇最佳圖表形式（infographic/架構圖/流程圖/大字報）
- 🌐 **中英雙語** — 完整雙語流程，HK 繁體醫學術語強制
- 🏥 **醫學簡報優化** — 流行病學→病理機制→臨床數據→治療對比的經典框架
- 📏 **大字報法則** — 數據視覺化最佳實踐，拒絕純文字頁面
- ✨ **終審自動化** — 一致性檢查、來源引用、格式驗證

## 內建配色方案

| 類型 | 主色 | 適用 |
|------|------|------|
| 醫學/Roche | `#003D6B` | 臨床報告、醫學教育 |
| 健康/養生 | `#83C5BE` | 健康管理、生活方式 |
| 科技/AI | `#3B82F6` | 技術產品、AI 方案 |
| 商業 | `#1A2332` | 商業提案、投資簡報 |

## 調用的 AI Skills

- `article-writing` — 文檔分析與內容提取
- `design-system` / `brandkit` — 設計系統建立
- `design-taste-frontend` / `high-end-visual-design` — 視覺校準
- `copywriting` / `humanizer` / `copy-editing` — 文案優化
- `baoyu-infographic` — 21 種佈局 × 21 種風格的資訊圖表
- `architecture-diagram` — 深色主題架構/流程圖
- `excalidraw` — 手繪風格示意圖
- `dashboard-builder` — 數據儀表板
- `manim-video` — 數學/技術動畫
- `ios-icon-gen` — 圖標生成
- `loop-design-check` — 設計審查迴圈

## 安裝

### Hermes Agent

```bash
git clone https://github.com/jeremychum1030/ppt-workflow.git ~/.hermes/skills/ppt-workflow
```

或在對話中載入：
```
/skill ppt-workflow
```

## 使用方法

| 指令 | 效果 |
|------|------|
| `/skill ppt-workflow` | 啟動工作鏈，顯示當前進度 |
| 「繼續做 PPT」 | 載入當前 Phase Skills |
| 「終審」 | Phase 7 檢查清單 |

## Jeremy PPT 鐵律

- ⚪ **白底絕對** — 深色頁面不可接受
- 🔵 **Roche Blue #003D6B** — 僅頂條 + accent
- 📖 **Inter 字體** — 不用系統默認
- 📊 **圖文並茂** — 拒絕純文字頁面
- 🌐 **中英雙語** — 標題圖表均雙語
- 🏥 **HK 繁體術語** — 發熱/胸痛/體重下降...
- 📏 **留白 40%** — 給眼睛呼吸空間

## License

MIT — 自由使用、修改、分發。

---

*Made with ❤️ by Jeremy Chum*
