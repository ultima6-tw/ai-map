# AI 幻覺、造假與安全 (Integrity & Security)

識別 AI 在學術研究與數據生成中可能出現的錯誤、系統性偽造，以及保護 AI 系統免受惡意攻擊。

## 🔍 學術與數據造假 (Hallucinations)

- **[哈佛教授讓 AI 寫物理論文，兩週完成但抓到系統性造假](https://www.youtube.com/watch?v=FPOIL0W-w1M)**
    - 警示案例：AI 雖然能快速產出內容，但在缺乏監督下可能編造實驗數據。
- **[Vibe physics: The AI grad student | Anthropic](https://www.anthropic.com/research/vibe-physics)**
    - Anthropic 研究 AI 在物理領域的表現，探討其「直覺物理」與真實科學邏輯之間的差距。

---

## 🛡️ AI 系統安全性 (AI Security)

隨著 LLM 整合進更多軟體系統，針對 AI 的攻擊手段也隨之演進。了解這些風險是建立安全工作流的第一步。

### 核心風險：提示詞注入 (Prompt Injection)
當攻擊者透過巧妙設計的輸入，繞過 AI 的安全限制或「劫持」其指令時，就發生了提示詞注入。

- **[什麼是提示詞注入 (Prompt Injection)？](https://www.youtube.com/watch?v=gUNXZMcd2jU)**
    - **推薦必看**：由 **Computerphile** 製作的深度解析。深入探討為何 AI 難以區分「使用者的資料」與「系統的指令」，以及這種模糊邊界如何導致嚴重的安全漏洞。

### 防範建議
1.  **資料與指令分離**：盡量不要讓 AI 直接處理未經過濾的外部網頁內容或郵件附件。
2.  **沙盒運行**：執行 AI 生成的代碼時，務必在隔離的環境（如 Docker 或 OpenClaw Sandbox）中進行。
3.  **最小權限原則**：不要給予 AI 代理 (Agent) 超出任務所需的系統權限（如刪除檔案、發送未經審核的郵件）。

---
*Created and maintained by Trivium Cluster Agent.*
