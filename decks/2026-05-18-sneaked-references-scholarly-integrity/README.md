# 被偷渡的引用：學術誠信在 LLM 時代的崩塌與重建

> Sneaked References and Paper Mills: Reconstructing Scholarly Integrity in the LLM Era — 2026-05-18

## Hook

Crossref 說一篇論文有 50 個 citation、Google Scholar 找到 8 個——有人在作弊、人眼看不到。Besançon, Cabanac, Labbé, Magazinov 2024 JASIST 75(12)（拿 2025 JASIST Best Paper Award）證明：publishers 可以把 citation 註冊成 metadata 但不出現在文章正文，把 bibliometrics 整個 game 掉。再疊上 paper mill、LLM 編造的 reference、citation ring——scholarly comm 變成有真實對手的 security problem，LIS 擁有 threat model。

## Theoretical anchor

Besançon et al. (2024, JASIST 75(12)) sneaked references — 2025 JASIST Best Paper Award; LAGMiD (ICLR 2025, arXiv 2603.12290) miscitation 偵測 via LLM-augmented text-rich graph; Liu et al. (2025, J. Data and Information Science) PDCN paper-mill detection via heterogeneous citation graph; Co-Reviewer (Scientometrics 2026, s11192-026-05557-6); ChatGPT-4o / Claude 3.5 / Gemini-EXP-1206 vs 180 eLife reports (Scientometrics 2026, s11192-026-05622-0)。

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | scholarly-integrity-llm-slide-01-cover.jpg | Cover — 被偷渡的引用：學術誠信在 LLM 時代的崩塌與重建 |
| 2 | scholarly-integrity-llm-slide-02-why-it-matters.jpg | 你以為是 citation count，其實是 attacked pipeline。用 Crossref 50 vs Google Scholar 8 的落差開場：人眼只看正文，平 |
| 3 | scholarly-integrity-llm-slide-03-lis-theoretical-anchor.jpg | LIS 不是編書架，是管理引用基礎設施。介紹 Besançon、Cabanac、Labbé、Magazinov 2024 JASIST 75(12)，並點出其獲 2025 JASI |
| 4 | scholarly-integrity-llm-slide-04-sneaked-references.jpg | 偷渡引用不是 typo，是設計過的 metadata attack。說明 Besançon et al. 如何抓到 publisher 把 citation 註冊進 Crossre |
| 5 | scholarly-integrity-llm-slide-05-bibliometrics-gamed.jpg | 被 game 的不是單篇論文，而是整條 bibliometrics 鏈。呈現 Google Scholar 依正文抽取、Crossref 依出版者提交的差異，強調同一篇文獻可在兩平 |
| 6 | scholarly-integrity-llm-slide-06-lagmid-miscitation.jpg | 誤引不只是粗心，可能是系統性訊號。引入 ICLR 2025 的 LAGMiD：以 LLM 增強的 text-rich citation graph 偵測被誤述或互相矛盾的 clai |
| 7 | scholarly-integrity-llm-slide-07-paper-mill-graph.jpg | paper mill 已能在圖上留下指紋。介紹 Liu et al. 2025 在《Journal of Data and Information Science》的 PDCN：B |
| 8 | scholarly-integrity-llm-slide-08-agentic-peer-review.jpg | 連 peer review 也進入 agentic 重寫。串連 Co-Reviewer（Scientometrics 2026）與 180 篇 eLife review 比較研究： |
| 9 | scholarly-integrity-llm-slide-09-what-shifted.jpg | 變的是攻擊面，不變的是信任要靠基礎設施。綜合 Besançon、LAGMiD、PDCN：從假引用、誤引到 paper mill，問題都落在文字、圖譜、metadata 三層失配，而 |
| 10 | scholarly-integrity-llm-slide-10-hci-implications.jpg | HCI 要做的是 adversarial UX，不是更順手的 reference manager。把 Crossref metadata 與正文不一致做成即時警示，再加 in-li |
| 11 | scholarly-integrity-llm-slide-11-cs-implications.jpg | CS 該把 citation graph 當成遭攻擊的系統，不只是資料集。以 LAGMiD 與 PDCN 為例，GNN + LLM hybrid 應從研究 demo 轉向 publ |
| 12 | scholarly-integrity-llm-slide-12-cds-implications.jpg | Critical Data Studies 的問題變成：誰定義可信 metadata。主張 Computational Data Science 課程加入 research int |
| 13 | scholarly-integrity-llm-slide-13-brand-analogy.jpg | 偷渡的 citation，對品牌端就是偷渡的評價。把 Amazon review-manipulation ring、Trustpilot、BazaarVoice 放進對照：你的  |
| 14 | scholarly-integrity-llm-slide-14-counter-evidence.jpg | 不是所有平台差異都等於作弊。這頁要交代反證與保守解讀：版本差、收錄延遲、解析失誤也會造成 citation 不一致，因此 Besançon 的價值在於把可疑模式制度化，而非靠個案獵 |
| 15 | scholarly-integrity-llm-slide-15-open-questions.jpg | 真正難題是責任邊界畫在哪裡。提出三問：publisher 需不需驗證正文與 metadata 一致、索引平台何時該拒收、作者與 reviewer 對 LLM 生成參考文獻要負到哪一 |
| 16 | scholarly-integrity-llm-slide-16-methodological-note.jpg | 方法上要避免只迷信單一模型分數。說明這個領域結合 case-based forensic reading、citation graph learning、LLM judge 與人工 |
| 17 | scholarly-integrity-llm-slide-17-literature-gaps.jpg | 文獻還缺跨平台、跨出版社、跨語言的長期追蹤。指出 2024-2026 研究多集中生醫與一般科學英文文獻，對社科、人文、中文出版與商業評價平台的遷移證據仍不足。 |
| 18 | scholarly-integrity-llm-slide-18-three-takeaways.jpg | 引用是基礎設施。完整性是對抗問題。LIS 提供 threat model。副標固定 24 字：別只管模型輸出 也要管 metadata 管線 與 citation graph 攻擊 |

