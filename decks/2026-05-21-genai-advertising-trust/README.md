# 生成式 AI 廣告：四層干預裡只有第一層被治理

> Generative AI Advertising: A Four-Tier Taxonomy, Only One Tier Governed — 2026-05-21

## Hook

GenAI 廣告有四層干預——product mention (observable) / information framing / behavioral redirection / long-term preference shaping (unobservable)。現行治理跟 deployed system 集中在 tier 1。Tier 3-4 是 welfare-relevant influence 的所在、而且是 invisible by construction。這篇明確帶入 FAccT 2026 詞彙：attributable / measurable / contestable / aligned with user welfare。對 HCI 是設計題 (怎麼讓 tier 3-4 變 observable)；對 CS 是技術題 (怎麼偵測 RAG 廣告)；對 CDS 是治理題 (揭露聲明完全不夠)。

## Theoretical anchor

Qiu, Mei 'Generative AI Advertising as a Problem of Trustworthy Commercial Intervention', arXiv:2605.18673 (cs.CY + cs.CL, May 18, 2026)

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | genai-advertising-trust-slide-01-cover.jpg | Cover — 生成式 AI 廣告：四層干預裡只有第一層被治理 |
| 2 | genai-advertising-trust-slide-02-why-care-now.jpg | 四層干預，治理只抓得到第一層。2605.18673〈1 Introduction〉把問題從 ad placement 改寫成 trustworthy intervention；對  |
| 3 | genai-advertising-trust-slide-03-anchor-paper-map.jpg | 理論錨點不是經典舊文，是本週 arXiv 新框架。Qiu 與 Mei 在〈2 The Current Landscape〉、〈3 A Taxonomy of Generative  |
| 4 | genai-advertising-trust-slide-04-four-tier-taxonomy.jpg | 不是一種廣告，是四層影響階梯。〈3.1 Influence Tiers〉與 Table 2 直接列出 Tier 1 product、Tier 2 framing、Tier 3 re |
| 5 | genai-advertising-trust-slide-05-only-tier-one.jpg | 現行部署與治理，幾乎都停在最淺層。〈2.1 What are Deployed in Industry〉的 Table 1 只盤點 6 個主流 surface，且都圍繞 clear |
| 6 | genai-advertising-trust-slide-06-detection-gap.jpg | 可見，不等於可被看見。〈3.1 Influence Tiers〉引用 Tang et al. 2025 指出 49% 使用者無法辨識 woven Tier 1 ads；連最易治理的 |
| 7 | genai-advertising-trust-slide-07-rag-bias-surface.jpg | RAG 把 retrieval 變成新廣告位，但使用者看不到。〈3.2 Case Studies: Advertising in RAG and Agentic Pipelines |
| 8 | genai-advertising-trust-slide-08-agentic-cascade.jpg | Agent 讓影響從回答內容升級成路徑控制。〈3.2〉的 agentic pipeline 與 Table 3 明列 4 個干預入口：context assembly、tool s |
| 9 | genai-advertising-trust-slide-09-what-shifted.jpg | 變的是干預位置，沒變的是商業誘因。〈4 Discussion〉說 deployed systems 與 academic mechanism design 都集中在 shallow |
| 10 | genai-advertising-trust-slide-10-hci-implication.jpg | 對 HCI，核心不是 disclosure widget，而是讓潛層影響可被看見。〈3.3 Towards Trustworthy Intervention〉與〈4 Discuss |
| 11 | genai-advertising-trust-slide-11-cs-detection.jpg | 對 CS，偵測器不能只抓品牌名。〈3.1〉明說 Tier 2 需要 counterfactual baseline comparison，Tier 3 需要 action attr |
| 12 | genai-advertising-trust-slide-12-cds-object.jpg | 對 CDS，研究對象是 commercial intervention in epistemic infrastructure。〈1 Introduction〉把『產品被放進哪裡』 |
| 13 | genai-advertising-trust-slide-13-case-rag-evidence.jpg | 案例頁：Tier 2 已有可量化前兆。〈3.1〉引 Aggarwal et al. 2024，指出 GEO 可讓 source visibility 在 LLM responses |
| 14 | genai-advertising-trust-slide-14-counterevidence-limits.jpg | 反證也要說清楚：目前多數深層證據仍偏 feasibility。〈4 Discussion〉明言 Tiers 2-4 的證據更接近 feasibility demonstration |
| 15 | genai-advertising-trust-slide-15-open-questions.jpg | 開放問題：誰來量測沒有顯性物件的影響？〈3.2 The cascade challenge〉追問 cascading multi-stage pipelines 怎麼做 attri |
| 16 | genai-advertising-trust-slide-16-method-note.jpg | 方法註：這篇強在 framework，不在新實驗。原文可直接抓到的是 arXiv HTML 的〈1〉到〈4〉、Table 1-3 與引文數字；因此本 deck 的量化主要來自作者在 |
| 17 | genai-advertising-trust-slide-17-literature-gaps.jpg | 文獻缺口其實已被作者點名。〈3.1 Tier 4〉說 detection requires longitudinal analysis，且 privacy-preserving m |
| 18 | genai-advertising-trust-slide-18-three-takeaways.jpg | 只治 Tier 1。真正風險在 Tier 3-4。治理要從揭露版位，轉向量測干預、追蹤路徑、審計偏好漂移。 |

## Implications

- **HCI:** 需要 longitudinal preference-drift instrument——single-session usability test 系統性 miss tier 4
- **CS:** Detection problem：建 classifier flag information-framing 跟 retrieval-bias 為獨立 signal type、不只 product mention
- **Critical Data Studies:** Information science 拿到新研究對象——『commercial intervention in epistemic infrastructure』——乾淨的 dissertation lane

## Key findings

- 四層 taxonomy：product mention / information framing / behavioral redirection / long-term preference shaping (2605.18673)
- Deployed system 跟 current governance 都集中在 tier 1 (最 observable)——structural mismatch
- Retrieval-augmented generation 製造新 attack surface——biased retrieval = biased framing without user-visible product placement
- Agentic system 放大問題——agent act in user's name with advertiser's preference
- 中心問題 reframe：不再是『is this an ad?』、而是『can commercial influence be made attributable / measurable / contestable / welfare-aligned?』
- Tier 4 (long-term preference shaping) 只能透過 longitudinal user study 觀察——single-session UX research 系統性 miss
- Disclosure-only governance (TikTok / IG-style sponsored tag) 不夠——只 apply tier 1
