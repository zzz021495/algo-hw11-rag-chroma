# Algorithms HW11 – RAG Retrieval with Chroma DB

## 學生資訊
- 姓名：[陳宣伃]
- 學號：[b3230941]
- 課程：3468 演算法 1142

## 實驗環境
- 平台：Windows 11 本機環境 (PowerShell)
- 向量資料庫：Chroma DB
- 評估指標：Recall@3

## 檢索測試 (sample_queries.txt 摘要)
本實驗設計了 4 個中英文 Query，測試 RAG 系統是否能精準從課本教材中檢索出正確章節內容。測試結果如下，4 個問題皆順利在 Top-3 內命中目標（Top-3 Hit = Yes）：

1. **Query 1 (English):** What is a direct-address table? 
   - *Result:* Top-3 Hit = Yes
2. **Query 2 (English):** How does chaining resolve collisions?
   - *Result:* Top-3 Hit = Yes
3. **Query 3 (中文):** 什麼是雜湊衝突 (Hash Collision)?
   - *Result:* Top-3 Hit = Yes
4. **Query 4 (中文):** 除法雜湊法 (Division Method) 怎麼運作?
   - *Result:* Top-3 Hit = Yes

## 評估結果 (eval_output.txt 摘要)
根據 `eval.py` 的自動化評估腳本，本 RAG 系統之最終精準度指標為：
- **Overall Recall@3: 1.0000 (100%)**

實驗數據顯示系統檢索成功率達到 100%，確認 Chroma 向量資料庫的索引建立（ingest）與相似度檢索（query retrieval）功能完全正常運作，順利達成實驗效益。

## 對應作業
- 作業：3468 演算法 HW11 (Ch11) Problem 8(b)
