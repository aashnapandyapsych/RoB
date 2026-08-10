# RoB 2 Workbench

An editable, guided, browser-based implementation of the **Cochrane Risk of Bias 2 (RoB 2)** tool for individually randomized, parallel-group trials — built as a learning and working tool for early-career and independent researchers.

Everything is in a single file, **`index.html`**. Open it in any modern browser (double-click it, no server or installation needed). It also works offline, and no data ever leaves the browser.

## Features

- **Official signalling questions** from the RoB 2 version of 22 August 2019, for all five domains, including both Domain 2 variants:
  - effect of **assignment** to intervention (intention-to-treat), and
  - effect of **adhering** to intervention (per-protocol) — switchable in the study setup.
- **Editable everything** — study details, responses (Y / PY / PN / N / NI / NA), per-question support-for-judgement notes, domain judgements, justifications, and optional direction-of-bias questions.
- **Built-in analysis**:
  - the official RoB 2 mapping algorithms run live as you answer, proposing a judgement for each domain and overall, with a plain-language explanation of *why*;
  - conditional questions are automatically gated (shown/skipped) based on earlier answers, as in the official tool;
  - consistency checks flag unanswered questions, overrides without justification, missing supporting quotes, and the "some concerns in multiple domains" rule;
  - a draft risk-of-bias summary paragraph is generated from your answers, ready to edit and paste into a review.
- **Assessor stays in charge** — the algorithm output is a proposal; every judgement can be overridden, and the tool asks for a written justification when you do (as RoB 2 requires).
- **Learning mode** — per-domain explanations ("why this domain exists", common learner mistakes) and per-question "How to answer" guidance drawn from the RoB 2 guidance criteria. Toggle it off once you know the tool.
- **Export to Excel (.xlsx)** — a real Excel workbook generated entirely in the browser (no libraries, no upload) with:
  - an **Assessment** sheet: full detail — every question, response, supporting note, algorithm result, assessor judgement and justification, colour-coded;
  - a **Summary** sheet: one row per study in the same shape as the official RoB 2 Excel template's Summary tab, ready to combine across studies.
- **Save / resume** — download progress as `.json` and reopen it later; work is also autosaved to the browser's local storage.
- **Print / PDF** export for records or supervision meetings.
- Light and dark theme, keyboard-accessible controls.

## The judgement algorithms

The domain and overall mapping algorithms were transcribed from the official RoB 2 algorithm flowcharts (as implemented in the official macro-enabled Excel tool) and verified against 21 test scenarios covering the Low / Some concerns / High paths of every domain, both Domain 2 variants, and the overall mapping.

## Attribution and intended use

The RoB 2 tool is by Sterne JAC, Savović J, Page MJ, et al. *RoB 2: a revised tool for assessing risk of bias in randomised trials.* BMJ 2019;366:l4898. Official materials, the full guidance document, and the official Excel implementation are at [riskofbias.info](https://www.riskofbias.info).

This workbench is an independent educational implementation for learning and practising risk-of-bias assessment. For publication-grade systematic reviews, follow the official guidance document and your review protocol; algorithm output is always a *proposed* judgement — the assessor's reasoned judgement is final.
