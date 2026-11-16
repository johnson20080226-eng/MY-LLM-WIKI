---
title: 2026-11-16：Karpathy LLM Wiki 筆記摘要
category: Sources
tags: [Karpathy, AGENTS.md, 筆記系統]
updated: 2026-11-16
---

# 2026-11-16：Karpathy LLM Wiki 筆記摘要

- **原始檔案**：`raw/2026-11-16-llm-wiki-concept.md`
- **相關概念**：[知識複利與持久化維基](../concepts/compounding-knowledge.md)

## 核心重點整理
1. **三層架構分工**：
   - `raw/`：唯讀的原始資料來源，AI 不可修改。
   - `wiki/`：AI 全權維護的 Markdown 知識庫，包含概念頁與摘要頁。
   - `AGENTS.md`（Schema）：定義目錄結構與自動化操作規則的設定檔。
2. **三大核心操作**：
   - **Ingest（吸收）**：讀入新資料，同步更新摘要頁、概念頁、目錄與日誌。
   - **Query（查詢）**：依 `index.md` 檢索回答，並將高價值分析回寫為新頁面。
   - **Lint（健檢）**：定期檢查頁面矛盾、孤島頁面與缺失連結。
