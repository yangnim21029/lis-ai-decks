# 幽靈引用：LLM 在學術文獻造出 14 萬筆不存在的引文

> Ghost Citations: LLM-Induced Non-Existent References in Scholarly Literature — 2026-05-21

## Hook

LLM hallucinated reference 不是平均散佈——它們集中在 AI 採用率高的領域、且不成比例地引用 already-prominent (and male) scholar，把現有 prestige 不平等加速放大。傷害不是 error rate 本身、是它在 citation capital 上的方向偏差。圖資長期把 citation network 當 epistemic infrastructure 處理，這篇用 111M 引用 / 2.5M 論文的全網規模數據把 LLM 幻覺從『產品 demo 風險』升級到『學術可信度的結構性污染』、並提出可量化的 Matthew-effect 加速假說。對 HCI/CS 是 evaluator 設計題、對 LIS 是書目控制 (bibliographic control) 重構題。

## Theoretical anchor

Zhao et al. 'LLM hallucinations in the wild: Large-scale evidence from non-existent citations', arXiv:2605.07723 (submitted May 8 2026, indexed and circulating 2026-05-15~21 window); 配 Library Drift (arXiv:2605.19576, May 19) on degradation in self-evolving skill libraries —— 同個 epistemic-rot 家族。

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | ghost-citations-llm-academia-slide-01-cover.jpg | Cover — 幽靈引用：LLM 在學術文獻造出 14 萬筆不存在的引文 |
| 2 | ghost-citations-llm-academia-slide-02-why-this-matters.jpg | 這不是錯字率，是聲望偏差加速器。用 111M 引用與 2.5M 論文看，LLM 幻覺引用集中衝擊高 AI 採用領域，並把 citation capital 導向已顯赫作者。你的 r |
| 3 | ghost-citations-llm-academia-slide-03-theoretical-anchor.jpg | 引用網路不是裝飾，是知識基礎設施。理論錨點放在 Zhao et al.〈LLM hallucinations in the wild〉與 Library Drift，前者量化不存在 |
| 4 | ghost-citations-llm-academia-slide-04-audit-at-scale.jpg | 全網規模稽核，才看得到結構性污染。Zhao et al. 檢查 arXiv、bioRxiv、SSRN、PMC 共 111M references，不是抽樣產品測試，而是把學術引用網 |
| 5 | ghost-citations-llm-academia-slide-05-146k-in-2025.jpg | 保守估計，2025 一年就有 146,932 筆不存在引文。重點不只是數量大，而是它已穿過投稿、預印本與平台收錄流程。副標可點出：錯誤不是邊角噪音，而是進入正式學術流通。 |
| 6 | ghost-citations-llm-academia-slide-06-fields-with-ai.jpg | 錯誤不是平均散佈，而是追著 AI 採用率走。高採用領域與出現 AI assistance 語言標記的論文，幻覺引用風險顯著更高。你的 adoption curve = LIS 的  |
| 7 | ghost-citations-llm-academia-slide-07-penalizing-newcomers.jpg | 受害最重的是小團隊與早期職涯研究者。當引用驗證失敗、追溯成本上升，資源較少的新進者承擔更高修正與信任損失。這裡要把『error burden』畫成不對稱配重，而非平均風險。 |
| 8 | ghost-citations-llm-academia-slide-08-matthew-effect.jpg | 幽靈引用偏向已知名且男性學者。Zhao et al. 指向一種被 LLM 放大的 Matthew effect：不存在的引文也沿既有 prestige 分布生成，讓 credit  |
| 9 | ghost-citations-llm-academia-slide-09-what-shifted.jpg | 變的是污染速度，沒變的是學術場域原本就不平等。LLM 沒發明 prestige hierarchy，但把它自動化、規模化、低成本化。此頁要做綜合：從 individual erro |
| 10 | ghost-citations-llm-academia-slide-10-hci-default-checks.jpg | 對 HCI，引用查核應是預設介面，不是外掛。編輯器、投稿系統、文獻管理器需要把 DOI、arXiv ID、作者-年份一致性做成常駐 surface。你的 form validati |
| 11 | ghost-citations-llm-academia-slide-11-cs-generation-guards.jpg | 對 CS，該把不存在引文當型別錯誤處理。generation time 應有便宜 detector 去檢 DOI、arXiv ID、期刊卷期是否存在，重點比起 RLHF 更像 re |
| 12 | ghost-citations-llm-academia-slide-12-cds-new-graph.jpg | 對 Critical Data Studies，新的資料集單位是 hallucinated citation graph。研究問題不只是哪裡錯，而是 AI 如何重分配可見度、可信度 |
| 13 | ghost-citations-llm-academia-slide-13-library-drift-case.jpg | 案例對照：Library Drift 證明知識庫也會自腐。2026-05-19 論文顯示 LLM-authored skills 平均增益 0.0，遠低於 human-curate |
| 14 | ghost-citations-llm-academia-slide-14-counterevidence-limits.jpg | 反證與限度也要講清楚。不是所有 AI 輔助都必然製造假引文，也可能有領域編輯規範較強、工具鏈較完整而風險較低；但現有 moderation 只抓到少數，不能把局部成功誤讀成系統已解 |
| 15 | ghost-citations-llm-academia-slide-15-open-questions.jpg | 開放問題：誰該為引用驗證付成本？作者、期刊、平台、模型商，還是文獻管理工具？此頁把責任切分成 supply side 與 audit side。你的 observability b |
| 16 | ghost-citations-llm-academia-slide-16-method-note.jpg | 方法註記：這篇強在保守估計與跨庫比對，不把找不到立即等同不存在。要點出其貢獻是把『野外幻覺』做成可重複審計的 bibliometric pipeline，也提醒後續研究需追 DOI |
| 17 | ghost-citations-llm-academia-slide-17-literature-gaps.jpg | 文獻缺口：我們仍缺長期追蹤、跨語種、跨出版社的污染傳播研究。也缺對 gendered prestige amplification、早期學者受損與撤稿外溢效應的縱向證據。此頁可作為 |
| 18 | ghost-citations-llm-academia-slide-18-three-takeaways.jpg | 幽靈引用會累積。污染沿聲望偏差流動。治理重點不是降幻覺率，是重建書目控制、介面查核、生成時型別防線。 |

## Implications

- **HCI:** Citation-checking UI 應該是 scholarly editor 的 default surface、不該是 opt-in plugin
- **CS:** 需要便宜的 detector 在 generation time flag non-existent DOI / arXiv ID——更接近 type-checking、不是 RLHF
- **Critical Data Studies:** Computational social science 得到新 dataset 類別——『hallucinated citation graph』——研究 AI 怎麼 mediate 學術 reputation

## Key findings

- 111M references audited across arXiv / bioRxiv / SSRN / PubMed Central (Zhao et al. 2605.07723)
- Conservative estimate：146,932 hallucinated citations in 2025 alone
- Errors 集中於 AI 採用率高的領域 + 顯示 AI-assistance 語言標記的論文
- Small / early-career 團隊不成比例受害——penalises 新入場者
- Hallucinated cite 偏向 already-prominent and male scholar——Matthew effect on credit
- Library Drift paper (2605.19576, May 19) 證明同樣 rot pattern in agentic skill libraries：LLM-authored skills 0.0 點增益 vs 16.2 from human-curated——auto-generated knowledge 沒治理會 degrade retrieval
- Existing moderation 只捕到一小部分；current peer-review filter miss 絕大多數
