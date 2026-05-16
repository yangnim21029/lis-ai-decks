# LIS × AI Decks

LIS 學科在 AI 進場後的 epistemic shift — image-driven decks，給 HCI / CS / Critical Data Studies 學者讀。

每份 deck 18 張、視覺繼承 royal blue #1E3FCC + coral red #EF4F3A + 19 世紀百科全書 engraving + Riso duo-tone。

## Decks

| Date | Topic | Folder |
|------|-------|--------|
| 2026-05-16 | LIS 學科 3 年的 epistemic shift（跨學科總覽） | [`decks/2026-05-16-cross-disciplinary`](decks/2026-05-16-cross-disciplinary) |

## 技術

- Image gen：OpenAI Codex CLI 內建 image_gen（gpt-5.4）
- Deck build：pptxgenjs + LibreOffice headless PDF
- JPEG 壓縮：mozjpeg adaptive ~100KB/張（`compress-deck-jpegs.py`，來自 superpower_ppt 共用 helper）

## 索引欄位

每個 deck folder 內含：
- `lis-ai-slide-01-cover.jpg` ... `lis-ai-slide-18-closing.jpg`（18 張、~100KB/張、binary JPEG 可直接 GitHub 內預覽）
- `README.md` — slide-by-slide content + 理論 anchor + implications
