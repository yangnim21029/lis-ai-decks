# DeepSeek V4 換 Huawei 晶片、Kimi 開源拿 SWE-Bench 第一——中國 LLM 一個月把成本曲線踩平

> DeepSeek V4, Kimi K2.6, Qwen 3.7: China's Open-Weight SOTA in One Month — 2026-05-22

## Hook

4 月 20 日 Kimi K2.6 釋出、SWE-Bench Pro 58.6 開源第一、贏過部分閉源點。4 月 24 日 DeepSeek V4 上線、1.6T 參數跑在 Huawei Ascend 950PR、kernel 不寫 CUDA、改用 TileLang DSL、V4-Pro $3.48/M tokens——把 token 價打到 OpenAI 的零頭。5 月 20 日 Qwen 3.7-Max 預覽、Arena-Hard 90.5 領跑。三家在一個月內把開源 SOTA 拉到 GPT-5.5 隔壁——但 weights 全在中國。

## Theoretical anchor

Kimi K2.6 release (https://www.deeplearning.ai/the-batch/kimi-k2-6-matches-open-qwen3-6-max-anddeepseek-v4-falls-just-behind-top-closed-models)；DeepSeek V4 technical report (Fortune 4/24, https://fortune.com/2026/04/24/deepseek-v4-ai-model-price-performance-china-open-source/) + ChinaTalk 報導；Qwen 3.7-Max announcement (Alibaba Cloud 5/20)；Artificial Analysis intelligence index (https://artificialanalysis.ai/articles/deepseek-is-back-among-the-leading-open-weights-models-with-v4-pro-and-v4-flash)。

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | china-opensource-trio-slide-01-cover.jpg | Cover — DeepSeek V4 換 Huawei 晶片、Kimi 開源拿 SWE-Bench 第一——中國 LLM 一個月把成本曲線踩平 |
| 2 | china-opensource-trio-slide-02-why-care-now.jpg | 一個月，三次前線跳價。4/20 Kimi K2.6、4/24 DeepSeek V4、5/21 Qwen3.7-Max 接力把開放權重推到 frontier 旁邊；你的 token |
| 3 | china-opensource-trio-slide-03-anchor-and-method.jpg | 先講方法，再講神話。topic brief 的 theoretical_anchor 沒列任何 arXiv ID；本 deck 因此以 DeepSeek V4 PDF《Abstra |
| 4 | china-opensource-trio-slide-04-kimi-coding-lead.jpg | Kimi 先把開源 coding 排到第一。Kimi 官博《Benchmark Table》列 SWE-Bench Pro 58.6，高於 GPT-5.4 的 57.7；Artif |
| 5 | china-opensource-trio-slide-05-deepseek-paper-numbers.jpg | DeepSeek 不是只大，是把長上下文做成可用。V4 技術報告《Abstract》寫 V4-Pro 1.6T / 49B active、1M context、32T pretra |
| 6 | china-opensource-trio-slide-06-tilelang-ascend-shift.jpg | 換 kernel，不只換卡。技術報告§3.2 就叫「Flexible and Efficient Kernel Development with TileLang」；§3.1 又寫 |
| 7 | china-opensource-trio-slide-07-price-floor-drop.jpg | 價格線被踩扁。Artificial Analysis 2026-04-24 列 V4-Pro 為 $1.74 / $3.48 每百萬 input / output tokens，V |
| 8 | china-opensource-trio-slide-08-qwen-agent-run.jpg | Qwen 把 agent 長跑變成展示場。官方《Qwen3.7: The Agent Frontier》寫 SWE-Pro 60.6、TerminalBench 69.7、GPQA |
| 9 | china-opensource-trio-slide-09-what-shifted-stayed.jpg | 變的是 bottleneck，不變的是 scale。這一輪不只比參數，還比 harness、kernel、工具鏈與定價；但領先者仍靠巨量訓練與封閉基礎設施。開放的是權重，不是地緣條 |
| 10 | china-opensource-trio-slide-10-hci-design-space.jpg | 對 HCI，延遲與成本不再先卡死 UX。當 V4-Flash output 來到 $0.28、Kimi 與 Qwen 可連續跑上千次工具呼叫，介面可從一次問答改成長流程協作；你的  |
| 11 | china-opensource-trio-slide-11-cs-stack-war.jpg | 對 CS，真正換的是 stack。DeepSeek 報告把§3.1 EP、§3.2 TileLang、§3.5 KV cache 一起公開，說明模型競爭已下沉到 kernel 與  |
| 12 | china-opensource-trio-slide-12-cds-weight-sovereignty.jpg | 對 Critical Data Studies，問題是主權不是 benchmark。誰持有 weights、誰供應晶片、誰能 day-zero adaptation，決定誰能複現、 |
| 13 | china-opensource-trio-slide-13-rose-workflow-case.jpg | 把話拉回你的 workflow。若圖資檢索、分類、摘要改由 V4-Flash 跑量，Artificial Analysis 列 output 價格僅 $0.28 / 1M toke |
| 14 | china-opensource-trio-slide-14-counterevidence-cost-curve.jpg | 別太快喊開源勝利。Artificial Analysis 同篇也寫 V4-Pro 跑完整 Intelligence Index 要 $1,071，且輸出 190M tokens；A |
| 15 | china-opensource-trio-slide-15-ip-politics-risk.jpg | 政治噪音不是外部雜訊。Tom's Hardware 2026-04-26 引 Reuters 與白宮 memo，寫美方把指控升級到「industrial-scale」 distil |
| 16 | china-opensource-trio-slide-16-method-source-note.jpg | 方法註記要寫在檯面上。brief 的 theoretical_anchor 沒有 arXiv ID，Kimi K2.6 與 Qwen3.7 也未提供可抓取 arXiv 技術報告；因 |
| 17 | china-opensource-trio-slide-17-literature-method-gaps.jpg | 文獻缺口很明確：缺獨立 cross-harness replication、缺成本到任務完成率的公開面板，也缺「weights 在誰的 jurisdiction」對研究再現性的實證 |
| 18 | china-opensource-trio-slide-18-three-closing-takeaways.jpg | 三句帶走。權重 留在 中國 成本 壓平 曲線 Stack 下沉 到 kernel 開源 逼近 前沿 可重現性 被 主權 鎖住 產品 空間 擴大 治理 壓力 同步 升高 |

## Implications

- **HCI:** Latency / cost 不再是 LLM application UX 的硬限制——design space 跟著膨脹
- **CS:** Stack-level competition：CUDA → TileLang 不只是換 framework、是換整個 ML 軍備
- **Critical Data Studies:** 誰的 weights 在誰的 jurisdiction——research replicability 跟著主權壁壘分化

## Key findings

- Kimi K2.6 SWE-Bench Pro 58.6——首個開源贏部分閉源、Artificial Analysis intelligence index 54
- DeepSeek V4 1.6T 參數、跑 Huawei Ascend 950PR、kernel 用 TileLang 取代 CUDA
- DeepSeek V4-Pro $3.48 / 1M tokens——比 GPT-5.5 便宜一個 order of magnitude
- Qwen 3.7-Max Arena-Hard 90.5、MMLU-Pro 81.2——超 DeepSeek V3.2 跟 Claude Sonnet 4.6
- DeepSeek + Huawei 宣告 'day zero adaptation'——US 出口管制下 import substitution 成功
- Tom's Hardware：美方政府升級對 DeepSeek 的 IP 偷竊指控、跟 AI race 政治掛勾
- Rose 直接受益：圖資檢索/分類/摘要 workflow 成本曲線被踩平、$0.28/M tokens 入手
