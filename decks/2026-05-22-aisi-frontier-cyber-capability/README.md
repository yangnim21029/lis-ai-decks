# 人類紅隊跑 20 小時、Claude Mythos 3 小時跑完——AISI 把 32 步攻擊鏈當尺

> UK AISI Measures Frontier Cyber: Mythos and GPT-5.5 Beat the 32-Step Test — 2026-05-22

## Hook

UK AISI 4 月公開測 Claude Mythos Preview 跟 GPT-5.5——用一個叫 The Last Ones 的 32 步企業網路攻擊腳本、從偵察到全網接管。人類紅隊估 20 小時、Mythos 跑 10 次有 3 次完成、平均 22 步；GPT-5.5 同題 10 次跑 2 次完。同一個 expert CTF 上 Opus 4.7 只有 48.6%、Mythos 衝到 68.6%、GPT-5.5 71.4%。這不是 demo，是政府測完寫上 AISI blog 的政治籌碼——他們在告訴 Anthropic 跟 OpenAI：你們的 RSP 跟不上自己的模型。

## Theoretical anchor

UK AISI 'Our evaluation of Claude Mythos Preview's cyber capabilities' (April 2026, https://www.aisi.gov.uk/blog/our-evaluation-of-claude-mythos-previews-cyber-capabilities)；同月 OpenAI GPT-5.5 evaluation；Anthropic Responsible Scaling Policy v3 (2025, https://www.anthropic.com/news/responsible-scaling-policy-v3) 把 Cyber Operations 列 provisional、ASL-4/ASL-5 仍 undefined——這就是 governance gap。

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | aisi-32-step-cyber-slide-01-cover.jpg | Cover — 人類紅隊跑 20 小時、Claude Mythos 3 小時跑完——AISI 把 32 步攻擊鏈當尺 |
| 2 | aisi-32-step-cyber-slide-02-why-this-matters.jpg | 這不是 demo，是政府拿尺量前沿模型。AISI 先在 4 月 13 日寫 Mythos，再在 4 月 30 日寫 GPT-5.5；同一把 32 步 TLO 尺上，人類估 20 小 |
| 3 | aisi-32-step-cyber-slide-03-anchor-paper-found.jpg | 先找錨點，不先信 brief。題綱未列 arXiv ID；但 AISI 在「Cyber range results」直接連到 arXiv:2603.11214〈Measuring  |
| 4 | aisi-32-step-cyber-slide-04-the-range-is-yardstick.jpg | 尺先立起來，恐慌才有刻度。AISI blog〈Cyber range results〉把 TLO 定義成 32-step corporate network attack；arXi |
| 5 | aisi-32-step-cyber-slide-05-mythos-breaks-through.jpg | Mythos 先把門撞開。AISI 4 月 13 日文〈Cyber range results〉明寫：Claude Mythos Preview 在 TLO 10 次裡 3 次全破 |
| 6 | aisi-32-step-cyber-slide-06-gpt55-catches-up.jpg | 第二家也追上了，這就不是單點神蹟。AISI 4 月 30 日文〈Cyber Range Results〉寫 GPT-5.5 在 TLO 10 次裡 2 次全破；同頁腳註又明說 Op |
| 7 | aisi-32-step-cyber-slide-07-frontier-parity-appears.jpg | 前沿 parity 出現了。AISI 4 月 30 日文〈Cyber Task Results〉寫 Expert-level pass rate：GPT-5.5 71.4%±8.0 |
| 8 | aisi-32-step-cyber-slide-08-rsp-gap-exposed.jpg | 能力有數字，治理還在留白。Anthropic RSP v3 第 1 節第 4 頁寫，最佳做法可能是由「third parties」決定安全論證是否充分；但文件本身沒有把 TLO 這 |
| 9 | aisi-32-step-cyber-slide-09-what-shifted-what-stayed.jpg | 變的是長鏈自動化，沒變的是真實世界更髒。arXiv Section 2 說 10M→100M tokens 可帶來最高 59% 增益，且未見 plateau；Section 5 又 |
| 10 | aisi-32-step-cyber-slide-10-hci-needs-interrupts.jpg | HCI 不能只顯示成功率，要顯示攻擊進度。因為 TLO 是 step-based measurement，operator 真正能介入的是卡在哪一步、用了多少 token、何時觸發 |
| 11 | aisi-32-step-cyber-slide-11-cs-benchmark-politics.jpg | CS 看到的不只是更強 benchmark，而是 benchmark 主權化。AISI 自建 95 個 narrow tasks、兩個 cyber ranges，還在 blog 說 |
| 12 | aisi-32-step-cyber-slide-12-cds-enforcement-matters.jpg | CDS 的 punchline 很簡單：文件不是治理，執行才是。Anthropic RSP v3 第 4 頁明寫需要 independent bodies、auditors、vol |
| 13 | aisi-32-step-cyber-slide-13-rust-vm-case.jpg | 別只看平均值，看一題怎麼被碾過。AISI GPT-5.5 文的 spotlight「rust_vm」寫得很狠：Crystal Peak 專家約 12 小時，GPT-5.5 用 10 |
| 14 | aisi-32-step-cyber-slide-14-counterevidence-remains.jpg | 先別喊全面失控，反證還在。AISI Mythos 文與 GPT-5.5 文都寫 Cooling Tower 沒有模型全破；arXiv Conclusion 也說最佳模型在 ICS  |
| 15 | aisi-32-step-cyber-slide-15-open-question-hours.jpg | 連『要幾小時』都在漂，這很重要。AISI blogs 對 TLO 寫 human around 20 hours；arXiv Abstract 與 Section 2 則寫 est |
| 16 | aisi-32-step-cyber-slide-16-method-note-limits.jpg | 方法註記要擺前面，不要藏腳註。arXiv Section 5 列出四個上限與四個下限：沒有 active defenders、detections not penalised、vu |
| 17 | aisi-32-step-cyber-slide-17-literature-gap.jpg | 文獻缺口不在『模型會不會更強』，而在誰有權驗。AISI 把 range paper、blog、safeguard red-team 串成公開證據鏈；OpenAI system ca |
| 18 | aisi-32-step-cyber-slide-18-three-takeaways.jpg | 先記住三句。攻擊鏈 已可 自主 串接； 進步 主要 由 推理放大。 評測 必須 看 長鏈 任務； 不只 看 CTF。 治理 若無 第三方 強制； RSP 只是 企業 宣言。 |

## Implications

- **HCI:** AI safety dashboard 要把 step-by-step attack progress 視覺化、operator 才有介入點
- **CS:** Frontier cyber eval 從學術 CTF 變成主權測試——AISI / NIST / 中國 CAICT 的 benchmark 互不相認
- **Critical Data Studies:** Governance 文件（RSP）寫得多細不重要、有沒有第三方 enforce 才重要——AISI 就是在 enforce

## Key findings

- The Last Ones (TLO) 32-step 攻擊鏈：偵察 → exploit → 橫向移動 → 全網接管，人類紅隊估時 20 小時
- Mythos Preview 10 次跑 3 次完成、平均跑到第 22 步
- GPT-5.5 10 次跑 2 次完成
- Expert CTF：Mythos 68.6% / GPT-5.5 71.4% / 一代前 Opus 4.7 48.6%——frontier parity 在跨實驗室出現
- AISI blog 原文：'execute multi-stage attacks on vulnerable networks... tasks that would take human professionals days of work'
- Anthropic RSP v3 把 cyber 留在 provisional tier、ASL-4 trigger 未定義——AISI 是用第三方數據逼補完
- 美方 US AISI 4 月同步擴大測試 DeepMind / Microsoft / xAI 未公開模型
