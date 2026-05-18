# 讓檔案會說話：LLM × 知識圖譜重寫文化遺產基礎建設

> Making the Archive Speak: LLM × Knowledge-Graph Infrastructure for Cultural Heritage — 2026-05-18

## Hook

Medici archives 數位化 20 年了、幾乎沒人讀——太多義大利文、太少 metadata、沒 interface。AI & Society 2025-05 (s00146-025-02238-5) 證明 explainable LLM pipeline + visual finding aid 改變這件事。再加 Metadata Enrichment Model (arXiv 2505.23543) 跟 JCDL 2025 的 SciKGDash + Graphusion——2026 是 LAM convergence（圖書館/檔案/博物館）拿到真技術 stack 的年、不再是 position paper。

## Theoretical anchor

Coppola et al. (2025) Explainable AI, LLM and digitized archival cultural heritage: Medici Grand Ducal Archive, AI & Society; Metadata Enrichment Model (arXiv 2505.23543, May 2025) CV + LLM + KG; Graphusion (ACM Web Conf 2025 Companion) global-perspective scientific KG; SciKGDash (JCDL 2025, John/Auer/Karras); Tradition Meets Innovation review (Knowledge Organization Vol 52 No 4) on LAM convergence。

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | rag-heritage-stack-slide-01-cover.jpg | Cover — 讓檔案會說話：LLM × 知識圖譜重寫文化遺產基礎建設 |
| 2 | rag-heritage-stack-slide-02-why-now-matters.jpg | 檔案早已數位化，卻仍不可讀。Medici archives 數位化 20 年、幾乎沒人讀：不是掃描不夠，而是 metadata 太薄、介面太弱。Coppola et al. 202 |
| 3 | rag-heritage-stack-slide-03-finding-aid-core.jpg | 核心不是模型，是 finding aid。這份 deck 的 LIS 錨點是檔案描述與導覽，不是單次問答；Coppola et al. 2025 把 topic、agent、act |
| 4 | rag-heritage-stack-slide-04-medici-interface.jpg | 介面一變，檔案才成立。AI & Society 2025 的 Medici 個案用 D3.js 視覺 finding aid 疊在歷史信件上，讓人物、事件、地點可被探索；不是把信件 |
| 5 | rag-heritage-stack-slide-05-mem-stack.jpg | MEM 把文化遺產堆疊第一次講完整。arXiv 2505.23543 將 CV、fine-tuned LLM 與 semantic KG 接成專為館藏設計的整合框架，處理異質影像、 |
| 6 | rag-heritage-stack-slide-06-drift-tradeoff.jpg | 讀得更順，未必更真。PastReader 2025 顯示 OCR + LLM pipeline 可改善歷史文本可讀性，但也帶來 modernization drift：方言、拼寫與 |
| 7 | rag-heritage-stack-slide-07-graphusion-federation.jpg | Graphusion 讓跨館藏 federation 有了可移植骨架。Web Conf 2025 Companion 用 global perspective RAG 建 scie |
| 8 | rag-heritage-stack-slide-08-jcdl-interface.jpg | JCDL 2025 證明介面層成熟了。SciKGDash 處理 KG curation 與 dashboarding，另有 VR reading-promoter RAG syst |
| 9 | rag-heritage-stack-slide-09-what-shifted.jpg | 變的是 stack，沒變的是描述責任。2024 前多是 position paper；到 2025-2026，LLM、KG、viz、curation dashboard 開始接成工 |
| 10 | rag-heritage-stack-slide-10-hci-implication.jpg | HCI 問題不是 chat，更是導覽。JCDL 2025 與 Medici 個案都指向同一件事：小型 KG 加好視覺化，常比大原始庫加聊天框更能支持探索。你的 UX archite |
| 11 | rag-heritage-stack-slide-11-cs-implication.jpg | CS 真正的新通用架構是 MEM 式管線。CV + LLM + KG 不只適合 heritage，而是任何 heterogeneous corpus 的可解釋處理框架；關鍵挑戰從模 |
| 12 | rag-heritage-stack-slide-12-cds-implication.jpg | CDS 可把 modernization drift 變成可量測問題。以 NTU TDR 的中文 thesis collection 為例，可比較 OCR 原文、LLM 正規化文本 |
| 13 | rag-heritage-stack-slide-13-luxury-archives.jpg | 文化遺產不是只有公共館舍。LVMH、Gucci、Cartier 這類品牌檔案同樣受困於多語文本、薄 metadata、難查找；MEM、Graphusion、JCDL 式元件正好組成 |
| 14 | rag-heritage-stack-slide-14-counter-evidence.jpg | 反證提醒我們別把可讀當真實。PastReader 2025 的提升建立在現代語言流暢度，但若研究目標是保留歷史語形，LLM 可能正破壞材料。效率、親近性、與史料忠實度之間，需要明確 |
| 15 | rag-heritage-stack-slide-15-open-questions.jpg | 真正未解的是誰來定義『好 enrichment』。Tradition Meets Innovation 對 LAM convergence 的回顧提醒：圖書館、檔案、博物館的描述傳 |
| 16 | rag-heritage-stack-slide-16-method-note.jpg | 方法上可做一個小而硬的設計。選 NTU TDR 2025 中文 thesis 作樣本，建立 OCR、OCR+LLM、OCR+LLM+KG 三路比較，量化 dialect loss、 |
| 17 | rag-heritage-stack-slide-17-literature-gaps.jpg | 文獻缺口在長期治理，不在 demo。Digital Heritage 2025 與 ICCROM《Ctrl+S Culture》把 AI heritage 放回 preservat |
| 18 | rag-heritage-stack-slide-18-three-takeaways.jpg | 三個帶走。finding aid 比 chat 重要；MEM 式 stack 可跨館移植；modernization drift 必須被量化，不然文化遺產只是在被更順手地改寫。 |

## Implications

- **HCI:** Finding aid UX 是未解問題 — JCDL 2025 paper 證明小 KG + 好 viz 打贏大 raw collection
- **CS:** MEM-style multimodal pipeline (CV + LLM + KG) 是下個 general-purpose 架構 for 任何 heterogeneous corpus、不只 heritage
- **Critical Data Studies:** Rose thesis hook：modernization drift 在 OCR+LLM pipeline 是可測量的、methodologically tractable in Chinese-language collection (NTU TDR)

## Key findings

- Medici case study (AI & Society 2025) 用 D3.js visual finding aid over LLM-extracted topic / agent / action / location / event from 歷史信件 — interface 變成 archive
- MEM (arXiv 2505.23543) 是第一個 CV + fine-tuned LLM + semantic KG integrated framework specifically for cultural-heritage collection
- OCR + LLM pipeline (PastReader 2025, CEUR Vol-4098) 比傳統 OCR 強、但帶來 modernization drift — erases dialect + historical structure (quality preservation 取捨)
- Graphusion (2025) 用『global perspective』RAG framework 蓋 scientific KG — 可直接移植到 cross-collection 文化遺產 federation
- JCDL 2025 收 SciKGDash for KG curation + VR reading-promoter RAG system (Zhenyu Li) — 介面層成熟
- Digital Heritage 2025 / ICCROM 『Ctrl+S Culture』(Nov 2025) 把 AI heritage 定位成 heritage preservation 議題、不是 tech deployment 議題 — NTU Asia-Pacific 切入點
- NTU TDR repository 有 2025 LGBTQ research thesis、可作為 modernization drift 在中文 collection 上的 thesis hook
