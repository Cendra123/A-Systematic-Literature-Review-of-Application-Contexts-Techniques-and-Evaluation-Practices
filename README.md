# Counselling Dialogue Systems: A Systematic Literature Review of Application Contexts, Techniques, and Evaluation Practices

Supplementary data for the systematic literature review (SLR) by **Cendra Devayana Putra, Hei-Chia Wang, Berliana Devianti Putri, and Bartolomeus Priya Perkasa Utama Widada**.

Counselling dialogue systems (CDSs) are conversational agents that help people explore personal problems, regulate emotions or make decisions. This repository contains the full screening log, eligibility decisions, coding and data-extraction sheets behind the review, so that every number in the paper can be traced back to individual records.

## Research questions

| RQ | Question |
|---|---|
| RQ1 | In which disciplines and application contexts have CDSs been studied, and how has the field developed over time? |
| RQ2 | Which dialogue goals, techniques and interaction modalities are used to build CDSs? |
| RQ3 | How are CDSs evaluated, and which metrics are used? |
| RQ4 | Which challenges remain open, and what research directions follow from them? |

## Method in brief

- **Guideline:** PRISMA 2020; narrative synthesis and vote counting following SWiM (Synthesis Without Meta-analysis).
- **Databases (7):** Scopus, Web of Science, PubMed, IEEE Xplore, ACM Digital Library, ERIC, ACL Anthology.
- **Period:** 2012–2026 (searched October 2026); English-language journal and conference papers.
- **Query:** `#1 AND #2` in title, abstract and keywords
  - **#1 Dialogue system:** "dialog\* system\*" OR "dialog\* agent\*" OR chatbot\* OR "chat bot\*" OR "conversational agent\*" OR "conversational AI" OR "virtual assistant\*" OR "virtual agent\*" OR "relational agent\*" OR "companion AI" OR "large language model\*" OR LLM OR ChatGPT OR "generative AI" …
  - **#2 Counselling / mental health:** counsel\* OR psychotherap\* OR "motivational interviewing" OR "cognitive behavio\* therap\*" OR "therapeutic alliance" OR "career guidance" OR "peer support" OR "emotional support" OR "mental health" OR depress\* OR anxiety OR stress OR suicid\* OR loneliness …
  - The full query is given in Table 3 of the manuscript.
- **Two-tier design:**
  - **Level-1 map** (IC5–IC8): user evaluations of purpose-built, core CDSs grounded in a named counselling approach. Used for RQ1 and the evaluation mapping.
  - **Level-2 synthesis** (IC5–IC10): studies that tested a CDS as an intervention, with outcome measures and a comparator or control. Used for RQ2–RQ4.
- **Protocol amendment:** IC5–IC10 were added after title/abstract screening and before full-text assessment (19–20 October 2026), and were applied uniformly to all core reports.
- **Quality appraisal:** Mixed Methods Appraisal Tool (MMAT 2018) for the Level-2 studies.

## PRISMA flow

| Stage | n |
|---|---:|
| Records identified (7 databases) | 20,130 |
| Duplicates removed (normalised title + first author) | 7,526 |
| Records screened (title/abstract) | 12,604 |
| Records excluded (rules 1,980; reading 7,738) | 9,718 |
| Reports sought for retrieval (core 1,832; adjacent 1,054) | 2,886 |
| Reports not retrieved | 319 |
| Reports assessed in full text | 2,567 |
| Excluded IC5 — adjacent, not a core CDS | 925 |
| Core CDS reports | 1,642 |
| Excluded IC6 — no purpose-built system | 198 |
| Excluded IC7 — no human end users | 801 |
| Excluded IC8 — no named counselling approach | 306 |
| Duplicate records | 2 |
| **Level-1 map** (reports / studies) | **335 / 333** |
| Excluded IC9 — no intervention-outcome evaluation (kept in Level-1) | 142 |
| Excluded IC10 — no comparator/control (kept in Level-1) | 76 |
| **Level-2 synthesis** (studies / reports) | **115 / 117** |

## Repository contents

The files are listed in the order of the review pipeline.

