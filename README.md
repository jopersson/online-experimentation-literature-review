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

### `online_experimentation_SLR_2000_2025.csv`
One row per publication. Columns are (in order):

total_search_hits	industry_1st_author	micro_view	macro_view												

- **title** — full paper title
- **url** — link to paper
- **venue** - publshing outlet (journal, conference proceedings, industry magazine, or preprint archive)
- **database_searched** — e.g., INFORMS, ACM DL, IEEE Xplore  
- **field** — disciplinary classification of the *outlet* (preprints are labelled "preprint", and indsutry magazines are labelled "industry") \
- **total_search_hits** - the number of initial hits per search, filled out only for one row per unique value of database_searched to yield correct summation over rows to total hits
- **industry_first_author** — indicator for industry affiliation of first author (industry or academia)
- **micro_view** — 1 if classified as micro-view  
- **macro_view** — 1 if macro-view  

---

## Search Methodology (PRISMA-Guided)

The search procedure follows PRISMA principles adapted for a cross-disciplinary, methods-focused review under strict word limits:

1. **Identification:**  
   Searches were conducted across major publisher databases:  
   INFORMS, ACM Digital Library, IEEE Xplore, AEAweb, Oxford Academic, Econometrica Society, ScienceDirect, SpringerLink, JSTOR, AIS eLibrary, Cambridge Core, SAGE Journals, JMLR/Google Scholar, Taylor & Francis, Royal Statistical Society, Project Euclid, Wiley Online Library, PNAS/Nature/Science, arXiv, SSRN.

2. **Screening:**  
   Title + abstract screened using inclusion and exclusion criteria (see below) relevance to online experimentation, A/B testing, and related research.

4. **Inclusion:**  
   Our inclusion criteria were:
   -- Published or publicly archived (journal, conference, practitioners’ magazine, or preprint).
   -- Motivated by or addressing challenges in online experimentation, A/B testing, or related causal-inference and decision-making problems.
   -- Could be classified into the micro or macro view on experimentation.
   -- Written in English.
   
  If ambiguous, exclusion criteria were:
  -- Purely empirical applications lacking methodological or theoretical contribution.
  -- Biomedical, laboratory, simulation, or actual field-experiments (e.g., in development economics).
  -- Review papers without original analytical or methodological content.

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

