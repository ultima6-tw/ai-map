# 🔍 學術研究工作流 (AI-Assisted Research)

AI 不僅能摘要文字，更能輔助「發現隱藏關聯」與「驗證研究假設」。在處理大量學術資源時，選擇正確的技術路徑（RAG 或長上下文）至關重要。

## AI 輔助研究的核心流程

### 1. 問題探索 (Questioning)
- **實際做法**：開啟 [Perplexity AI](https://www.perplexity.ai/)，切換至 **Academic** 模式。輸入：「請列出過去三年內關於 [你的研究主題] 的五篇最具引用價值的論文，並比較它們的實驗方法論。」
- **目的**：快速鎖定研究缺口 (Research Gap)。

### 2. 文獻審查 (Reviewing)
- **實際做法**：將 PDF 上傳至 [Elicit](https://elicit.org/)。使用「Extract data from papers」功能，設定提取欄位為「Sample Size」、「Main Findings」與「Limitations」。
- **目的**：將數十篇文獻自動轉化為可比較的結構化表格。

### 3. 數據分析與視覺化 (Analyzing)
- **實際做法**：將原始實驗數據 (CSV/Excel) 上傳至 ChatGPT (Advanced Data Analysis) 或 Claude。
- **指令範例**：「請分析這份數據的趨勢，繪製相關係數熱圖 (Heatmap)，並找出統計上的異常值。完成後，請針對這些圖表生成一段學術敘述，用於論文的 Results 章節。」
- **目的**：縮短從原始數據到視覺化圖表與文字描述的轉化時間。

### 4. 寫作與校對 (Writing & Proofing)
- **實際做法**：將寫好的草稿段落貼入 Claude 4.6 (King of Logic)。
- **指令範例**：「這是我論文的 Methods 段落，請依據學術論文語氣進行優化。請確保術語正確，修正語法錯誤，並檢查各句子間的邏輯銜接。請保留我的原始數據，僅針對修辭與結構進行調整。」
- **目的**：提升論文的語言專業度，使其符合期刊投稿標準。

---

## 🔬 技術思辨：RAG 還是長上下文 (Long Context)？

隨著模型上下文視窗（Context Window）的擴張（如 Gemini 的 1M+ 或 Llama 4 的 2M+），研究者面臨一個關鍵選擇：我該使用 **RAG (檢索增強生成)** 還是直接把所有論文餵給 **長上下文模型**？

| 比較維度 | RAG (檢索增強生成) | 長上下文 (Long Context) |
| :--- | :--- | :--- |
| **適用場景** | 數萬篇論文的龐大資料庫。 | 10-50 篇核心論文的深度分析。 |
| **成本 (Token)** | 低 (僅檢索相關片段)。 | 高 (每次對話都需讀入全量文本)。 |
| **準確性** | 依賴檢索品質，但能精準定位來源。 | 具備更強的跨段落關聯理解力，但需注意「迷失在中間」現象。 |
| **延遲** | 較快。 | 隨著輸入增加，首字輸出時間 (TTFT) 會變長。 |

### 🎬 推薦資源
- **[YouTube] RAG 與長上下文的對決 - 你到底需要哪一個？**: [點此觀看](https://youtu.be/UabBYexBD4k)
    - 深入分析兩者的優缺點，幫助研究者建立高效的知識檢索策略。

---

## 高階應用: AI 代理 (Agents)

### 多步驟代理 (Multi-step Agents)
- **實際做法**：使用系統如 [GPT Crawler](https://github.com/builderio/gpt-crawler) 或自建 Agent。
- **工作流設定**：
    1. **搜索**：自動在 arXiv 搜尋特定關鍵字。
    2. **過濾**：根據你的摘要關鍵字過濾掉不相關論文。
    3. **總結**：提取每篇論文的核心創新點。
    4. **回報**：將結果自動發送到你的 Discord 或 Notion 頁面。
- **目的**：建立自動化的「情報監控系統」。

## 📺 更多推薦
- **[YouTube] AI Agent 對於工作帶來的衝擊 - 以學術研究為例**: [點此觀看](https://www.youtube.com/watch?v=VqB8zMujdjM)

---
*Created and maintained by Trivium Cluster Agent.*
