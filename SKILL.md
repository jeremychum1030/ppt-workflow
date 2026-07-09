---
name: ppt-workflow
description: PPT 完整製作工作鏈 — 從文檔分析、框架搭建、配色排版、圖表製作到多媒體嵌入。一鍵產出醫學級專業演示文稿。
version: 1.0.0
---

# PPT 製作全流程工作鏈

> `/skill ppt-workflow` → 啟動完整 7 階段 PPT 製作流水線

---

## 7 階段總覽

```
📖 Phase 1: 文檔分析  →  提取核心訊息、受眾分析、關鍵數據標記
🏗️ Phase 2: 框架搭建  →  目錄結構、每頁「一句話」、節奏感設計
🎨 Phase 3: 設計系統  →  Roche Blue+白底、Inter字體、圖表配色
📝 Phase 4: 內容排版  →  文案撰寫、大字報法則、中英雙語、留白
📊 Phase 5: 圖表製作  →  infographic、架構圖、流程圖、數據大字報
🎬 Phase 6: 多媒體    →  圖片/影片嵌入、動畫、來源引用
✨ Phase 7: 終審拋光  →  一致性檢查、匯出 PDF/PPTX
```

---

## Phase 1: 文檔分析

**載入 Skills:** `article-writing`

**三個核心問題:**
```
👤 對象？ 醫生同行 / 患者公眾 / 投資者 / 監管
📋 目的？ 教育 / 報告 / 提案 / 發表
⏱️ 時長？ 5分鐘 / 30分鐘 / 60分鐘
```

**分層提取:**
- 🔴 Must-Know：必須傳達的 3-5 個核心觀點
- 🟡 Should-Know：支撐性數據和證據
- 🟢 Nice-to-Know：補充背景資料

**輸出:** 核心訊息清單 + 關鍵數據表 + 受眾一句話

---

## Phase 2: 框架搭建

**載入 Skills:** `content-strategy`

**醫學簡報框架 (Jeremy 常用):**
```
封面頁 → 目錄 → 流行病學 → 病理機制(流程圖) → 
臨床數據 → 治療對比 → 安全性 → 結論 → Q&A
```

**規則:**
- 每頁只傳達 1 個核心訊息
- 每頁有「一句話 Summary」放在標題
- 頁數 ≈ 演講分鐘數 × 0.5~1

**輸出:** 框架大綱（頁碼 + 每頁一句話）

---

## Phase 3: 設計系統

**載入 Skills:** `design-system` `brandkit` `design-taste-frontend` `high-end-visual-design`

**Jeremy 標配 Token:**
```yaml
主色:   #003D6B (Roche Blue — 僅頂條+accent)
背景:   #FFFFFF (白底鐵律)
卡片:   #F5F7FA / #E8F0F8 (淺灰)
文字:   #1A1A2E (主) / #555555 (輔)
字體:   Inter (標題28pt/正文18pt/註解12pt)
圓角:   12px | 間距: 60px頁邊/24px元素
```

**配色方案:**
| 類型 | 主色 | 輔色 |
|------|------|------|
| 醫學/Roche | #003D6B | #005A8C |
| 健康/養生 | #83C5BE | #6BB5A8 |
| 科技/AI | #3B82F6 | #2563EB |
| 商業 | #1A2332 | #0F172A |

**輸出:** Design Token + 3 張模板頁（封面/內容/結尾）

---

## Phase 4: 內容排版

**載入 Skills:** `copywriting` `humanizer` `copy-editing`

**文字法則:**
- 每頁 ≤ 50 字 / 6 行
- 標題 = 一句話核心訊息（非「介紹XXX」）
- 重點數字大字報處理

**大字報法則:**
```
錯誤: 「研究納入1,247名患者，治療組PFS優於對照組」

正確:
    1,247 名患者
    PFS ↑ 4.2 個月
    p < 0.001
```

**中英雙語:** 標題中英雙語 + 圖表雙語標籤 + HK繁體術語

**60-40 法則:** 60% 內容 + 40% 留白，給眼睛呼吸空間

**輸出:** 所有頁面文案初稿（中英對照）

---

## Phase 5: 圖表製作

**載入 Skills:** `baoyu-infographic` `architecture-diagram` `excalidraw` `dashboard-builder`

**圖表選擇指南:**
| 數據類型 | 圖表 | Skill |
|---------|------|-------|
| 流程/步驟 | 流程圖 | `architecture-diagram` |
| 疾病機制 | 雙路徑對比圖 | `architecture-diagram` |
| 治療對比 | 柱狀圖/森林圖 | `baoyu-infographic` |
| 市場份額 | 餅圖/甜甜圈 | `baoyu-infographic` |
| 時間趨勢 | 折線圖 | `dashboard-builder` |
| 概念關係 | 手繪圖 | `excalidraw` |

**圖表配色:**
```
治療組: #003D6B | 對照組: #94A3B8
正面: #10B981 | 負面: #EF4444 | 中性: #60A5FA
所有圖表: 白底 + 淺灰邊框
```

**輸出:** 所有數據圖表（SVG/PNG）+ 標題+來源

---

## Phase 6: 多媒體嵌入

**載入 Skills:** `ios-icon-gen` `manim-video` `image-to-code`

| 類型 | 適用 | 格式 |
|------|------|------|
| 圖片 | 臨床影像/產品照 | PNG/JPG 300dpi |
| 動畫 | 病理機制/藥物作用 | MP4 (manim-video) |
| 圖標 | 項目符號/分類 | SVG (ios-icon-gen) |

**來源引用:** `Roche MSA Clinical Report 2026` (Inter 10pt, #94A3B8, 右下角)

---

## Phase 7: 終審與拋光

**載入 Skills:** `loop-design-check` `humanizer`

**檢查清單:**
- [ ] 所有頁面白底 (#FFFFFF)
- [ ] Roche Blue 僅 accent，無整頁深色
- [ ] 字體統一 Inter，字級層次一致
- [ ] HK 繁體術語全頁統一
- [ ] 中英雙語對照完整
- [ ] 每頁「一句話」清晰可讀
- [ ] 所有圖表有標題 + 來源
- [ ] 數據前後一致，無錯別字
- [ ] 封面→目錄→內容→結論→Q&A 完整

**匯出:** PDF + PPTX + 備註頁

---

## 使用方法

| 指令 | 效果 |
|------|------|
| `/skill ppt-workflow` | 顯示進度 + 下一步 |
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
