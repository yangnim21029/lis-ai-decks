# LIS × AI Decks

LIS 學科在 AI 進場後的 epistemic shift — image-driven decks，給 HCI / CS / Critical Data Studies / 行銷 / 奢侈品讀者讀。

每份 deck 18 張、視覺繼承 royal blue #1E3FCC + coral red #EF4F3A + 19 世紀百科全書 engraving + Riso duo-tone。每張 JPG 用 mozjpeg adaptive 壓到 ~100KB。

## 怎麼預覽

**直接點 deck 資料夾下的 README.md**（推薦）—GitHub 會把 18 張 JPG 內嵌 inline 渲染、像看 deck 一樣往下滑、不用打開檔案。

也可以：
- **點任何 .jpg**：GitHub 會直接顯示原圖
- **clone repo**：`git clone https://github.com/yangnim21029/lis-ai-decks` 然後在本機資料夾用任何 image viewer 看
- **本機 PDF**：每個 deck 的 `.pptx` 在 [`_work/<topic-id>/`](_work/)（local only、未 push 因為太大）；要 PDF 用 `soffice --headless --convert-to pdf <pptx>` 自己轉

## 怎麼讀順序

`results.md` 是依完成時間排序的索引。看標題挑想看的、點進去就是 README + 18 張圖。

## Decks (round 1 + round 2)

| Date | Topic | Folder |
|------|-------|--------|
| 2026-05-16 | LIS 學科 3 年的 epistemic shift（跨學科總覽） | [`decks/2026-05-16-cross-disciplinary`](decks/2026-05-16-cross-disciplinary) |
| 2026-05-17 | 後 SEO 時代：當品牌要被 LLM 引用 | [`decks/2026-05-17-geo-after-seo-llm-citation`](decks/2026-05-17-geo-after-seo-llm-citation) |
| 2026-05-17 | AI 素養新標尺：UNESCO / OECD / AILIS 1.0 | [`decks/2026-05-17-ai-literacy-ailis-1-unesco`](decks/2026-05-17-ai-literacy-ailis-1-unesco) |
| 2026-05-17 | 當分類法遇上 LLM：知識組織 × RAG | [`decks/2026-05-17-knowledge-org-meets-llm`](decks/2026-05-17-knowledge-org-meets-llm) |
| 2026-05-17 | 把 1980 的照片變成 2026 的廣告：奢侈品檔案 AI 復活 | [`decks/2026-05-17-luxury-heritage-archive-ai`](decks/2026-05-17-luxury-heritage-archive-ai) |
| 2026-05-17 | 你的下個造型師是 AI agent：Kering Madeline | [`decks/2026-05-17-agentic-luxury-shopping-stylist`](decks/2026-05-17-agentic-luxury-shopping-stylist) |
| 2026-05-17 | 合成代言人時代：AI influencer × EU AI Act + FTC | [`decks/2026-05-17-synthetic-influencer-eu-ai-act`](decks/2026-05-17-synthetic-influencer-eu-ai-act) |
| 2026-05-18 | 被偷渡的引用：學術誠信 × LLM | [`decks/2026-05-18-sneaked-references-scholarly-integrity`](decks/2026-05-18-sneaked-references-scholarly-integrity) |
| 2026-05-18 | 錯訊治理的社會技術轉向 | [`decks/2026-05-18-misinfo-sociotechnical-governance`](decks/2026-05-18-misinfo-sociotechnical-governance) |
| 2026-05-18 | 讓檔案會說話：LLM × KG × 文化遺產 | [`decks/2026-05-18-rag-cultural-heritage-stack`](decks/2026-05-18-rag-cultural-heritage-stack) |
| 2026-05-18 | 代理人接管 MMM：multi-touch attribution 的死亡 | [`decks/2026-05-18-agentic-marketing-mix-modeling`](decks/2026-05-18-agentic-marketing-mix-modeling) |
| 2026-05-18 | Entrupy × Vestiaire：AI 鑑定重建二手奢侈品信任 | [`decks/2026-05-18-luxury-resale-ai-authentication`](decks/2026-05-18-luxury-resale-ai-authentication) |
| 2026-05-18 | Aman 的生物指標管家：奢華服務業 AI 個人化 | [`decks/2026-05-18-luxury-ai-hospitality-biometric`](decks/2026-05-18-luxury-ai-hospitality-biometric) |

> 完整完成時間表 → [`results.md`](results.md)

## 技術 stack

- **Image gen**：OpenAI Codex CLI 內建 image_gen（gpt-5.4）
- **Deck build**：pptxgenjs (Node.js)
- **PDF (optional)**：LibreOffice headless
- **JPEG compression**：mozjpeg adaptive quality search（target ~100KB / slide、見 [`compress-deck-jpegs.py`](../superpower_ppt/compress-deck-jpegs.py)）
- **Orchestration**：`autonomous-deck-loop.sh`（loop runner）→ `pipeline-one-deck.sh`（one deck end-to-end）

## 索引欄位（每個 deck folder 內含）

- `<topic-id>-slide-01-cover.jpg` ... `<topic-id>-slide-18-*.jpg`（18 張、~100KB、binary JPG、GitHub 內預覽）
- `README.md` — hook + theoretical anchor + slide-by-slide content table + key findings + implications + **inline 圖**
