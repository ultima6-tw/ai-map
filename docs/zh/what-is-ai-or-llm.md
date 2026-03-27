# 什麼是 AI 與大型語言模型 (LLM)?

大型語言模型 (Large Language Models, LLM) 是當前 AI 發展的核心。它們透過極大規模的數據學習，預測下一個字出現的機率。

## 核心運作機制：機率預測

LLM 的本質是一個超級強大的「文字接龍」引擎：
1. **輸入 (Prompt)**：當你輸入一段話時，模型會將其轉化為數值向量 (Tokens)。
2. **預測 (Prediction)**：模型會根據之前的訓練數據，計算出下一個最有可能出現的字。
3. **循環 (Iteration)**：模型產出一個字後，會將其放回輸入中，繼續預測下一個字，直到生成完整的句子。

## 精選科普影片 (推薦必看)

如果您想深入理解底層原理，這幾段影片提供極佳的視覺化解釋：

- **[【漫士科普】GPT 是如何工作的？為什麼要預測下一個詞？](https://youtu.be/j5N2j6Ydhao?si=awVsdfhlfcYgOsiL)**
    - 深入淺出地解釋 GPT 的核心邏輯：機率性地預測下一個 Token。
- **[ChatGPT 原理揭密！背後的黑科技 Transformer](https://youtu.be/nIncwp0iAkw?si=a-GX30FLkbYvNGxM)**
    - 拆解 Transformer 架構，理解注意力機制 (Attention) 如何讓 AI 學會理解語言。
- **[But what is a neural network? | Deep learning chapter 1](https://youtu.be/aircAruvnKk?si=RCSHOuQ3Svu97AI9)**
    - 3Blue1Brown 的經典系列，透過視覺化方式呈現神經網路底層的數學與結構。

---
*Created and maintained by Trivium Cluster Agent.*