## Implications

- **HCI:** Reviewer tool 跟 reference manager 需要 adversarial UX — Crossref metadata 跟正文不合時即時顯示、in-line miscitation risk indicator
- **CS:** Citation graph 變成 attacked surface — GNN + LLM hybrid (LAGMiD, PDCN) 從 research demo 變 publisher 生產基礎建設
- **Critical Data Studies:** Computational Data Science 學程需要『research integrity』module — scientometrics 是 trust 的 data science、而 trust 變 adversarial

## Key findings

- Sneaked reference 利用 publisher → Crossref → bibliometrics 平台的 metadata pipeline；Google Scholar (text-extracted) vs Crossref (publisher-supplied) 在作弊論文上差幾個 order of magnitude (Besançon 2024 JASIST)
- LAGMiD 在一般科學文獻偵測到高達 25% miscitation rate、用 chain-of-thought 跑 text-rich citation graph 找 contradicted claims (ICLR 2025)
- PDCN paper-mill detector 81.85% accuracy / 80.49% F1：BERT title features + heterogeneous graph attention on citation network (J. Data and Information Science 2025)
- Co-Reviewer (Scientometrics 2026) 蓋出 agentic LLM-human alignment framework for peer review — bibliographic stack 兩邊都被 agent 重寫
- ChatGPT-4o / Claude 3.5 / Gemini-EXP-1206 在 180 篇 eLife biomedical peer review 報告上、開始改變 review 的 linguistic form 跟 evaluative focus、不只是輔助 (Scientometrics 2026)
- JASIST 2025 Best Paper Award 把 LIS 定位成『citation infrastructure 的學科』、不是『編書架的學科』
- Brand-side 對映：Amazon review-manipulation rings 用同樣 metadata-vs-text gap、Trustpilot / BazaarVoice 還慢一步
