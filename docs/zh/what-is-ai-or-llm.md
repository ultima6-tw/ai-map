# 什麼是 AI 與大型語言模型 (LLM)?

大型語言模型 (Large Language Models, LLM) 是當前 AI 發展的核心。它們透過極大規模的數據學習，預測下一個字出現的機率。

## 生物神經網路 vs. 人工神經網路 (LLM)

理解 LLM 的關鍵進在於其底層結構：**人工神經網路 (Artificial Neural Networks, ANN)**。

- **生物神經網路 (Biological Neural Network)**：人類大腦由數千億個神經元組成，透過突觸傳遞電訊號來學習與反應。
- **人工神經網路 (LLM 的基礎)**：科學家模仿大腦結構，用數學公式模擬神經元的行為。在 LLM 中，這些「模擬神經元」被稱為**參數 (Parameters)**。
- **關係**：LLM 就像是一個數位化的大腦。當我們說一個模型有「1750 億個參數」時，你可以想像它擁有 1750 億個數位神經元連接。透過這些連接，模型能從海量文字中學習語法、邏輯甚至常識。

## 核心運作機制：機率預測

LLM 的本質是一個超級強大的「文字接龍」引擎：
1. **輸入 (Prompt)**：當你輸入一段話時，模型會將其轉化為數值向量 (Tokens)。
2. **預測 (Prediction)**：模型會根據之前的訓練數據，計算出下一個最有可能出現的字。
3. **循環 (Iteration)**：模型產出一個字後，會將其放回輸入中，繼續預測下一個字，直到生成完整的句子。

## 精選科普與教學 (推薦必看)

如果您想深入理解底層原理，這幾位教育者的內容提供極佳的解釋：

- **[李宏毅 Hung-yi Lee (YouTube 頻道)](https://www.youtube.com/@HungyiLeeNTU)**
    - **強烈推薦**：台大李宏毅教授的機器學習與深度學習課程，是全球華語圈公認最優質、最易懂的 AI 入門教材。
    - **[【生成式人工智慧與機器學習導論2025】(YouTube 播放清單)](https://www.youtube.com/playlist?list=PLJV_el3uVTsMMGi5kbnKP5DrDHZpTX0jT)**
        - **最新課程**：李宏毅教授 2025 年的最新生成式 AI 課程，涵蓋了從基礎 LLM 到最新 Agent 技術的完整導論。
- **[A Visual Guide to How LLMs Work](https://youtu.be/XLN2x3bAMLQ?si=WpDqG4B9Xk6_6m7b)**
    - **原理詳解**：3Blue1Brown 製作，深入淺出地解釋了大型語言模型如何將「意義」轉化為向量空間，並進行機率預測。
- **[But what is a GPT? Visual intro to Transformers](https://youtu.be/wjZofJX0v4M?si=GzK16kE_65k7x_9e)**
    - **視覺化神作**：同樣由 3Blue1Brown 製作，利用強大的數學視覺化工具，講解 Transformer 如何運作、什麼是注意力機制 (Attention)。
- **[A Visual Guide to How Llama 3 Works](https://youtu.be/OQ_EhCtNc2M?si=G0kS976G77x_M7N4)**
    - **視覺化詳解**：透過極其精美且直觀的動畫，手把手帶你拆解 Llama 3 的運作過程，從 Tokenization 到輸出。
- **[【漫士科普】GPT 是如何工作的？為什麼要預測下一個詞？](https://youtu.be/j5N2j6Ydhao?si=awVsdfhlfcYgOsiL)**
    - 深入淺出地解釋 GPT 的核心邏輯：機率性地預測下一個 Token。
- **[ChatGPT 原理揭密！背後的黑科技 Transformer](https://youtu.be/nIncwp0iAkw?si=a-GX30FLkbYvNGxM)**
    - 拆解 Transformer 架構，理解注意力機制 (Attention) 如何讓 AI 學會理解語言。
- **[But what is a neural network? | Deep learning chapter 1](https://youtu.be/aircAruvnKk?si=RCSHOuQ3Svu97AI9)**
    - 3Blue1Brown 的經典系列，透過視覺化方式呈現神經網路底層的數學與結構。
- **[Neural Networks: The Full Course](https://youtu.be/shM5KhjcY4M?si=Fp7A9S8T_qV_O4E9)**
    - **進階學習**：由 **3Blue1Brown** 整理的神經網路完整系列。從基礎的神經元概念到微積分在深度學習中的應用，是目前最完整的視覺化神經網路課程。

---
*Created and maintained by Trivium Cluster Agent.*
