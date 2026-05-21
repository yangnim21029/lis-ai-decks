# 引用網路會衰老：20 年判決書揭示共引預測力半衰期

> Co-Citation Predictability Decays Over Time: A 20-Year Statute Retrieval Benchmark — 2026-05-21

## Hook

圖資 / IR / 法律科技都假設『共引相似度』是穩定信號。這篇用 396M 引用 / 101M 判決書直接量化它的衰減速率：Adamic-Adar MRR 在固定 article set 上掉 33%、temporal split 下掉 47%。Semantic drift 4.3% (embedding analysis) mechanistically explain 衰減。Civil law 比 criminal procedure 衰減快、尤其 2017 reform 後。對任何用 citation graph 做 retrieval 的系統 (Connected Papers / Semantic Scholar) 都有架構意義。

## Theoretical anchor

Ovcharov 'Temporal Decay of Co-Citation Predictability: A 20-Year Statute Retrieval Benchmark from 396M Ukrainian Court Citations', arXiv:2605.17639 (May 17, 2026)

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | co-citation-temporal-decay-slide-01-cover.jpg | Cover — 引用網路會衰老：20 年判決書揭示共引預測力半衰期 |
| 2 | co-citation-temporal-decay-slide-02-why-this-matters.jpg | 共引不是恆定訊號。對 HCI、CS、CDS 讀者，這篇把大家默認穩定的 citation similarity 拆開量化：arXiv:2605.17639〈Abstract〉直接報 |
| 3 | co-citation-temporal-decay-slide-03-anchor-paper.jpg | 理論錨點：Ovcharov，arXiv:2605.17639。Slide 要交代這不是 brief 傳話，而是依 arXiv 頁面〈Abstract〉與題名取數：396M code |
| 4 | co-citation-temporal-decay-slide-04-benchmark-scale.jpg | 先看資料尺度，再談衰減。〈Abstract〉寫明 UA-StatuteRetrieval 橫跨 2007-2026 共 20 個年度快照，來自 396M 引用與 101M 判決；畫 |
| 5 | co-citation-temporal-decay-slide-05-fixed-set-decay.jpg | 固定 article set 也會老。依 arXiv〈Abstract〉，Adamic-Adar 的 MRR 從 0.43 降到 0.29，下降 33%；這頁要強調作者用 fixe |
| 6 | co-citation-temporal-decay-slide-06-temporal-split-drop.jpg | 真正上線情境更糟。〈Abstract〉報告 train/test temporal split 下 MRR 由 0.51 掉到 0.27，衰退 47%；這頁要讓觀眾立刻連到任何靜態 |
| 7 | co-citation-temporal-decay-slide-07-domain-heterogeneity.jpg | 衰減不是平均發生。arXiv〈Abstract〉指出 criminal procedure 維持 MRR 約 0.40，civil law 則由 0.35 掉到 0.15，且與 2 |
| 8 | co-citation-temporal-decay-slide-08-drift-mechanism.jpg | 機制不只在圖上，也在語義上。〈Abstract〉寫 hub articles 超過 100K citations 較抗衰退，但 1K-10K 的 mid-frequency art |
| 9 | co-citation-temporal-decay-slide-09-what-moved.jpg | 綜合一句話：穩定的是少數樞紐法條，漂移的是實務檢索前線。這頁把〈Abstract〉三組訊號併置：固定集 33%、時間切分 47%、語義漂移 4.3%，說明『結構相似』其實被時間條件 |
| 10 | co-citation-temporal-decay-slide-10-hci-implications.jpg | HCI 意涵：相似度分數需要保存期限。若 citation recommender 沒有 freshness affordance，使用者會把過期分數當穩定真相；你的 rankin |
| 11 | co-citation-temporal-decay-slide-11-cs-implications.jpg | CS 意涵：co-citation feature 不是 train once, deploy forever。這頁把 0.51→0.27 的 temporal split 作為系 |
| 12 | co-citation-temporal-decay-slide-12-cds-implications.jpg | CDS 意涵：這不是只關於模型，而是制度與知識基礎設施共同老化。2017 reform 與 civil law 急跌放在同一畫面，提醒讀者：引用網路把司法變動沉積成資料偏移，評測也 |
| 13 | co-citation-temporal-decay-slide-13-reform-case.jpg | 案例深挖：2017 reform 之後為何 civil law 掉更快？這頁只能把它定義成 paper-grounded observation，不過須明寫目前直接抓到的是 arX |
| 14 | co-citation-temporal-decay-slide-14-counter-evidence.jpg | 反證也重要，不是所有 citation 都一起壞掉。〈Abstract〉給了兩個穩定島：criminal procedure 約 0.40、hub articles 超過 100K |
| 15 | co-citation-temporal-decay-slide-15-open-questions.jpg | 開放問題：4.3% semantic drift 足夠解釋 47% ranking drop 嗎？作者在〈Abstract〉把它作為 mechanistic explanation |
| 16 | co-citation-temporal-decay-slide-16-method-note.jpg | 方法註記：這篇最值得學的也許是研究設計。arXiv〈Abstract〉可驗證的是 leave-one-out over full bipartite citation graph、 |
| 17 | co-citation-temporal-decay-slide-17-literature-gap.jpg | 文獻缺口：我們有很多 citation-based tools，卻少有把『時間衰老』當一級評測維度。這頁可把台灣判決書或中文學術論文放進同一模板；你的 SEO 排名衰減 = LIS |
| 18 | co-citation-temporal-decay-slide-18-three-takeaways.jpg | 結尾只放三句，總長控制在 24 詞左右：共引會老。老化不均。系統必須重訓。下方小字註明量化依據來自 arXiv:2605.17639〈Abstract〉，避免把本 deck 未直取 |

## Implications

- **HCI:** Citation-based recommender 需要 freshness halflife UI affordance——告訴 user 何時 similarity score 過期
- **CS:** Co-citation feature 的 retrieval system 需要 temporal re-training schedule、static deployment 會 under-perform
- **Critical Data Studies:** Computational legal studies 拿到乾淨的 temporal IR benchmark——方法可移植到任何 longitudinal citation corpus

## Key findings

- UA-StatuteRetrieval benchmark：20 個 annual snapshots 2007-2026、released on Hugging Face (2605.17639)
- Adamic-Adar MRR 在固定 article set 上下降 33%、temporal split 下 47%
- Semantic drift 量化為 4.3% via embedding analysis——機制解釋衰減
- Criminal procedure citation：相對 resilient
- Civil law citation：2017 judicial reform 後 steeper decline
- Mid-cited article (不在 top / tail) 最易失預測力
- Single-author paper using domain-specific 20-year dataset——replicable methodology
