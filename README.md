*English · [Русский](README.ru.md)*

# Hi, I'm Sergey Karmanov!

**ML / Data Science — seeking a role in applied AI: document processing, data extraction, RAG**

MSc, Novosibirsk State University (Faculty of Natural Sciences, 2026). ML experience with biological and biomedical data.

[kainanasarlil@gmail.com](mailto:kainanasarlil@gmail.com) · [LinkedIn](https://linkedin.com/in/сергей-карманов-27897336b)

---

## Tech stack

### Confident
- **Python:** NumPy, pandas, matplotlib, scikit-learn
- **Data:** processing and cleaning, exploratory analysis, visualization, feature engineering
- **Document processing:** data extraction from PDF (`pdfplumber`)
- **Validation:** homology stratification (MMseqs2), data-leakage control, control experiments on shuffled labels
- **Tools & databases:** Git, SQL, Linux
- **Domain:** bioinformatics — sequences, annotations, working with biological databases (UniProt, RefSeq, KEGG, ODB)

### Learning
- **LLM / RAG:** prompt engineering, RAG pipelines, OpenAI API
- **Document processing (LLM):** extracting and structuring data from PDF, PyMuPDF
- **Backend for ML services:** FastAPI

---

## Education

### Novosibirsk State University (NSU)
- **MSc**, Faculty of Natural Sciences, bioinformatics, 2023–2026
- **Thesis:** "EC-number prediction for enzymes with operon structure using AI"

### Saratov State University (N. G. Chernyshevsky)
- **Professional retraining**, Digital Department: "Data Processing Specialist", 2022–2023
- **Final project:** "Cancer diagnostics from biomarkers using machine learning" (co-authored)

---

## Projects & experience

### Master's thesis: EC-number prediction for enzymes
Pipeline: data collection from four sources, predictions from off-the-shelf models (ProteInfer, CLEAN), a verification filter based on operon context, and stratified quality evaluation.
- Macro-F1 **0.807 → 0.887**, accuracy 0.967 → 0.982 while coverage drops 0.879 → 0.716 — the filter declines uncertain predictions instead of getting them wrong
- The largest gain is where the model is weakest: **+0.124 F1** on low-homology proteins
- Strict validation: homology stratification (MMseqs2), per-sequence leakage exclusion, a reproducible pipeline
- Data sources: ODB, RefSeq, UniProtKB, KEGG; PDF parsing (`pdfplumber`)
- Repository: [prokaryotic-ec-operon-filter](https://github.com/Kain420/prokaryotic-ec-operon-filter)

### Spotify Churn Analysis: diagnosing the absence of signal in data
A project with a negative result and a set of experiments showing the result is real, not a modeling error.
- Five control experiments: a pipeline check on data with a known signal, comparing real labels against deliberately shuffled ones, an examination of what class balancing does, calibration of the mutual-information estimate, and a demonstration of overfitting
- ROC-AUC **0.50** across all models and preprocessing strategies; the tuned model loses to a constant predictor
- Practical takeaway: how to tell "the model is undertrained" from "there is no signal in the data" before spending time on tuning
- Repository: [spotify-churn-analysis](https://github.com/Kain420/spotify-churn-analysis)

### Navi — a Telegram bot for channel navigation
- Post indexing, full-text search, and navigation through an inline interface
- Asynchronous architecture (aiohttp, Telethon, asyncio) in webhook mode, deployed on Render — a running service rather than a local computation
- Repository: [Navi](https://github.com/Kain420/Navi)

### Research Assistant | AI Centre, NSU
- Preparing and processing datasets for research
- Taking part in planning and running experiments
- Exploratory analysis of metabolomic data: searching for correlations between metabolites
- Drafting and reviewing part of a research paper — co-authorship (see Publications)

### Hackathons
**Sistema Hack: Novosibirsk** (MTS and the Sistema Charitable Foundation, hosted at NSU), 14–16 November 2025 — team of 4, CDEK case: a tool for diagnosing and preventing employee burnout. I was responsible for defining the metrics, justifying the applicability of the burnout criteria, and the ML part.

**Cookie Fest**, Novosibirsk, 29 November – 2 December 2024 — team of 2, predicting employee burnout from HR data (18,590 records). I was responsible for data preparation and exploratory analysis, and for presenting the solution.

### In progress
- **Structured data extraction from scanned documents** (vision model): per-field metrics, a rejection threshold for manual review, and search across documents

---

## Publications

**Gene networks and metabolomic screening analysis revealed specific pathways of amino acid and acylcarnitine profile alterations in blood plasma of patients with Parkinson's disease and vascular parkinsonism**

Makarova A.A., Melnikova P.M., Rogachev A.D., Demenkov P.S., Ivanisenko T.V., Predtechenskaya E.V., **Karmanov S.Yu.**, Koval V.V., Pokrovsky A.G., Lavrik I.N., Kolchanov N.A., Ivanisenko V.A. // Vavilov Journal of Genetics and Breeding. 2024. Vol. 28, no. 8, pp. 927–939.

Metabolomic screening of amino acids and acylcarnitines in blood plasma and reconstruction of regulatory gene networks to find mechanisms specific to Parkinson's disease and vascular parkinsonism. Indexed in PubMed and Scopus, open access.

[DOI: 10.18699/vjgb-24-100](https://doi.org/10.18699/vjgb-24-100)

---

## Career goal

Looking for an **ML Engineer / Data Scientist** role in applied AI. Areas I want to work in:
- solutions for **document processing and data extraction** (LLM + classical parsing)
- **RAG systems** and semantic search over documents
- building and optimizing ML pipelines
- quality control of data and model metrics