| File | Stage | Main sheets |
|---|---|---|
| `2026_10_16_Screening_TitleAbstract.xlsx` | Identification and title/abstract screening | `Summary` (database counts, overlap, PRISMA identification), `All_records` (20,130 raw records), `Unique_records` (12,604 de-duplicated records with abstracts, open-access status and screening decisions), `Possible_duplicates`, `Screening_codes`, `Included_for_RQs` (2,886 included records with keyword-based RQ coding), `RQ_overview`, `Reviews_for_Table1` (415 reviews used for the related-work comparison) |
| `2026_10_19_Screening_FullText_Retrieval.xlsx` | Full-text retrieval | All sheets above plus `Missing_full_text` (319 unretrieved reports, with reasons) and `PDF_check` (file-name and duplicate checks of retrieved PDFs) |
| `2026_10_20_Eligibility_FinalSet.xlsx` | Eligibility, mapping and extraction | `PRISMA` (flow with live formulas and the amended criteria), `Eligibility_core` (decision for all 1,642 core reports), `Level1_map` (335 coded reports), `Final_set_extraction` (structured extraction for the 115 Level-2 studies), `Trends_RQ1`, `Map_summary`, `Codes` |
| `Table A1 Characteristics of the 115 studies included in the Level-2 synthesis.xlsx` | Manuscript appendix | Study, system, context and population, counselling approach, technique and modality, design (N) and comparator |

PDFs of the included papers are not distributed here because of publisher copyright. Each record has a DOI link instead.

## Coding scheme

**Five-dimension coding framework:** application context · dialogue goal · technique family · modality · evaluation approach.

**Title/abstract screening codes** (`Screening_codes`)

| Code | Meaning |
|---|---|
| I / IA | Include: core / adjacent CDS study |
| X0 | Excluded by rules (metadata or unambiguous keywords) |
| X1–X6 | Excluded under IC3: no dialogue system; no counselling concept; detection only; general health Q&A; education/tutoring; customer or public service |
| X7–X9 | Excluded under EC2/EC4: attitude survey without a system; review/commentary/protocol; unrelated to the RQs |

**Full-text eligibility codes** (`Codes`)

| Code | Meaning |
|---|---|
| I | Included in the Level-2 synthesis |
| N6 / N7 / N8 | Excluded under IC6 / IC7 / IC8 |
| N9 / N10 | Excluded under IC9 / IC10 (kept in the Level-1 map) |
| DUP:Uxxxxx | Duplicate of another record |
| LINK:Uxxxxx | Secondary report of an included study |

**Result codes (Level-2):** *Favours CDS* · *Mixed* · *No difference* · *Feasibility only*.

Every record has a stable `Unique ID` (U00001–U12604) that links all workbooks.

## Key findings

- 71% of the mapped evaluations appeared from 2023 onwards.
- CBT was the dominant counselling approach (44%) and text the dominant modality (63%). Generative LLMs featured in 47% of the systems evaluated since 2023.
- Only about a third of the mapped evaluations were controlled.
- Of the 115 controlled studies, 59% favoured the CDS on the primary outcome, 23% had mixed results, 11% found no difference and 6% reported feasibility only.
- Follow-up beyond the intervention was rare (17%), and safety was measured in only 5% of studies.

## Limitations of the dataset

- APA PsycInfo and grey literature were not searched.
- 319 reports (11.1%) could not be retrieved in full text.
- Level-1 codes for technique and modality were supported by keyword rules on the full text and should be read as approximate.

## Citation

If you use this dataset, please cite the article (citation details will be added on publication):

> Putra, C. D., Wang, H.-C., Putri, B. D., & Widada, B. P. P. U. (2026). Counselling dialogue systems: A systematic literature review of application contexts, techniques, and evaluation practices. 

## Contact

Cendra Devayana Putra, Department of Information Systems, Universitas Negeri Surabaya, Indonesia. Email: putracendra@unesa.ac.id · ORCID [0000-0002-5692-9762](https://orcid.org/0000-0002-5692-9762)

## License

Released under the [MIT License](LICENSE).
