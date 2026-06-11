# Online Experimentation Literature Review (2000–2025)

This repository contains the dataset used for the literature review underlying the paper *Return-Aware Platform Experimentation: New Directions for Research*:

Doremus, J., Persson, J., St. Thomas, B., Flores, C. A., Ankargren, S., Schultzberg, M., & Kretschman, K. (2025). *Return-aware platform experimentation: New directions for research*. SSRN. https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6834318

The review covers research on online experimentation, A/B testing, and related causal-inference and decision-making problems from 2000 to 2025. The dataset was created to map where this work appears across disciplines and to distinguish between two analytical viewpoints:

- **Micro view:** research focused on design, estimation, inference, or decisions within individual experiments.
- **Macro view:** research that studies experimentation as an organizational, institutional, or decision-theoretic process across many experiments.

The dataset is intended to make the review more transparent and to help researchers and practitioners find related work across fields.

---

## Contents

### `online_experimentation_SLR_2000_2025.csv`

One row per included publication. The main columns are:

- **title** — paper title
- **url** — link to the paper
- **venue** — publishing outlet, conference, industry magazine, or preprint archive
- **database_searched** — database or source where the paper was identified
- **field** — disciplinary classification of the outlet; preprints and industry magazines are coded separately
- **total_search_hits** — number of initial hits for the corresponding database search, filled in once per `database_searched` value so totals can be recovered by summing over non-missing rows
- **industry_first_author** — whether the first author was affiliated with industry or academia at the time of publication
- **micro_view** — indicator for papers classified as taking the micro view
- **macro_view** — indicator for papers classified as taking the macro view

## Search and Classification

The review follows PRISMA principles, adapted for a descriptive literature review rather than a meta-analysis.

Searches were conducted across major publisher databases, disciplinary outlets, and preprint archives, including INFORMS, ACM Digital Library, IEEE Xplore, AEAweb, Oxford Academic, ScienceDirect, SpringerLink, JSTOR, AIS eLibrary, Cambridge Core, SAGE Journals, JMLR / Google Scholar, Taylor & Francis, Royal Statistical Society, Project Euclid, Wiley Online Library, PNAS / Nature / Science, arXiv, and SSRN.

The search returned 17,039 unique records after de-duplication. After title and abstract screening, full-text checks for ambiguous cases, and application of the inclusion and exclusion criteria, 355 papers were included in the final dataset.

Included papers had to be published or publicly archived, written in English, and motivated by or addressing challenges in online experimentation, A/B testing, or related causal-inference and decision-making problems. We excluded purely empirical applications without a methodological or theoretical contribution, biomedical and laboratory experiments, standard field experiments outside the online experimentation setting, and review papers without original analytical content.

Each paper was manually coded by analytical viewpoint, field of outlet, and first-author affiliation. Coding was performed by the two first authors of the paper and reconciled through discussion.

## Main Descriptive Finding

Among the 355 included papers, about 86% take the micro view of experimentation, while about 14% take the macro view. This imbalance motivates the paper’s focus on return-aware experimentation and on research questions that arise when experimentation is viewed as a resource-allocation and rollout-decision problem across many experiments. See Appendix A of the paper for additional results and discussion.

## Suggested Citation

If you use this dataset, please cite the paper:

Doremus, J., Persson, J., St. Thomas, B., Flores, C. A., Ankargren, S., Schultzberg, M., & Kretschman, K. (2025). *Return-aware platform experimentation: New directions for research*. SSRN. https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6834318

You may also cite this repository directly if you use or modify the dataset:

Doremus, J., Persson, J., St. Thomas, B., Flores, C. A., Ankargren, S., Schultzberg, M., & Kretschman, K. (2025). *Online experimentation literature review (2000–2025)* [Dataset]. GitHub. https://github.com/jopersson/online-experimentation-literature-review/

## License

MIT License.

## Contributions

This repository is primarily intended for transparency and reuse. If you notice missing papers, broken links, or classification errors, please open an issue or submit a pull request.

## Contact

For questions, please contact:

Joel Persson  
joelpersson@spotify.com
