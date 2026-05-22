# Anthropic 賠 15 億、Disney 告 Midjourney——LLM 跟 image-gen 在 fair use 上分流

> Anthropic Pays $1.5B While Disney Sues Midjourney: The Fair Use Split — 2026-05-22

## Hook

Bartz v Anthropic 案、法官 Alsup 2025/6/23 裁定：用合法買的書訓練 LLM 是 fair use、quintessentially transformative；但下載儲存盜版庫不是。9/5 Anthropic 同意 15 億美金和解 50 萬本盜版書、每本 $3000——美國史上最大版權和解。同時 Disney + Universal 6/11 在 CDCA 告 Midjourney 110 頁、附 Star Wars / Simpsons 角色生成截圖。差別在哪？LLM 鮮少 verbatim 重現訓練資料、image-gen 直接吐 Yoda 跟 Homer Simpson。

## Theoretical anchor

Bartz v Anthropic 法官 Alsup 裁定書 (N.D. Cal., 6/23/2025, https://www.susmangodfrey.com/wins/susman-godfrey-secures-1-5-billion-settlement-in-landmark-ai-piracy-case/)；Disney + Universal v Midjourney (CDCA 6/11/2025, https://www.cnbc.com/2025/06/11/disney-universal-midjourney-ai-copyright.html)；Lemley & Casey 'Fair Learning' (Texas Law Review, 2021) 是底層學派支援。

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | anthropic-disney-copyright-slide-01-cover.jpg | Cover — Anthropic 賠 15 億、Disney 告 Midjourney——LLM 跟 image-gen 在 fair use 上分流 |
| 2 | anthropic-disney-copyright-slide-02-why-this-matters.jpg | 同樣叫生成式 AI，法院卻開始分兩條路。對 HCI、CS、CDS 真正要緊的不是八卦，而是你的介面、記憶測試、資料 provenance，明天都可能直接變成訴訟證物。 |
| 3 | anthropic-disney-copyright-slide-03-fair-learning-anchor.jpg | 底圖先亮出來。brief 未列任何 arXiv ID；《Fair Learning》也不在 arXiv，我改抓 Texas Law Review／SSRN 的 81 頁 PDF。其 |
| 4 | anthropic-disney-copyright-slide-04-two-step-ruling.jpg | Alsup 把行為切兩刀。2025/6/23 的 Bartz 裁定讓「訓練 Claude」過 fair use，卻把 central library 另算；公開報導引述命令稱 An |
| 5 | anthropic-disney-copyright-slide-05-piracy-gets-billed.jpg | 賠的不是學習，是盜版囤書。Susman Godfrey 2025/9/25 公布：Anthropic 支付 15 億美元加利息，預估約 50 萬件作品、每件約 3000 美元；若前 |
| 6 | anthropic-disney-copyright-slide-06-characters-on-screen.jpg | 角色一出現，案型就變。Disney 與 Universal 2025/6/11 在 CDCA 提告；docket 直接顯示 Document 1「Page 1 of 110」。畫面 |
| 7 | anthropic-disney-copyright-slide-07-midjourney-defense.jpg | Midjourney 的 8 月抗辯先不要畫成既定勝負。可核實二手來源只到它主打 transformative fair use；但我沒有成功抓到該一手 filing PDF，所以 |
| 8 | anthropic-disney-copyright-slide-08-theory-lineage.jpg | 這條理論線不是 2025 才冒出來。《Fair Learning》P55–57 把核心講白：ML 多半不是為了拿表達，而是要 ideas、facts、linguistic stru |
| 9 | anthropic-disney-copyright-slide-09-what-shifted.jpg | 變的是裁判顆粒度，不再一刀切「AI fair use / AI 不 fair」。沒變的是老問題仍回到 reproduction、market harm、source legitim |
| 10 | anthropic-disney-copyright-slide-10-hci-friction.jpg | 介面不是中立外殼。當 image-gen 能穩定吐出 Yoda 或 Homer Simpson，HCI 任務就變成在 prompt、explore feed、download fl |
| 11 | anthropic-disney-copyright-slide-11-memorization-evidence.jpg | memorization 從 safety 指標升格成法庭證據。若公司想像 Anthropic 一樣主張訓練具 transformative 性，就得拿 verbatim extr |
| 12 | anthropic-disney-copyright-slide-12-provenance-politics.jpg | Critical Data Studies 要問的不是 AI 抽不抽象，而是誰有權把資料變成基礎設施。Anthropic 案把「合法取得」和「非法囤積」拆開；你的 corpus = |
| 13 | anthropic-disney-copyright-slide-13-seo-case-study.jpg | SEO 不是旁觀者。把網站合法爬下來做索引，比較像《Fair Learning》裡的 reading／search；但若團隊拿來源不明整包資料庫開練，就從『讀』跨成『持有侵權副本』 |
| 14 | anthropic-disney-copyright-slide-14-counter-evidence.jpg | 別把『LLM 很少逐字重現』當自然法。《Fair Learning》P29–31 早提醒 intermediate copying 仍可能侵權，且法定賠償最高可到每作 15 萬美元 |
| 15 | anthropic-disney-copyright-slide-15-open-questions.jpg | 真正還沒定的是市場替代。Alsup 讓訓練過關，不代表所有輸出都過關；若模型開始穩定吐出可替代原作的角色、段落或風格包，factor four 會重新翻桌。你的 benchmark |
| 16 | anthropic-disney-copyright-slide-16-method-note.jpg | 方法要攤開寫。本 deck 一手抓到的是《Fair Learning》PDF、Susman 和 SCOTUS Thaler docket；Bartz 正式命令全文與 Midjour |
| 17 | anthropic-disney-copyright-slide-17-literature-gaps.jpg | 文獻還缺中間層。《Fair Learning》主要處理『怎麼讀資料』，Disney 案逼問的是『怎麼吐角色』；真正空白是記憶測試、過濾門檻、平台展示責任怎麼接起來。LIS 能補的是 |
| 18 | anthropic-disney-copyright-slide-18-three-takeaways.jpg | 最後只留三句，字要少、拳要重。主畫面只排：訓練可辯護；盜版要賠錢；輸出越像角色，平台越危險。副標小字可補：fair use 從來不是免死金牌。 |

## Implications

- **HCI:** Image-gen 產品需要 IP-aware filter——不是道德問題、是訴訟風險
- **CS:** Memorization metric 從 LLM safety 學術指標變成 lawsuit-defense 必備證據
- **Critical Data Studies:** 誰擁有訓練資料、誰承擔風險——fair use 不是普世答案、是個案技術判斷

## Key findings

- Alsup 裁定 fair use 分兩段：訓練 OK、儲存盜版庫不 OK
- Anthropic 和解 15 億 USD / 50 萬本書 / 每本 $3000、史上最大版權和解 (2026/9/5)
- Disney v Midjourney 訴狀 110 頁、附圖證生出商標角色——CDCA 立案 2025/6/11
- Midjourney 8 月 motion to dismiss、主打 transformative fair use 抗辯
- Pamela Samuelson + Mark Lemley 學派一直主張 training 應屬 fair use、Alsup 抄這條
- 技術差異：LLM 輸出極少 verbatim 重現、image-gen 能 reproduce 可識別 IP——這是案件分流的物理原因
- Supreme Court 2026/3/2 拒 Thaler cert、純 AI 產出無 copyright——把 'AI is the author' 路線封死
