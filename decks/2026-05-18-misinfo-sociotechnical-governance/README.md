# 錯訊治理的社會技術轉向：從偵測模型到制度設計

> From Detectors to Governance: The Sociotechnical Turn in Misinformation — 2026-05-18

## Hook

ML/HCI 處理 misinformation 大多在 optimize classifier。Sanfilippo, Zhu, Yang 2025 ARIST review on JASIST 76(1) 攤牌：30 年 detector 沒 move the needle、因為這是 sociotechnical governance 問題、不是 classification accuracy 問題。他們綜合 1991-2023 277 篇文獻、提出橫跨 systems / services / interactions / individuals 的 flexible governance model——LIS 最接近 platform accountability 統一理論的東西、剛好踩在 LLM 時代。

## Theoretical anchor

Sanfilippo, Zhu & Yang (2025) Sociotechnical Governance of Misinformation, JASIST 76(1) ARIST 文章；Nature Communications (2025, s41467-025-67145-1) Linguistic features of AI mis/disinformation 跟 LLM 偵測 limit；Schroeder et al. (2025) Malicious AI Swarms and Democracy, arXiv 2506.06299；EU Parliament Briefing PE 779259 (2025) on information manipulation in GenAI age。

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | misinfo-sociotechnical-governance-slide-01-cover.jpg | Cover — 錯訊治理的社會技術轉向：從偵測模型到制度設計 |
| 2 | misinfo-sociotechnical-governance-slide-02-why-now-matters.jpg | 別再只優化 detector。30 年 misinformation 研究把力氣押在分類器，卻沒真正移動治理成效；這頁要讓 HCI/CS/CDS 看見：你的 accuracy 問題 |
| 3 | misinfo-sociotechnical-governance-slide-03-lis-anchor-model.jpg | LIS 經典現在變成總框架。介紹 Sanfilippo、Zhu、Yang 2025《Sociotechnical Governance of Misinformation》：綜合  |
| 4 | misinfo-sociotechnical-governance-slide-04-five-intervention-layers.jpg | 五個介入面，不只刪文。這頁要展開 systems、information、services、interactions、individuals 五層治理面向，強調 Sanfilipp |
| 5 | misinfo-sociotechnical-governance-slide-05-detectors-hit-limit.jpg | 偵測軍備競賽碰壁了。依 Nature Communications 2025，LLM 生成 mis/disinformation 的語言特徵更具 detection-resista |
| 6 | misinfo-sociotechnical-governance-slide-06-swarms-break-moderation.jpg | 單點防守，擋不住 AI swarm。引用 Schroeder et al. 2025 惡意 AI swarms：多代理、協調式、持續調整的操作已超過 single-shot det |
| 7 | misinfo-sociotechnical-governance-slide-07-governance-catches-up.jpg | 威脅升級，制度才開始追。用 EU Parliament Briefing PE 779259 與 2025 AI Act 脈絡，交代 incident telemetry、repo |
| 8 | misinfo-sociotechnical-governance-slide-08-factcheck-tools-vary.jpg | 工具表現不穩，操作治理更關鍵。引 Information Research 2025 對 Facebook disability misinformation 的 LLM fact |
| 9 | misinfo-sociotechnical-governance-slide-09-what-shifted-stayed.jpg | 變的是生成速度，不變的是治理責任。綜合 1990s everyday misinformation lineage 到 2025 LLM 平台，指出內容型態、規模、協調性大變，但可 |
| 10 | misinfo-sociotechnical-governance-slide-10-hci-governance-surfaces.jpg | HCI 不能只做 label。這頁要把 implications_hci 落成 governance-surface UX：版本歷史、來源 provenance、介入透明度、申訴節 |
| 11 | misinfo-sociotechnical-governance-slide-11-cs-needs-simulation.jpg | CS 要從 benchmark 走向 simulation。靜態 test set 已不足，應結合 multi-agent swarm scenario、干預成本、誤傷外部性與恢復 |
| 12 | misinfo-sociotechnical-governance-slide-12-cds-audit-agenda.jpg | CDS 的題目已經長出來了。以平台 governance disclosure 對照實際 takedown log、appeal trace、事件通報，做 empirical au |
| 13 | misinfo-sociotechnical-governance-slide-13-luxury-brand-safety.jpg | Luxury 是治理，不只是 brand safety。把關鍵字封鎖、帳號標記、冒名處置映射到五層治理模型，說明高端品牌更依賴長時段信任與真偽秩序；你的 brand imperso |
| 14 | misinfo-sociotechnical-governance-slide-14-counterevidence-boundaries.jpg | 不是說 detector 全無價值。這頁要放入反證與邊界：在高風險事件初期、狹域語料、明確政策規則下，分類器仍有 operational value；但它是治理模組之一，不是治理本 |
| 15 | misinfo-sociotechnical-governance-slide-15-open-questions-power.jpg | 誰定義 harm，誰承擔誤傷？順著 Sanfilippo et al. 往下問：平台、政府、第三方查核、品牌安全團隊與使用者之間，權力如何分配，透明度要揭露到哪一層才算負責。 |
| 16 | misinfo-sociotechnical-governance-slide-16-methods-across-logs.jpg | 方法上要把文獻、介面與紀錄接起來。建議混合 systematic review、policy tracing、interface walkthrough、takedown log  |
| 17 | misinfo-sociotechnical-governance-slide-17-literature-gaps-map.jpg | 缺口不在模型大小，在跨層證據。點出目前研究仍少見長期追蹤、跨平台比較、非英語場域、品牌冒名與日常服務治理資料；ASIS&T 2025 retrospective 可作 LIS 歷史 |
| 18 | misinfo-sociotechnical-governance-slide-18-three-takeaways.jpg | 錯訊不是純分類問題。治理要跨平台服務互動個體。LLM 時代勝負在可見性、問責、長期信任。 |

## Implications

- **HCI:** Design 必須超越 misinformation label、走向 governance-surface UX — version history、source provenance、intervention transparency 都要 platform 層級暴露
- **CS:** Detection benchmark 要跟 governance simulation environment 配（multi-agent swarm scenario）、不再只是 static test set
- **Critical Data Studies:** CDS 學位論文題：對照 platform governance disclosure vs 實際 takedown log 做 empirical audit — 可量、可資助、可發 FAccT/JASIST

## Key findings

- Sanfilippo et al. 2025 JASIST 把 277 篇綜合成 governance model 五個介入面：systems / information / services / interactions / individuals — 不只『偵測 + 移除』
- Nature Communications 2025：LLM-generated mis/disinfo 的 linguistic features 系統性 detection-resistant、戳破 detector arms race 預設
- Schroeder et al. (arXiv 2506.06299, 2025) 記錄 malicious AI swarms — coordinated multi-agent LLM operation 打敗 single-shot detection
- EU AI Act 2025 上路 mandate incident telemetry + 『AI Influence Observatory』 reporting — governance 鷹架追上 threat
- Information Research (2025) 比 LLM-based fact-checking tool 在 Facebook disability misinfo 上的不一致表現 — 仍需 operational governance
- ASIS&T 2025 Information Matters retrospective 把 LIS 定位成 governance 工作的歷史承擔者（前網際網路時代的 everyday misinformation lineage）
- Luxury 對映：brand-safety team 現在跑 detection logic — 但 luxury 比任何 vertical 都需要 long-horizon trust governance for AI brand impersonation
