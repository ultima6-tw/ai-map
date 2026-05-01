# ACE Website Project

## 專案目標
ACE（AI Competency Excellence）的公開網站，取代原本的 MkDocs 技術文件網站，改為對非技術研究人員與行政人員友善的多頁式靜態網站。

## 開發機器

- M1 Max Mac Studio 32GB UMA（macOS）— 主力工作機

## 網址
https://ultima6-tw.github.io/ai-map/

## GitHub Repo
https://github.com/ultima6-tw/ai-map

---

## 目前完成狀態（2026-05-01）

### 網站架構
| 檔案 | 說明 |
|------|------|
| `index.html` | 首頁：Hero、三核心、**讓 AI 先認識你**、研究人員與行政人員應用分區 |
| `setup-guide.html` | 讓 AI 先認識你：引導式 Prompt + 複製按鈕（中文）|
| `en/setup-guide.html` | Let AI Know You First（英文版）|
| `courses.html` | 課程：三個工作坊，各拆分為多個章節，YouTube 影片 placeholder |
| `resources.html` | 資源：工具選擇三色卡、APS/ACS 期刊政策比較、外部連結 |
| `about.html` | 關於 ACE：使命、對象、三核心說明 |
| `pillar-foundations.html` | 核心一：AI 基礎與風險管理（LLM 概念、幻覺、情境窗口） |
| `pillar-tools.html` | 核心二：選對 AI 工具（Samsung 事件、工具比較表、判斷原則） |
| `pillar-prompting.html` | 核心三：有效與 AI 互動（五個技巧、研究工作流、範例 prompt） |
| `llm-writing.html` | 研究人員應用：文字處理（潤稿、摘要、翻譯、審稿回覆） |
| `llm-knowledge.html` | 研究人員應用：知識與邏輯（除錯、腦力激盪、跨域概念） |
| `llm-automation.html` | 研究人員應用：自動化流程（批次整理、格式轉換、Python 腳本） |
| `llm-admin.html` | 行政人員應用：公文、會議記錄、信件、公告、報名網站、報表 |
| `assets/css/style.css` | 全站共用 CSS，ACE 配色（Teal #0E7B8C、Navy #1A5276） |
| `assets/img/ace-logo.png` | ACE Logo |

### 部署方式
- GitHub Actions（`.github/workflows/deploy.yml`）
- Push 到 `main` branch 自動觸發，直接上傳 HTML 根目錄
- 不再使用 MkDocs（原有 `docs/zh/`、`docs/en/`、`mkdocs.yml` 保留但不參與部署）

---

## 設計規範

### 配色
| 變數 | 色碼 | 用途 |
|------|------|------|
| `--teal` | `#0E7B8C` | 主色、按鈕、重點 |
| `--navy` | `#1A5276` | 標題、Hero 漸層 |
| `--teal-light` | `#3A9BAB` | Hover 狀態 |
| `--teal-pale` | `#E8F4F6` | 背景淡色 |

### 互動設計
- Prompt 範例：`<details>` 展開收合 + 右上角複製按鈕（複製後顯示「已複製！」2 秒）
- 三核心卡片、LLM 應用卡片：點擊連到對應子頁面

---

## 內容來源
- 原始 `.md` 內容來自 `docs/zh/`（MkDocs 時代）
- 課程章節結構對應 `Projects/AI Literacy/Video1_VO_English_Internal.md`（Video 1 共 46 頁）
- YouTube 連結從原有 `.md` 中篩選，加入各核心頁面的「延伸觀看」區塊

## 更新紀錄
- **2026-04-30**：courses.html + en/courses.html Workshop 1 加入投影片下載列（⬇ 下載 PPTX + 🔍 線上預覽），連結指向 Google Drive（AI_Literacy_Class1.pptx，Google Slides ID: 1TX8-TUDn4y1c7u5x_byfLSDDRGCXEKB0）

## 待辦
- [ ] 課程頁面影片 placeholder → 有 YouTube 連結後換成 iframe embed
- [ ] 核心二（選對工具）延伸觀看影片（目前無適合的 `.md` 來源）
- [ ] about.html 若有聯絡方式可補上
- [x] setup-guide.html 的 YouTube 影片連結（已嵌入 iframe）

## 更新紀錄（續）
- **2026-05-01**：新增 Claude Setup Guide 相關頁面
  - `setup-guide.html` / `en/setup-guide.html`：讓 AI 先認識你，含完整 Prompt + 複製按鈕
  - `index.html` / `en/index.html`：在研究人員/行政人員 section 之前加入 Setup Guide 入口 section
  - `setup-guide.html` / `en/setup-guide.html`：嵌入 YouTube 影片（中：D--Tg7HwnmE / 英：iPmEORni1bs）
  - Prompt 結尾改為通用版：檔名 `my-ai-settings.md`，列出各工具放置位置，移除 Claude 專屬敘述
