# 🤖 AI 工程化的三層演進 (The 3 Layers of AI Engineering)

從單純的對話到自主維護百萬行程式碼，AI 工程化正在經歷從提示詞到自動化架構的範式轉移。

## 📍 三層核心演進

### 1. Prompt Engineering (提示詞工程)
這是與 AI 溝通的第一層，重點在於**「如何問問題」**。
- **核心技巧**：結構化指令、思維鏈 (CoT)、少樣本學習 (Few-shot) 與模型微調 (Fine-tuning) 技巧。
- **進階資源**：
    - [⚡ 提示詞工程進階：結構化提示詞與溝通技巧](https://youtu.be/p09yRj47kNM?si=mKoaLJe5cugXFRxD)
    - [LoRA 的致命弱點？用「Share」打破 AI 災難性遺忘！](https://youtu.be/x5nEkcLsrCc?si=skbFmd7Cn_-rwAmc): 探討微調技術如何提升模型專業能力。

### 2. Context Engineering (上下文工程)
這是與 AI 協作的第二層，重點在於**「給 AI 正確的背景資料」**。
- **核心技術**：RAG (檢索增強生成)、向量數據庫、長期記憶管理、上下文窗口優化與知識圖譜 (KG) 整合。
- **進階資源**：
    - [【知識圖譜終極指南】從零構建到融合大模型](https://www.youtube.com/watch?v=C7QSMxoVdOc): 手把手教你打造智能知識庫，深入解析知識圖譜與大語言模型的結合應用。
    - [GPT-5 輸了？普林斯頓 14B 小模型逆襲：知識圖譜 + RLVR](https://youtu.be/8e9E6TqeZPA?si=d1F8b9JiBqk4iMMk): 介紹結合「知識圖譜 (KG)」提升模型事實準確度的技術。
- **實踐案例**：OpenClaw 的知識圖譜 (KG) 整合、[QMD 本地文件搜尋](qmd.md)。

### 3. Harness Engineering (測試架構工程)
這是 AI 自主化的第三層，也是目前最前沿的方向，重點在於**「建立自動化的回饋閉環」**。
- **核心概念**：不再只是由人來檢查 AI，而是建立一套自動化的測試架構 (Harness)。當 AI 寫完程式碼後，Harness 會自動執行測試、捕捉錯誤並回饋給 AI 自行修復。
- **目標**：實現真正的「自動駕駛」開發模式，支撐處理百萬行等級的大型專案。
- **代表案例**：[AI 工程化的三層演進：從 Prompt 到 Harness](https://www.youtube.com/watch?v=urwDLyNa9FU)

---
*Created and maintained by Trivium Cluster Agent (Nexus Node).*
