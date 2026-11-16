---
title: 知識複利與持久化維基 (Compounding Knowledge)
category: Concepts
tags: [LLM-Wiki, 知識管理, RAG]
updated: 2026-11-16
---

# 知識複利與持久化維基 (Compounding Knowledge)

## 核心定義
**知識複利**是指每次加入新的學習資料或提出新問題時，系統不是從零開始重新檢索，而是將新知識直接編譯、整合進既有的結構化維基中，使知識庫的連結密度與洞察力隨時間遞增。

## 傳統 RAG 與 LLM Wiki 的差異
| 比較維度 | 傳統 RAG（如一般檔案上傳問答） | LLM Wiki 持久化維基 |
| :--- | :--- | :--- |
| **知識狀態** | 每次提問重新檢索片段，無長期累積 | 持續更新的 Markdown 結構化頁面 |
| **跨文件綜合** | 每次詢問都需重新拼湊多份文件 | 已預先建立雙向連結與綜合摘要 |
| **矛盾處理** | 容易忽略新舊資料的衝突 | Ingest 階段即主動標記觀點矛盾 |

## 相關來源
- [2026-11-16：Karpathy LLM Wiki 筆記摘要](../sources/2026-11-16-llm-wiki-summary.md)
