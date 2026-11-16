# 📚 個人學習筆記 LLM Wiki 與自動化研究簡報系統

本專案結合 **Andrej Karpathy 的 LLM Wiki 架構** 與 **原子化筆記法**，建立一個持續累積、具備複利效應的個人知識庫，並內建**互動式 HTML 研究簡報**。

## 🚀 線上瀏覽方式（GitHub Pages）

1. 將本專案所有檔案上傳至您的 GitHub Public Repository。
2. 進入 Repository 的 **Settings** → **Pages**。
3. 在 **Source** 選擇 `Deploy from a branch`，分支選擇 `main`、資料夾選擇 `/ (root)`，點擊 **Save**。
4. 等待約 1–2 分鐘，即可透過 `https://<您的帳號>.github.io/<倉庫名稱>/` 線上瀏覽知識庫與播放簡報！

## 📂 專案結構
- `index.html` & `style.css`：知識庫網頁主入口（支援 Markdown 渲染、KaTeX 公式與一鍵下載建議文獻）。
- `slides_html/2026-11-16-compounding-pkm-research.html`：**獨立可播放的現代學術極簡風 HTML 簡報**（支援方向鍵換頁、`S` 鍵開啟講者備忘錄、全螢幕播放）。
- `notes/`：嚴格基於 Wiki 產出的研究筆記。
- `slides_script/`：簡報逐頁腳本與講者逐字稿。
- `wiki/`：知識維基核心層（總目錄、演進日誌、概念頁與來源摘要）。
