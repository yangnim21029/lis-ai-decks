# 對齊有理論天花板：Best-of-N 已接近極限、PPO/GRPO 還差很遠

> Theoretical Limits of Alignment: Best-of-N Approaches the Ceiling, PPO/GRPO Are Substantially Suboptimal — 2026-05-21

## Hook

在固定 KL-divergence 預算下、最大可達 reward gain 由 Jeffreys-divergence 項決定 (不是舊的 √KL bound)。實證：Best-of-N alignment 觸及理論 Pareto frontier、PPO 跟 GRPO 還有顯著差距——這是個結構性論點，說現行 RLHF 在 leave capability on the table。幾乎所有商用模型 (Claude 4.7、GPT-5、Gemini 3) 都跑 PPO/GRPO 變體；如果這篇 closed-form bound 對、那業界在花 compute approaching a frontier that BoN already touches at inference time。

## Theoretical anchor

Monteiro Paes, Mackraz, Theobald, Danieli 'Theoretical Limits of Language Model Alignment', arXiv:2605.07105 (Apple ML, May 8, 2026)；配 Huang et al. 'Transitivity Meets Cyclicity', arXiv:2605.17342 (ICML 2026 accepted, May 17, 2026)

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | alignment-theoretical-ceiling-slide-01-cover.jpg | Cover — 對齊有理論天花板：Best-of-N 已接近極限、PPO/GRPO 還差很遠 |
| 2 | alignment-theoretical-ceiling-slide-02-why-it-matters-now.jpg | 這不是調參，是上限。2605.07105 的 §3.1、§5.1 與 Fig.1 說：固定 KL 預算下，可拿到多少 reward 有理論邊界；若 BoN 已貼線，HCI/CS/C |
| 3 | alignment-theoretical-ceiling-slide-03-theoretical-anchor-core.jpg | 理論錨點：Theoretical Limits of Language Model Alignment。2605.07105 在 Eq.2.1、§3.1 Theorem 1 把 a |
| 4 | alignment-theoretical-ceiling-slide-04-jeffreys-not-sqrtkl.jpg | 舊的 √KL 直覺不夠了。2605.07105 §3.1 明寫 prior work 只有 upper bound；Theorem 1 給的是 closed-form：最優 rew |
| 5 | alignment-theoretical-ceiling-slide-05-covariance-estimator-frontier.jpg | 上限可先算，再決定要不要訓練。2605.07105 §3.2 的 Definition 1、Definition 2 與 Proposition 1/2 把界線改寫成 base m |
| 6 | alignment-theoretical-ceiling-slide-06-bon-near-frontier.jpg | Best-of-N 幾乎貼著理論線走。2605.07105 §5.1 的小節名就叫「best-of-N is almost Pareto optimal」；Fig.1 與文中明說  |
| 7 | alignment-theoretical-ceiling-slide-07-ppo-grpo-gap.jpg | PPO、GRPO 不是差一點，是結構性落後。2605.07105 §5.1「GRPO and PPO are suboptimal」寫得很直：兩者在所有測試 KL budget 都 |
| 8 | alignment-theoretical-ceiling-slide-08-proxy-hacking-ensemble.jpg | reward hacking 不是玄學，是 proxy 誤差乘上低 KL 懲罰。2605.07105 §4.1 與 Proposition 3 指出：gold 與 proxy 的  |
| 9 | alignment-theoretical-ceiling-slide-09-what-shifted-what-stayed.jpg | 變的是 benchmark，沒變的是目標。目標仍是 Eq.2.1 那種在能力保留下提高偏好 reward；但 2605.07105 把比較基準從『誰比較會訓』改成『誰離 §3.2  |
| 10 | alignment-theoretical-ceiling-slide-10-hci-implication-design.jpg | 對 HCI：別把 RLHF 當預設更好的人機對齊。若 2605.07105 §5.1 成立，產品團隊應把 BoN-at-inference 與 RLHF-at-train 放進同一 |
| 11 | alignment-theoretical-ceiling-slide-11-cs-implication-stack.jpg | 對 CS：alignment capability 可能更像 inference stack 問題，不只是 training stack 問題。2605.07105 §6 明說 e |
| 12 | alignment-theoretical-ceiling-slide-12-cds-implication-governance.jpg | 對 Critical Data Studies：治理討論第一次有『離最優多遠』的可計算語言。2605.07105 §6 把 frontier 定成 achievable limit |
| 13 | alignment-theoretical-ceiling-slide-13-two-task-case.jpg | 案例深描：不是只在單一 benchmark 成立。2605.07105 §5 用兩個任務驗證，summarization 用 Reddit TL;DR，safety 用 Beave |
| 14 | alignment-theoretical-ceiling-slide-14-companion-paper-tension.jpg | 伴讀論文不是反駁，而是把『reward 形式』這件事再往前推。2605.17342 只成功抓到 arXiv abstract，未取得章節全文；依 abstract，HRC+DSPP |
| 15 | alignment-theoretical-ceiling-slide-15-open-questions-next.jpg | 開放問題比結論更重要。2605.07105 §6 Limitations 直接點名：若目標改成 f-divergence regularization、win-rate maxim |
| 16 | alignment-theoretical-ceiling-slide-16-method-note-estimation.jpg | 方法註：這不是只靠漂亮定理。2605.07105 §5.1 說 estimator convergence 會報 95% bootstrap intervals，App.E 還做  |
| 17 | alignment-theoretical-ceiling-slide-17-literature-gap-bt.jpg | 文獻缺口其實在 reward modeling，不只在 optimizer。2605.07105 §6 與 App.C 指出 Bradley-Terry 只學相對排序，不約束 pr |
| 18 | alignment-theoretical-ceiling-slide-18-three-takeaways-close.jpg | 收尾：三個帶走句。上限 可算，別再 只信 √KL 舊式 想像 了。BoN 已 貼線，training 未必 勝過 inference 選擇。Proxy 會 駭化，ensemble  |

## Implications

- **HCI:** Product 團隊應該 test BoN-at-inference vs RLHF-at-train、不假設 RLHF 嚴格較佳
- **CS:** Inference-compute 是比 training-compute 更有效率的 alignment capability lever——re-prioritise stack
- **Critical Data Studies:** FAccT 治理討論：理論 alignment ceiling 已知、regulator 可以 reason about 『how far is this model from optimal』、不再 vibing

## Key findings

- Closed-form：optimal reward improvement = Jeffreys-divergence term、reformulated as covariance under base model (2605.07105)
- Best-of-N 實證上 track 理論 Pareto frontier on safety + summarization
- PPO 跟 GRPO 顯著低於 frontier
- Reward ensembling 理論上 mitigate reward hacking——合理化實務做法
- 提供 practical estimator computable from base model samples (no training)
- Companion HRC+DSPPO (2605.17342, ICML 2026)：把 alignment 當 time-varying game、+1.23% on RewardBench 2、44.75% length-controlled win on AlpacaEval 2.0
- 兩篇共同 question 主流『scalar reward + policy gradient』paradigm
