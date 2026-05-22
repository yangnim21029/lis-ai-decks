# 副校長叫祕書重打學生手稿再丟 Turnitin——Palo Alto 家長告校方 Title VI + Title IX

> Palo Alto Civil Rights Suit: When the AI Detector Becomes the Judge — 2026-05-23

## Hook

Kato v Palo Alto Unified、案號 5:26-cv-04078、N.D. Cal.、2026/5/5 立案。Paly 高二亞裔男生寫 Crucible essay 被 Turnitin 標 76% AI、學期成績從 A 掉到 C。訴狀說副校長 Berkson 把學生手寫的重寫稿跟期末考交給祕書打字、再丟 Turnitin 跑一次、沒通知家長。家長提 Title VI 國籍歧視 + Title IX 性別歧視——同班另一個亞裔男生被同樣處理、男生被 Turnitin 標 AI 的機率是女生的 4 到 5 倍。訴狀直接引用 Stanford Liang 2023——TOEFL essay 被 GPT detector 誤標 AI 的 false positive rate 61.22%。

## Theoretical anchor

Kato v Palo Alto Unified School District 訴狀 (N.D. Cal., 5:26-cv-04078, 2026/5/5, https://www.pacermonitor.com/public/case/64492587/Kato_v_Palo_Alto_Unified_School_District_et_al)；Liang, Yuksekgonul, Mao, Wu, Zou (2023) 'GPT detectors are biased against non-native English writers', arXiv:2304.02819；SF Standard 5/11 報導 (https://sfstandard.com/2026/05/11/ai-detection-cheating-palo-alto/)。

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | palo-alto-cheating-suit-slide-01-cover.jpg | Cover — 副校長叫祕書重打學生手稿再丟 Turnitin——Palo Alto 家長告校方 Title VI + Title IX |
| 2 | palo-alto-cheating-suit-slide-02-why-this-matters.jpg | 76% 一亮，老師就像拿到判決書。Paly 高二生一篇《Crucible》作文被打成 AI，成績從 A 掉到 C，家長改走 Title VI + Title IX。你的 detec |
| 3 | palo-alto-cheating-suit-slide-03-anchor-paper.jpg | 這副牌的理論心臟，不是作弊，而是錯標。Liang et al., arXiv:2304.02819 在 Abstract 與 Results 都直說：detectors 會把 no |
| 4 | palo-alto-cheating-suit-slide-04-case-entered.jpg | 案子已進聯邦法院，工具分數被帶進權利救濟。依 SF Standard 與 brief，Kato v. Palo Alto Unified, 5:26-cv-04078 於 2026 |
| 5 | palo-alto-cheating-suit-slide-05-score-not-verdict.jpg | 76% 不是判決，官方自己就這樣寫。Turnitin《How should I review the AI Writing report?》說分數「not meant to pro |
| 6 | palo-alto-cheating-suit-slide-06-secretary-retest.jpg | 最刺眼的不是模型，是重跑流程。依 SF Standard 與 brief，副校長 Berkson 把學生手寫重寫稿與期末考交給祕書打字後再丟 Turnitin，且未通知家長；PAC |
| 7 | palo-alto-cheating-suit-slide-07-double-disparity.jpg | 這不是單純師生爭議，訴狀把它升格成差別影響。brief 指稱另一名亞裔男生遭同樣處理，且男生被 Turnitin 標 AI 的機率是女生 4 到 5 倍；此數字本輪未從 PACER |
| 8 | palo-alto-cheating-suit-slide-08-paper-numbers.jpg | 真正該盯住的硬數字在 arXiv PDF 的 Results。〈GPT detectors exhibit bias against non-native English auth |
| 9 | palo-alto-cheating-suit-slide-09-what-changed.jpg | 變的是工具，不變的是把分類結果誤當事實。Liang 在 Introduction 與 Results 說 detectors 對 native 樣本 near-perfect，卻把 |
| 10 | palo-alto-cheating-suit-slide-10-hci-redesign.jpg | 介面別先秀 0 到 100，先秀證據鏈。這頁要畫出替代版 AI cheating report：來源、轉錄者、版本時間線、受影響句段、信賴帶與人工覆核欄位都比一個大紅 76% 更重 |
| 11 | palo-alto-cheating-suit-slide-11-cs-recalibrate.jpg | 模型若吃的是 native-dominant 語料，部署到多語教室前就該重校準。Liang 在 Results 把低 perplexity 與誤判綁在一起，且對一致誤判樣本報出 P |
| 12 | palo-alto-cheating-suit-slide-12-cds-governance.jpg | Critical Data Studies 要看的，是平台分數怎麼替機構遮責。Turnitin 官方指南明講 educator judgment 要結合其他 data points |
| 13 | palo-alto-cheating-suit-slide-13-transcription-case.jpg | 手寫稿先被祕書轉成打字稿，證據已不是原件。這頁要把 chain of custody 畫成流程圖，旁邊對照 Turnitin 2023-2025 多次修 bug 與 text fo |
| 14 | palo-alto-cheating-suit-slide-14-counterevidence-limit.jpg | 替 detector 說句公道話：它從沒保證自己能當法官。Turnitin 2024-07 更新把 1% 到 19% 直接改成 *%，理由就是 false positives 風險 |
| 15 | palo-alto-cheating-suit-slide-15-method-note.jpg | 方法上，Liang 不是大而全普查，而是高警報示範。PDF 的 Results 與後段實驗還測了 70 篇 ChatGPT 大學生申請作文、70 篇 ChatGPT 高中論文、14 |
| 16 | palo-alto-cheating-suit-slide-16-open-questions.jpg | 最該追問的，反而是論文沒測、學校卻真的做了的場景。若文本先經手寫、再由第三人轉錄、再進 detector，錯標率會不會比 61.22% 更高？這頁用大問號配版本時間線，提醒我們 d |
| 17 | palo-alto-cheating-suit-slide-17-literature-gaps.jpg | 文獻缺口很清楚：Liang 測的是 native vs non-native，沒直接測性別、神經多樣性、學科文體與懲處流程。Palo Alto 案把 Title VI、Title  |
| 18 | palo-alto-cheating-suit-slide-18-three-takeaways.jpg | 別讓分數先宣判。偵測器 先看 信賴帶 再看 證據鏈 最後 才談 懲處；偏誤 會追打 ESL 男生 與 制式 文體 作者；治理 不能 把 平台 分數 外包 成 判決。 |

## Implications

- **HCI:** AI cheating 介面該長什麼樣——不是給老師 0-100% 數字、是給 evidence trail + 統計信賴帶
- **CS:** Detection model 訓練資料偏 native English——deployment 在多語環境前要重 calibrate
- **Critical Data Studies:** 把『客觀工具』當行政 cover 是常見治理失敗模式——AI detector 是新版本

## Key findings

- 案號 5:26-cv-04078、N.D. Cal.、2026/5/5 立案
- Turnitin 給的 76% 數字、誤差帶 ±15 點——學校把它當絕對證據
- 副校長 Berkson 叫祕書重打手稿丟 Turnitin、沒通知家長就罰
- Title VI（國籍）+ Title IX（性別）雙軌、男生被 flag 機率是女生 4-5 倍
- Liang et al. 2023：TOEFL essay 被 GPT detector 誤標 AI false positive 61.22%、native 5.1%
- Turnitin 公開承認 ±15 點誤差、不該作為唯一懲處依據——學校仍照用
- AI detector 對 ESL / neurodivergent / formal academic writing 系統性高估 AI 機率——這是統計分類器的根本限制
