# 🚀 AI 資源地圖 (AI Resource Map)

歡迎來到 **AI 資源地圖**。這是一個精心策劃的知識庫，旨在幫助您在快速發展的 AI 領域中導航。

## 🗺️ 視覺路線圖

```mermaid
flowchart LR
    root((AI Map)) --- Basics(基礎 Basics)
    root --- Practical(實戰 Practical)
    root --- Research(科研 Research)
    root --- Trends(趨勢 Trends)

    Basics --- B1[什麼是 LLM?]
    Basics --- B2[AI 幻覺預防]
    Basics --- B3[AI 應用案例]

    Practical --- P1[🖥️ 程式開發]
    Practical --- P2[🎨 影像生成]
    Practical --- P3[🏠 本地模型與隱私]

    Research --- R1[🔍 學術研究工作流]
    Research --- R2[⚡ 提示詞工程進階]
    Research --- R3[🧩 Agent 智能體]
    Research --- R4[📂 QMD 本地知識]

    Trends --- T1[🎓 跨領域學術研究]
    Trends --- T2[最新 AI 新聞]

    click B1 "what-is-ai-or-llm/" "點擊進入 什麼是 LLM?"
    click B2 "ai-hallucination/" "點擊進入 AI 幻覺預防"
    click B3 "ai-application/" "點擊進入 AI 應用案例"
    click P1 "tools-coding/" "點擊進入 🖥️ 程式開發"
    click P2 "tools-image/" "點擊進入 🎨 影像生成"
    click P3 "local-ai-privacy/" "點擊進入 🏠 本地模型與隱私"
    click R1 "research-workflow/" "點擊進入 🔍 學術研究工作流"
    click R2 "advanced-prompting/" "點擊進入 ⚡ 提示詞工程進階"
    click R3 "agent/" "點擊進入 🧩 Agent 智能體"
    click R4 "qmd/" "點擊進入 📂 QMD 本地知識引擎"
    click T1 "academic-trends/" "點擊進入 🎓 跨領域學術研究"
    click T2 "ai-news/" "點擊進入 最新 AI 新聞"
    
    style root fill:#f9f,stroke:#333,stroke-width:2px
    style Basics fill:#bbf,stroke:#333
    style Practical fill:#bfb,stroke:#333
    style Research fill:#fbb,stroke:#333
    style Trends fill:#fdb,stroke:#333
```

## 📂 探索類別

- **[🖥️ 程式開發](tools-coding.md)**: Cursor, GitHub Copilot 與自動化開發代理。
- **[🎨 影像生成](tools-image.md)**: Midjourney, Flux.1 與 Stable Diffusion 實戰。
- **[🏠 本地模型與隱私](local-ai-privacy.md)**: Ollama 與本地算力配置指南。
- **[🔍 學術研究工作流](research-workflow.md)**: **核心推薦**。利用 AI 進行文獻審查與數據分析。
- **[⚡ 提示詞工程進階](advanced-prompting.md)**: 結構化提示詞與模型微調 (LoRA) 技巧。
- **[🎓 跨領域學術研究](academic-trends.md)**: 追蹤 GNoME, AlphaFold 等科學領域的 AI 突破。
- **[🧩 Agent 智能體基礎](agent.md)**: 深入了解 OpenClaw 與代理技能的開發原理。
- **[📂 QMD 本地知識引擎](qmd.md)**: 高效的本地知識庫搜尋與索引工具。

---
*Created and maintained by Trivium Cluster Agent.*
