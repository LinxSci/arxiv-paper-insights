# arXiv Paper Insights

Chinese README: [README.zh-CN.md](README.zh-CN.md)

arXiv Paper Insights is a public dataset for arXiv paper discovery, recommendations, and structured research insights.

The dataset is derived from LinxSci: `https://linxsci.com`

For any `arxiv_id`, you can open the paper reading page and view its insight page on LinxSci:

`https://linxsci.com/pdf/{arxiv_id}`

## Related Links

- LinxSci: `https://linxsci.com`
- GitHub repository: `https://github.com/LinxSci/arxiv-paper-insights`
- Hugging Face dataset page: `https://huggingface.co/datasets/LinxSci/arxiv-paper-insights`
- Kaggle dataset page: `https://www.kaggle.com/datasets/linxsci/arxiv-paper-insights`

## What Is In This GitHub Export

- project overview
- dataset schema
- lightweight sample files
- release metadata

## Update Schedule

- the dataset is updated every Monday
- each update covers recommendation papers from the previous week
- new insights are added when available in the release pipeline

## Files

- `DATASET_CARD.md`
- `LICENSE`
- `schemas/SCHEMA.md`
- `sample/recommendations.sample.jsonl`
- `sample/insights.sample.jsonl`
- `manifest.json`
- `release_notes.md`

## Field Guide

### recommendations

- `date`: recommendation date
- `arxiv_id`: arXiv paper identifier
- `rank`: rank within the recommendation list
- `title`: paper title
- `abstract`: paper abstract
- `tldr`: short summary
- `arxiv_categories`: arXiv categories
- `github_links`: extracted GitHub links
- `hf_links`: extracted Hugging Face links
- `github_stars`: GitHub stars snapshot when available
- `figures_count`: number of figures detected
- `tables_count`: number of tables detected
- `has_insight`: whether an insight record exists

### insights

- `arxiv_id`: arXiv paper identifier
- `title`: paper title
- `abstract`: paper abstract
- `paper_type`: coarse paper type label
- `keywords_extracted`: extracted keywords
- `project_page`: project page URL
- `github_repo`: GitHub repository URL
- `demo_url`: demo URL
- `problem_statement`: concise problem statement
- `proposed_solution_overview`: concise solution summary
- `key_contributions`: contribution list
- `limitations`: limitation list
- `future_work`: future work summary
- `research_questions_or_hypotheses`: research question list
- `dataset_names`: dataset names mentioned
- `evaluation_metric_names`: evaluation metric names
- `baseline_method_names`: baseline method names
- `implementation_details`: concise implementation summary
- `key_references_summary`: summarized references
- `main_findings`: main findings list
- `sota_comparison`: summary against prior work
- `ablation_findings`: ablation summaries
- `failure_cases`: failure case summaries
- `is_code_available`: code availability flag
- `code_url`: code URL when available
- `is_data_available`: data availability flag
- `gpu_requirement`: GPU requirement summary
- `training_time`: training time summary
- `personal_summary`: reader-oriented summary
- `strengths`: strengths list
- `weaknesses`: weaknesses list
- `questions_and_ideas`: open questions or ideas
- `tags`: tag list
- `prerequisite_knowledge`: prerequisite knowledge list
- `figures_count`: number of figures
- `tables_count`: number of tables
- `formulas_count`: number of formulas

## Notes

- paper full text is excluded
- raw chunk provenance is removed
- this export is intended as a lightweight project-facing release
- license: `CC BY 4.0` for derived dataset artifacts only
- original paper contents and third-party materials remain subject to their respective licenses and rights

## Citation

If you use this dataset, cite LinxSci and link back to:

`https://linxsci.com`

## Version History

- `2026-04-20`: initial public release
- Weekly cadence: every Monday we publish the previous week's recommended papers
