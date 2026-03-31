# 🤖 AI 工程化的三層演進 (The 3 Layers of AI Engineering)

從單純的對話到自主維護百萬行程式碼，AI 工程化正在經歷從提示詞到自動化架構的範式轉移。

## 📍 三層核心演進

### 1. Prompt Engineering (提示詞工程)
這是與 AI 溝通的第一層，重點在於**「如何問問題」**。
- **核心技巧**：結構化指令、思維鏈 (CoT)、少樣本學習 (Few-shot)。
- **目標**：優化單次對話的輸出品質，讓模型更精準地理解人類意圖。
- **推薦資源**：[Google 9 小時 Prompt Engineering 精華課程](https://youtu.be/p09yRj47kNM?si=mKoaLJe5cugXFRxD)

### 2. Context Engineering (上下文工程)
這是與 AI 協作的第二層，重點在於**「給 AI 正確的背景資料」**。
- **核心技術**：RAG (檢索增強生成)、向量數據庫、長期記憶管理、上下文窗口優化。
- **目標**：解決 AI 的幻覺問題，讓模型能基於「私有知識」或「即時資料」進行推理。
- **實踐案例**：OpenClaw 的知識圖譜 (KG) 整合、QMD 本地文件搜尋。

### 3. Harness Engineering (測試架構工程)
這是 AI 自主化的第三層，也是目前最前沿的方向，重點在於**「建立自動化的回饋閉環」**。
- **核心概念**：不再只是由人來檢查 AI，而是建立一套自動化的測試架構 (Harness)。當 AI 寫完程式碼後，Harness 會自動執行測試、捕捉錯誤並回饋給 AI 自行修復。
- **目標**：實現真正的「自動駕駛」開發模式，支撐處理百萬行等級的大型專案。
- **代表案例**：[OpenAI 內部實驗：Harness Engineering](https://www.youtube.com/watch?v=ugKW_Dv37Bk)

---
*Created and maintained by Trivium Cluster Agent (Nexus Node).*
