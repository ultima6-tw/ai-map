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

## 目前完成狀態（2026-05-14）

### 網站架構
| 檔案 | 說明 |
|------|------|
| `index.html` | 首頁：Hero、三核心、**讓 AI 先認識你**、研究人員與行政人員應用分區 |
| `setup-guide.html` | 讓 AI 先認識你：引導式 Prompt + 複製按鈕（中文）|
| `en/setup-guide.html` | Let AI Know You First（英文版）|
| `coding-prompt.html` | 設定你的 AI 程式助手：訪談式 Prompt + 複製按鈕（中文）|
| `en/coding-prompt.html` | Set Up Your AI Coding Assistant（英文版）|
| `courses.html` | 課程：三個工作坊，各拆分為多個章節，ep01–07 + ep08 全部嵌入 |
| `resources.html` | Claude.ai 操作介紹：Cowork（3 影片）、Code（5 影片）、Design（2 影片）|
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
- **2026-09-08**：index.html「研究人員」section 原本 4 張卡片改為 3 支陶哲軒談 AI×數學/科學研究影片清單（resource-link 樣式，各附一句話內容簡介），4 個子頁面入口改成一行純文字連結（詳見 NOTES.md「首頁『研究人員』影片清單」）。en/index.html 已同步（標題/簡介翻譯成英文，人名譯為 Terence Tao、頻道名保留原文，語言標示 Chinese，比照 pillar-foundations.html 既有慣例）。
- **2026-05-14**：resources.html / en/resources.html 頁面副標題縮短為單行（ZH：「Claude Cowork、Code 與 Design 使用指南，含操作示範影片。」EN：「Claude Cowork, Code & Design — hands-on demo videos.」）
- **2026-05-14**：resources.html / en/resources.html 新增 Claude Design 節區（第三節），含官方連結（claude.ai/design）與兩支英文影片（t_LBECIQQqs Anthropic官方、X7YMMyd2Qnk Tristen O'Brien基礎教學）
- **2026-05-13**：resources.html / en/resources.html Code 區新增三支示波器/硬體控制影片（9oMwjWW3wsg Keysight示波器、A4H2UyeRx9w Lecroy示波器、nmGEedloQ6E ESP32自動化測試台），共五支影片
- **2026-05-14**：resources.html / en/resources.html 全部影片加語言標示（🎬 影片語言：中文/英文）；EN 頁中文影片描述翻譯成英文
- **2026-05-13**：resources.html / en/resources.html Code 兩支影片描述全面更新（分析 YouTube 說明，改為具體 demo 內容）
- **2026-05-13**：resources.html / en/resources.html Cowork 三支影片描述全面更新（逐一分析 YouTube 章節，改為列出每支影片的實際 demo 範例，方便讀者選片）
- **2026-05-13**：resources.html / en/resources.html Cowork 區新增第三支影片（227K1Vy82ag，「10分鐘精通 Claude Cowork 全自動辦公」）
- **2026-05-13**：網站結構重組（第三輪）
  - `resources.html` / `en/resources.html`：影片改為「一影片一行、影片左描述右」版型；說明文字改為清單格式（`<ul><li>`）；連結順序：h2 → Ep08 → 官方說明（Ep08 直接放在主標題正下方，官方說明緊接其後，合併為一個 flex 容器）
- **2026-05-13**：網站結構重組（第二輪）
  - `courses.html` / `en/courses.html`：Workshop 3 底部加入各廠商工具連結（ChatGPT / Gemini / Claude / Copilot）
  - `resources.html` / `en/resources.html`：頁面標題改為「Claude.ai 操作介紹」（nav 仍顯示「資源」）；移除實用連結 section
- **2026-05-13**：網站結構重組（第一輪）
  - `resources.html` / `en/resources.html`：改為 Claude Cowork + Code 使用指南，含四支示範影片（Cowork ZH/EN、Arduino、RPi）；移除三色卡與期刊政策
  - `index.html` / `en/index.html`：三核心方向下方新增「工具安全性」三色卡（安全/謹慎/避免）
  - `llm-writing.html` / `en/llm-writing.html`：新增 APS/ACS 期刊 AI 政策 section（原在 resources.html）
