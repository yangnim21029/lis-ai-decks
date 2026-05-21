# 把程式碼當代理人骨架：42 作者重定義 agent infrastructure

> Code as Agent Harness: A 42-Author Reframing of Agentic AI Infrastructure — 2026-05-21

## Hook

Code 不是 agent 的輸出——是 agent 的 exoskeleton。這篇 42 作者 position paper 把整個 AutoGPT vs LangGraph 爭論抬高一階：harness (包 LLM 的 code-execution 層) 才是 agent system 的研究對象。三層：harness interface (agent ↔ environment)、harness mechanism (planning + memory)、scaling (multi-agent)。Argus 同週 paper 操作化：64 個 parallel searcher + 1 navigator 在 BrowseComp 上拿 86.2、Navigator reasoning 在 21.5K tokens 以下卻調度 64 個 searcher——context-engineering 新 SOTA。

## Theoretical anchor

Ning et al. (42 作者) 'Code as Agent Harness', arXiv:2605.18747 (May 18, 2026)；配 Zhang et al. 'Argus: Evidence Assembly for Scalable Deep Research Agents', arXiv:2605.16217 (May 15, 2026)

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | code-as-agent-harness-slide-01-cover.jpg | Cover — 把程式碼當代理人骨架：42 作者重定義 agent infrastructure |
| 2 | code-as-agent-harness-slide-02-why-harness-matters.jpg | 你以為在比 prompt，其實在比骨架。Ning et al. 2605.18747 摘要把 code 定義為 agent reasoning、acting、environment |
| 3 | code-as-agent-harness-slide-03-theoretical-anchor.jpg | 理論錨點：agent harness 是研究對象。2605.18747〈Code as Agent Harness〉不是工具清單，而是把 `2 Harness Interface` |
| 4 | code-as-agent-harness-slide-04-code-not-output.jpg | Code 不是輸出品，是外骨骼。2605.18747 摘要明說 code 已不只是 target output，而是 executable、inspectable、stateful |
| 5 | code-as-agent-harness-slide-05-three-layer-map.jpg | 三層圖不是比喻，是章節結構。依 2605.18747 的 `2 Harness Interface`、`3 Harness Mechanisms`、`4 Scaling the H |
| 6 | code-as-agent-harness-slide-06-interface-layer.jpg | 介面層：code 連接推理、行動、環境。`2.1 Code for Reasoning`、`2.2 Code for Acting`、`2.3 Code for Environme |
| 7 | code-as-agent-harness-slide-07-mechanism-layer.jpg | 機制層：可靠性不是 prompt 美學。2605.18747 `3 Harness Mechanisms` 明列 planning、memory、tool use、feedback |
| 8 | code-as-agent-harness-slide-08-scaling-layer.jpg | 擴展層：多代理的核心是 shared code artifacts。2605.18747 摘要說 multi-agent coordination、review、verificat |
| 9 | code-as-agent-harness-slide-09-argus-results.jpg | Argus 把 position paper 變成操作化證據。2605.16217 摘要：35B-A3B MoE 的 Searcher+Navigator，平均八基準單 Searc |
| 10 | code-as-agent-harness-slide-10-what-shifted.jpg | 變的是分析單位，不變的是驗證焦慮。2605.16217 `2 Argus: Agentic Evidence Assembly` 與 2605.18747 `3.4 Plan, E |
| 11 | code-as-agent-harness-slide-11-hci-window.jpg | HCI 含義：別只設計 chat surface，要設計 harness inspection。Argus `2.2 Navigator` 維護 shared evidence g |
| 12 | code-as-agent-harness-slide-12-cs-curriculum.jpg | CS 含義：agent infrastructure 應獨立成課。2605.18747 `5.2 Open Problems` 列出 evaluation beyond final |
| 13 | code-as-agent-harness-slide-13-cds-standard.jpg | CDS 含義：LLM-as-survey、LLM-as-historian 先缺的是 harness standard。2605.18747 `5.2.1 Harness-Leve |
| 14 | code-as-agent-harness-slide-14-case-study-argus.jpg | 案例：Argus 的突破不只在多工，而在壓縮。2605.16217 摘要說 Navigator reasoning context stays under 21.5K tokens |
| 15 | code-as-agent-harness-slide-15-counterevidence-limit.jpg | 反證也在文內：平行搜尋不是自動更好。2605.16217 摘要先批評 parallel rollouts 常 duplicate rather than complete，`1 I |
| 16 | code-as-agent-harness-slide-16-method-note.jpg | 方法註：這不是單一 benchmark 神話。2605.16217 `3 Search-Verify-Synthesize Agent Learning` 訓練 Navigator |
| 17 | code-as-agent-harness-slide-17-literature-gaps.jpg | 文獻缺口已被作者自己點名。2605.18747 `5.2 Open Problems` 包含 semantic verification beyond executable fee |
| 18 | code-as-agent-harness-slide-18-three-takeaways.jpg | 三句收束：研究 agent，先研究 harness。做擴展，先做共享狀態。談智能，先談驗證、調度、審計。 |

## Implications

- **HCI:** Agent UX 研究必須從『chat surface』走到『harness inspection』——user 需要 orchestration layer 的 window
- **CS:** Curriculum implication：『agent infrastructure』變成可教的 course、跟 LLM training 分開
- **Critical Data Studies:** CSS agent (LLM-as-survey、LLM-as-historian) 需要 harness standard before deployable

## Key findings

- 42 作者 position paper 把 agent 研究 organize 在『harness as the unit of analysis』(2605.18747)
- 三層：harness interface / harness mechanism (planning + memory) / scaling (multi-agent coord)
- 涵蓋：coding assistant / GUI-OS automation / embodied agent / scientific discovery / DevOps / recommendation
- Argus (2605.16217)：35B-A3B MoE backbone、Searcher + Navigator architecture
- Argus 表現：+5.5 (1 searcher) → +12.7 (8 searcher) → 86.2 (64 searcher) on BrowseComp
- Argus Navigator reasoning 在 21.5K tokens 以下 despite 64 個 parallel search——context-engineering 突破
- 兩篇同指：serious agent 是 infrastructure 問題、不是 prompting 問題
