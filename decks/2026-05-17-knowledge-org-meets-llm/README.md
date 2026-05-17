# 當分類法遇上 LLM：知識組織如何重新定義 RAG 的可信度

> Knowledge Organization Meets LLMs: Ontologies, GraphRAG, Authority — 2026-05-17

## Hook

分類法以前是 1876 Cutter 問題、2026 是 hallucination 問題。FalkorDB GraphRAG 在 benchmark 上 hallucination 降 90%、LLMs4OL 2025 證 LIS 學 ontology few-shot 可行。這裡是 LIS 幾百年的 knowledge organization 思考（authority control、faceted classification、controlled vocabularies）對 AI engineering 變成 operationally essential——Rose 可以拿去任何 AI master's 賣的故事。

## Theoretical anchor

LLMs4OL 2025 (Open Conference Proceedings, 'Heterogeneous LLM Methods for Ontology Learning'); Taxonomy-Driven KG Construction (ACL Findings 2025); Ontology-Based RAG (ScienceDirect 2025, S1552628325000468); RSC Digital Discovery 2026 scientific KG with open LLMs (d5dd00275c)。傳統 authority control 被 reframe 成 'who curates the ontology the LLM trusts'。

## Slides

| # | Filename | Headline / content |
|---|----------|---------------------|
| 01 | knowledge-org-llm-slide-01-cover.jpg | Cover — 當分類法遇上 LLM：知識組織如何重新定義 RAG 的可信度 |
| 2 | knowledge-org-llm-slide-02-why-now-matters.jpg | 分類法沒有過時。它只是換了故障型態。1876 Cutter 面對的是找不到書，2026 RAG 面對的是 hallucination；你的 prompt failure = LIS |
| 3 | knowledge-org-llm-slide-03-authority-control-returns.jpg | Authority control 回來了。只是名字變成 ontology governance。以 Cutter、controlled vocabularies、faceted  |
| 4 | knowledge-org-llm-slide-04-graphrag-cuts-hallucination.jpg | GraphRAG 不是加圖資料而已。是加可驗證關係。以 FalkorDB 2025 benchmark 為錨，呈現 ontology grounding 後 hallucinati |
| 5 | knowledge-org-llm-slide-05-triples-enter-retrieval.jpg | Ontology-Based RAG 把三元組塞進檢索，不只塞進知識庫。引 ScienceDirect 2025 說明 subject-predicate-object 如何成為檢 |
| 6 | knowledge-org-llm-slide-06-few-shot-ontology-learning.jpg | LLMs4OL 2025 顯示 ontology learning 已可 few-shot。重點不是模型忽然懂分類，而是 LIS 定義的類型與層級能被 prompt 編排、ense |
| 7 | knowledge-org-llm-slide-07-taxonomy-guides-retrieval.jpg | Taxonomy-guided retrieval 繞過大規模標註依賴。以 ACL Findings 2025 的 taxonomy-driven KG construction  |
| 8 | knowledge-org-llm-slide-08-kg-roi-becomes-visible.jpg | 知識圖譜不只學術漂亮，也開始有財務語言。Industry survey 2025 指向 finance／healthcare 生產 ROI 約 300–320%；這張要把 accu |
| 9 | knowledge-org-llm-slide-09-what-shifted-stayed.jpg | 變的是執行層，不變的是組織邏輯。從卡片目錄到 GraphRAG，核心仍是命名、關聯、權威、可追溯；只是 curator 位置從館員延伸到 ontology editor、RAG e |
| 10 | knowledge-org-llm-slide-10-hci-curator-interface.jpg | HCI 問題不是聊天框，而是 curator interface。結合 visual ontology editor 與 LLM suggestion workflow，讓人能審核 |
| 11 | knowledge-org-llm-slide-11-cs-needs-authority-axis.jpg | CS benchmark 少了一條 authority quality 軸。這張主張 RAG 評測不該只比 recall、latency、faithfulness，還要比 onto |
| 12 | knowledge-org-llm-slide-12-canonical-knowledge-politics.jpg | Ontology 決定誰的知識被算作 canonical。用 Berman 的批判傳統重述今日問題：不是模型偏見而已，而是類目命名、排除與授權如何前置進 RAG。你的 schema |
| 13 | knowledge-org-llm-slide-13-luxury-taxonomy-testbed.jpg | Luxury taxonomy 是理想測試場。材料、ateliers、provenance lines、真偽與維修史都需要 machine-readable ontology；以  |
| 14 | knowledge-org-llm-slide-14-counterevidence-and-limits.jpg | 不是所有場景都值得上 ontology。當知識變動快、共識弱、成本高時，結構化可能拖慢系統；這張要呈現 counter-evidence：有些 QA 任務 dense retrie |
| 15 | knowledge-org-llm-slide-15-open-research-questions.jpg | 真正難題在誰來維護與誰能修改。提出三個開放問題：ontology drift 如何量測、跨語言 authority 如何對齊、LLM suggestion 如何不覆蓋少數知識。副標 |
| 16 | knowledge-org-llm-slide-16-methods-for-evaluation.jpg | 方法上要把 LIS 與 AI evaluation 接起來。建議混合設計：task accuracy、hallucination audits、curator agreement、 |
| 17 | knowledge-org-llm-slide-17-literature-gap-map.jpg | 文獻缺口不在『有沒有知識圖譜』，而在『誰定義它可信』。總結 2025–2026 研究：工程論文重性能，LIS 可補 authority、versioning、provenance、 |
| 18 | knowledge-org-llm-slide-18-three-takeaways-only.jpg | 分類法不是舊學。Ontology 是 RAG 信任層。Authority control 不是館務遺產，而是 2026 AI 系統最缺的治理語法。副標：你的 trusted AI  |

## Implications

- **HCI:** ontology curator 的 UI — visual ontology editor + LLM suggestion 整合、CHI 等級題目
- **CS:** RAG engineering benchmark 缺 'authority quality' axis — LIS 可以貢獻 NACO-grade gold ontology 給 IR community
- **Critical Data Studies:** ontology = 誰的知識被 categorized as canonical — Berman 沒過時、是 reframed 進 RAG 治理

## Key findings

- GraphRAG + ontology grounding：hallucination 降 90% (FalkorDB benchmark 2025)
- Ontology-Based RAG 把 subject-predicate-object triple embed 進 retrieval (ScienceDirect 2025)
- LLMs4OL 2025 challenge：few-shot prompting + ensemble typing 跑 taxonomy discovery
- Production KG ROI 300-320% in finance/healthcare (industry survey 2025)
- Taxonomy-guided retrieval 繞過 large labeled-data 需求 (ACL Findings 2025)
- Open-LLM ontology generation for scientific KG (RSC Digital Discovery 2026)
- 'Authority control' 問題回歸：誰 curates LLM 信任的 ontology？
