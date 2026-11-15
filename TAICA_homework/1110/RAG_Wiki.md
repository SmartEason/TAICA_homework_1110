📘 你的 LLM Wiki 主題：RAG (Retrieval-Augmented Generation) 知識庫
1. 什麼是 RAG？ (定義與核心概念)

全名：Retrieval-Augmented Generation（檢索增強生成）。

概念：結合「資訊檢索」與「AI 生成」的技術框架。允許大型語言模型（LLM）在不重新訓練的情況下，直接讀取企業內部或外部資料庫來回答問題。

解決痛點：有效解決傳統 AI 的「幻覺（虛構錯誤資訊）」與「資訊過時」問題。（來源：AWS 參考連結：https://aws.amazon.com/tw/what-is/retrieval-augmented-generation/）

2. RAG 的四大運作步驟 (Workflow)

資料收集：準備專屬文本資料（如 FAQ、產品手冊）。

文本分塊與向量化 (Chunking & Embedding)：將長篇資料切分小段落，透過嵌入模型轉換為 AI 能理解的向量格式。

問題分析與檢索 (Retrieval)：使用者提問時，系統在向量資料庫中搜尋，精準找出高度相關的資料區塊。

生成回答 (Generation)：將檢索到的背景知識與提問一併交給 LLM，統整產出精準答案。（來源：田中系統 參考連結：https://ai-automation.tscloud.com.tw/blog/ai-trends/what-is-rag）

3. RAG 的三大商業優勢

取得最新資訊：突破 LLM 預訓練資料的時間限制，即時連接最新數據。

事實依據 (Grounding)：強制 AI 根據檢索到的參考資料回答，大幅降低幻覺，提升信任度。

高性價比：相比高昂的「微調 (Fine-tuning)」基礎模型，RAG 成本更低且能靈活更新知識庫。（來源：Google Cloud 參考連結：https://cloud.google.com/use-cases/retrieval-augmented-generation?hl=zh-TW）

4. 實際應用場景

智慧客服系統：串接內部規定，提供精確回應。

教育與研究平台：從龐大文獻中檢索並提煉專業解釋。

內容生成與分析工具：快速從大量文件中抓取重點、生成摘要，輔助商業決策。（來源：Appen 參考連結：https://tw.appendata.com/blogs/rag）

5. 底層關鍵技術

語意檢索與向量化：傳統關鍵字搜尋不足以應付複雜提問。RAG 依賴嵌入模型（如 Sentence Transformer）將文字轉為「向量」。

運作機制：計算「語意相似度」，找出語意最接近的知識片段，讓大規模資料的檢索與生成快速且準確。（來源：InfuseAI 參考連結：https://blog.infuseai.io/rag-retrieval-augmented-generation-introduction-a5854cb6393e）