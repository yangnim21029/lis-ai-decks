# LLM 不懂消費者：頂尖模型只能對中 47.8% 真實反應

> ConsumerSimBench: Frontier LLMs Reconstruct Less Than Half of Real Consumer Reactions — 2026-05-21

## Hook

業界正在用 LLM 跑 AI focus group / synthetic respondent / pre-test ad copy。這篇 1,553 個真實中文話題 / 23,122 條 rule-audited 標準的 benchmark 直接打臉那個 workflow——最強 frontier 模型 (Gemini-3.1-Pro) 也只覆蓋 47.8% 真實 reaction criteria。對行銷 / luxury research 關鍵：不能用一個只懂一半的模擬器做策略決策。Multi-agent pipeline 只把分數從 32.9% 拉到 37.6%——這不是 prompt engineering 能補的。Reasoning benchmark 表現跟 consumer simulation 是 orthogonal 兩條軸。

## Theoretical anchor

Wang, Li, Lin 'Can LLMs Think Like Consumers? Benchmarking Crowd-Level Reaction Reconstruction with ConsumerSimBench', arXiv:2605.17079 (May 16, 2026)

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | consumer-sim-bench-slide-01-cover.jpg | Cover — LLM 不懂消費者：頂尖模型只能對中 47.8% 真實反應 |
| 2 | consumer-sim-bench-slide-02-why-it-matters.jpg | 別再把 LLM 當現成焦點團體。摘要與§1開宗明義：業界正用模型 pre-test 行銷訊息，但最強系統也只重建 47.8% 真實反應。你的 synthetic responden |
| 3 | consumer-sim-bench-slide-03-theoretical-anchor.jpg | 理論錨點不是 persona，而是 crowd-level reaction reconstruction。依 §1、§2 Table 1，這篇把 consumer simulat |
| 4 | consumer-sim-bench-slide-04-benchmark-scale.jpg | 規模先把門檻拉高。摘要、§1 與 Figure 1 寫明：1,553 個真實中文話題、23,122 條 atomic rule-audited criteria、4 個 react |
| 5 | consumer-sim-bench-slide-05-auditable-eval.jpg | 方法學亮點在評估，不在 prompt。摘要、§5.3、§1 contribution 都給數字：把整體打分拆成逐點 yes-no 後，三評審一致率 65.8% 升到 92.1%，且 |
| 6 | consumer-sim-bench-slide-06-frontier-gap.jpg | 最強模型也只懂一半不到。摘要、§1、§7 都重複同一結論：Gemini-3.1-Pro 僅覆蓋 47.8%；§1 同列 GPT-5.2 為 35.8%、Claude-Opus-4. |
| 7 | consumer-sim-bench-slide-07-prompting-limits.jpg | 這不是 prompt engineering 可以補平的坑。摘要與§5.2寫明 direct ConsumerSCF prompting 反而降分；§1 contribution  |
| 8 | consumer-sim-bench-slide-08-asymmetric-failure.jpg | 模型會演情緒，卻抓不到群眾真正咬哪裡。§4.3標題就叫 The Asymmetric Failure: Tone without Target；§7再寫一次 failure is  |
| 9 | consumer-sim-bench-slide-09-what-shifted.jpg | 變的是評估單位，不變的是能力缺口。從 §2 Table 1 到 §7，作者把『像不像人』從單一 persona 改成群體反應重建；但 frontier 模型仍遠離 reliable |
| 10 | consumer-sim-bench-slide-10-hci-implication.jpg | 對 HCI，不該再只輸出一個會說話的 persona。根據摘要、§7 的 coverage framing，工具介面應分 reaction family 回報校準置信與盲區；你的  |
| 11 | consumer-sim-bench-slide-11-cs-implication.jpg | 對 CS，缺的是 training signal，不只是 scaffold。§7說 closing the gap likely requires more than prompt |
| 12 | consumer-sim-bench-slide-12-cds-implication.jpg | 對 Critical Data Studies，這篇把 AI focus group 從話術變成可問責主張。§2 Table 1 強調 auditable eval，§6提醒 de |
| 13 | consumer-sim-bench-slide-13-case-study.jpg | 次級深描看 Appendix K。作者用 iPhone 17 hands-on 個案做 per-criterion audit，重點不是文風像不像網友，而是哪個 trigger 沒 |
| 14 | consumer-sim-bench-slide-14-counter-evidence.jpg | 反證不是模型全爛，而是強弱排序改寫。§1 與§7都承認模型能 sound consumer-like、能表演 emotion；§4.3則說問題在 tone without targ |
| 15 | consumer-sim-bench-slide-15-open-questions.jpg | 真正的開放問題在外推性。Appendix F 列出平台代表性、時間污染、endpoint coverage 等限制；§6也說高分仍需放回 platform 與 governance |
| 16 | consumer-sim-bench-slide-16-method-note.jpg | 方法註記要講清楚中文脈絡。§1 指 RedNote 是 high-context consumer discourse；摘要與 Figure 1 都顯示 benchmark 立基中 |
| 17 | consumer-sim-bench-slide-17-literature-gap.jpg | 文獻缺口在 benchmark family 錯位。依 §2 Table 1，ToM、CTR、persona simulation 各抓到一部分，但只有 ConsumerSimBe |
| 18 | consumer-sim-bench-slide-18-three-takeaways.jpg | 收尾只放三行，每行八詞內。第一行：最強模型仍未及半。第二行：可審計評估比華麗 prompt 更重要。第三行：別拿半懂消費者的模擬器，替真實受眾做策略決策。 |

## Implications

- **HCI:** Synthetic-user research tool 必須 surface per-reaction-category calibrated confidence interval、不是單一 persona 輸出
- **CS:** 需要新 training signal——現行 RLHF preference data 不教 crowd-level reaction distribution
- **Critical Data Studies:** Computational marketing / CSS 終於能 benchmark 『AI focus group』的承諾、不再 vibing

## Key findings

- 1,553 個真實中文社群話題、23,122 atomic rule-audited 標準、4 reaction family (2605.17079)
- Gemini-3.1-Pro：47.8% 覆蓋真實 reaction criteria (top 模型)
- GPT-5.2 跟 Claude-4.6 落後 despite strong 技術 benchmark
- Pointwise (yes/no) 評估把 judge agreement 從 65.8% 拉到 92.1%——方法學貢獻
- Multi-agent pipeline 32.9% → 37.6%——marginal、不是 transformative
- Reasoning benchmark 表現 NOT predict consumer simulation 表現——orthogonal 兩軸
- 中文 context 非平凡——多數 consumer-sim 工作只跑英文
