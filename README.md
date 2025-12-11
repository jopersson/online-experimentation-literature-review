# Online Experimentation Literature Review (2000–2025)

This repository contains the curated dataset produced for our systematic literature review of research on **online experimentation**, **A/B testing**, and **causal-inference–based evaluation methods** between **2000 and 2025**. The goal is to map the academic landscape across disciplines, distinguish between *micro* and *macro* analytical viewpoints, and support future research on experimentation programs, return-aware decision-making, and organizational approaches to testing at scale.

---

## Scope and Motivation

Online experimentation research spans many fields—Computer Science, Economics, Marketing, Operations Research, Information Systems, and Statistics—yet the literatures rarely reference each other. Our objective is to:

- identify all major outlets where experimentation research appears;  
- systematically categorize papers into **micro view** (single-experiment design, estimation, causal inference) and **macro view** (program-level, decision-theoretic, organizational, return-aware);  
- highlight foundational theoretical contributions that predate online experimentation but remain influential.

This dataset underpins the descriptive analyses and figures used in our paper.

---

## Contents

### `lit_review_master.csv` (or your filename)
Each row represents one publication. Columns include:

- **title** — full paper title  
- **authors** (optional, if included)  
- **year**  
- **venue**  
- **database_searched** — e.g., INFORMS, ACM DL, IEEE Xplore  
- **field** — disciplinary classification of the *outlet*  
- **industry_first_author** — indicator for industry affiliation  
- **micro_view** — 1 if classified as micro-view  
- **macro_view** — 1 if macro-view  
- **foundational** — 1 for pre-existing or cross-cutting foundational work  
- **included_in_final** — inclusion after full-text screening  
- **url / doi**  
- **notes**

---

## Search Methodology (PRISMA-Guided)

The search procedure follows PRISMA principles (2009/2020) adapted for a cross-disciplinary, methods-focused review under strict word limits:

1. **Identification:**  
   Searches were conducted across major publisher databases:  
   INFORMS, ACM Digital Library, IEEE Xplore, AEAweb, Oxford Academic, Econometrica Society, ScienceDirect, SpringerLink, JSTOR, AIS eLibrary, Cambridge Core, SAGE Journals, JMLR/Google Scholar, Taylor & Francis, Royal Statistical Society, Project Euclid, Wiley Online Library, PNAS/Nature/Science, arXiv, SSRN.

2. **Screening:**  
   Title + abstract screened using inclusion criteria: relevance to online experimentation, A/B testing, platform experimentation, return-aware decision-making, or causal-ML methods for experimentation.

3. **Eligibility:**  
   Full-text screening for ambiguous cases. Excluded non-methodological empirical papers, domain-specific medical/biological RCTs, and non-digital experiments unless conceptually relevant.

4. **Inclusion:**  
   Final dataset compiled into structured sheet with micro/macro/foundational classifications.

A complete PRISMA flow diagram is provided in the appendix of the accompanying paper.

---

## Suggested Citation

If you use this dataset, please cite:

> **Return-Aware Platform Experimentation: 
New Directions for Research**, 2025.  
> Authors: Jacqueline Doremus, Joel Persson, Brian St. Thomas, Carlos A. Flores, Sebastian Ankargren, Mårten Schultzberg, Kyle Kretschman.  
> Dataset available at: [https://github.com/jopersson/online-experimentation-literature-review](https://github.com/jopersson/online-experimentation-literature-review/)

---

## License
MIT License (or add your preferred license).

---

## Contributions
This repository is primarily for transparency and reproducibility. If you identify missing papers or misclassifications, feel free to open an issue or submit a pull request.

---

## Contact
For questions, please contact:  
**Joel Persson** — joelpersson@spotify.com