- **2026-05-11**：YouTube 標題全面統一（ep01–07）：ZH 格式 `{主題} | AI 素養系列 Ep.XX`、EN 格式 `{Topic} | AI Literacy Series Ep.XX`；同步修正 courses.html ZH iframe title 屬性中的全形分隔符號與不一致後綴
- **2026-05-11**：courses.html + en/courses.html Ch 2-2 換為 ep07 YouTube embed（ZH: ppNN74zWJVw，EN: 3CgTsibYXl8）
- **2026-05-11**：courses.html + en/courses.html Ch 2-1 換為 ep06 YouTube embed（ZH: PQZI8DjOfHo，EN: o6cMfp8ogBA）
- **2026-05-11**：courses.html + en/courses.html Ch 1-5 換為 ep05 YouTube embed（ZH: ZE5Eue5NzzE，EN: WRvNKtdNTc8）
- **2026-05-11**：courses.html + en/courses.html Ch 1-4 換為 ep04 YouTube embed（ZH: 9M1PNym-cOo，EN: ZcVWLmrPpzM）
- **2026-05-11**：courses.html + en/courses.html Ch 1-3 換為 ep03 YouTube embed（ZH: g1MgyRCgoOg，EN: q6HobCWNybY）
- **2026-05-11**：courses.html + en/courses.html Ch 1-2 換為 ep02 YouTube embed（ZH: dUQYxRhe5aA，EN: LS4jeJLy-5M）
- **2026-05-11**：en/courses.html Workshop 2 加入 Vibe Coding 延伸觀看（Extended Viewing，fHWFF_pnqDk）
- **2026-05-13**：Workshop 3 ZH embed 更新為修正版（1nO6gG9xx2g，舊版 3e0ZrzUewrc 因 sample rate 問題刪除）
- **2026-05-13**：courses.html + en/courses.html Workshop 3 改為三章結構，各對應不同客群，並以 YouTube 時間戳直接跳到對應章節（ZH: ?start=339 / ?start=853；EN: ?start=378 / ?start=1003）
- **2026-05-12**：courses.html + en/courses.html 新增 Workshop 3「AI Agent 時代：從概念到工具」，嵌入 EP08（ZH: 3e0ZrzUewrc，EN: Vapyq4WwjvQ）
- **2026-05-11**：en/courses.html 同步對齊 7 集影片系列（同中文版），ep01 EN iframe 換為新版（g58MKUTCeAA），Workshop 3 移除
- **2026-05-11**：courses.html 章節結構對齊 7 集影片系列：各章標題/描述改為對應各 ep 實際內容（ep01–07），Workshop 3 移除（內容已含在 ep07/Workshop 2 Ch 2），Workshop 2 標題改為「提示技巧與安全使用」；ep01 ZH iframe 換為新版（er_vunAQ8VE）
- **2026-05-07**：新增 coding-prompt.html / en/coding-prompt.html；首頁研究人員與行政人員 section 各加入 coding prompt 卡片（中英文）
- **2026-04-30**：courses.html + en/courses.html Workshop 1 加入投影片下載列（⬇ 下載 PPTX + 🔍 線上預覽），連結指向 Google Drive（AI_Literacy_Class1.pptx，Google Slides ID: 1TX8-TUDn4y1c7u5x_byfLSDDRGCXEKB0）

## 待辦
- [x] 課程頁面影片 placeholder → 全部換成 iframe embed（ep01–07，2026-05-11 完成）
- [x] llm-writing.html 4 個 prompt 改為引導式
- [x] llm-knowledge.html 3 個 prompt 改為引導式
- [x] llm-automation.html 3 個 prompt 改為引導式（Claude Code Demo 保留原格式）
- [x] llm-admin.html 6 個 prompt 改為引導式
- [x] en/ 四個頁面同步改為引導式英文版（共 16 個 prompt）
- 決策：所有 prompt 改為引導式（AI 主動問問題），使用者丟進去即可，不需要自己填空
- [ ] 核心二（選對工具）延伸觀看影片（目前無適合的 `.md` 來源）
- [ ] about.html 若有聯絡方式可補上
- [x] setup-guide.html 的 YouTube 影片連結（已嵌入 iframe）
- [x] en/index.html 同步「研究人員」影片清單（2026-09-08 完成，標題/簡介譯成英文，語言標示 Chinese）

## 更新紀錄（續）
- **2026-05-07**：setup-guide.html / en/setup-guide.html 更新為 v2 prompt（AI Initial Setup Prompt）
  - Prompt 從 14 題縮為 10 題，移除抽象個性題，新增技術背景題（Q5）
  - 各題加入引導例子，降低非技術使用者回答門檻
  - 輸出改為固定英文，輸出結構更新（新增 Tech Background & Tools，移除 Personality & Collaboration）
  - 加入 AI 自我識別指令（只顯示當前工具的安裝說明）
  - 步驟說明中 `claude-tmp.md` 改為 `my-ai-settings.md`
- **2026-05-01**：新增 Claude Setup Guide 相關頁面
  - `setup-guide.html` / `en/setup-guide.html`：讓 AI 先認識你，含完整 Prompt + 複製按鈕
  - `index.html` / `en/index.html`：在研究人員/行政人員 section 之前加入 Setup Guide 入口 section
  - `setup-guide.html` / `en/setup-guide.html`：嵌入 YouTube 影片（中：D--Tg7HwnmE / 英：iPmEORni1bs）
  - Prompt 結尾改為通用版：檔名 `my-ai-settings.md`，列出各工具放置位置，移除 Claude 專屬敘述
