---
title: Karpathy LLM Wiki 筆記摘要
date: 2026-11-16
---
# 2026-11-16：Karpathy LLM Wiki 筆記摘要

- **核心觀點**：傳統 RAG 每次提問皆從零檢索碎片，缺乏長期知識沉澱；LLM Wiki 則由 AI 擔任全職維護者，持續編譯持久化維基。
- **三層架構**：`raw/`（唯讀原始資料）、`wiki/`（AI 維護的知識庫）、`AGENTS.md`（操作規範 Schema）。
- **三種核心操作**：`Ingest`（吸收更新）、`Query`（查詢沉澱）、`Lint`（健康檢查）。
- **關聯概念**：[知識複利與持久化維基](../concepts/compounding-knowledge.md)
