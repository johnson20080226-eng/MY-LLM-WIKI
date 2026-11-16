# 研究筆記：如何結合原子化筆記與 LLM Wiki 建立知識複利系統？

- **建立日期**：2026-11-16
- **資料來源限制**：本報告正文 **100% 嚴格依據本知識庫（`wiki/`）既有內容撰寫**。

## 1. 問題背景：為什麼傳統筆記與 RAG 無法累積知識？
在個人知識管理中，我們常面臨兩大瓶頸：
1. **人工管理的規模瓶頸**：當筆記量從 10 則成長至 300 則以上時，傳統「由上至下」的樹狀資料夾分類會因為現實資訊跨領域且零散而失效（引用自：[朱騏筆記摘要](../wiki/sources/2026-11-16-note-management-summary.md)）。
2. **傳統 RAG 的無記憶瓶頸**：現有 AI 檔案問答系統（RAG）在每次提問時都必須重新檢索碎片並從頭拼湊答案，知識無法沉澱累積（引用自：[Karpathy LLM Wiki 摘要](../wiki/sources/2026-11-16-llm-wiki-summary.md)）。

## 2. 核心解法：原子化單位 ＋ AI 增量編譯
要實現真正的**知識複利**，需要同時結合方法論與系統架構（引用自：[知識複利與持久化維基](../wiki/concepts/compounding-knowledge.md)）：
- **最小筆記單位（Atomic Design）**：將知識拆解為「名詞筆記（關鍵字詞條）」與「觀念筆記（個人理解）」，使單一觀念能透過雙向連結被多個名詞重複引用（引用自：[原子化筆記法](../wiki/concepts/atomic-note-taking.md)）。
- **知識複利公式概念化**：若將知識庫的連結價值視為節點數 $N$ 的函數，當雙向連結密度 $k$ 隨每次 `Ingest` 提升時，知識網路的綜合價值可表示為：
  $$V \propto N \cdot \log(1 + k)$$
- **AI 接手維護成本**：透過 `AGENTS.md` 規範，由人類負責提供 `raw/` 素材與提問，AI 負責在每次 `Ingest` 時自動更新概念頁、標註矛盾並維護 `index.md` 與 `log.md`。

> ⚠️ **知識庫缺口說明**：關於「大規模知識圖譜的向量混合檢索演算法細節（如 BM25 與向量重排權重）」以及「Zettelkasten 卡片盒筆記法的歷史演變」，目前 Wiki 知識庫尚未收錄此部分細節，已列於下方建議文獻供後續吸收。

## 建議收錄文獻（待 Wiki 化）
- [Zettelkasten 卡片盒筆記法完整指南](https://zettelkasten.de/overview/) | 推薦理由：補充原子化筆記與雙向連結的源頭理論，可與現有概念頁進行深度對照。 | 建議檔名：2026-11-16-zettelkasten-method.md
- [QMD: Local Hybrid Search Engine for Markdown](https://github.com/tobi/qmd) | 推薦理由：補足當 Wiki 成長至數百頁時的本地端混合檢索工具實作細節。 | 建議檔名：2026-11-16-qmd-markdown-search.md
