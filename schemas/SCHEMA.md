# Public Schema

## recommendations

- `date`: recommendation date
- `arxiv_id`: arXiv identifier
- `rank`: rank within the day
- `title`
- `abstract`: paper abstract
- `tldr`: short summary generated or stored by the recommendation pipeline
- `arxiv_categories`: arXiv subject categories
- `github_links`: GitHub URLs extracted from paper metadata or content-derived signals
- `hf_links`: Hugging Face URLs extracted from paper metadata or content-derived signals
- `github_stars`: GitHub star snapshot when available
- `figures_count`: detected figure count
- `tables_count`: detected table count
- `has_insight`: whether a matching sanitized insight record exists

Removed from public release:

- `content_json_s3_key`
- `pdf_s3_key`
- `markdown_s3_key`
- `result_s3_key`
- raw `figures`
- raw `tables`
- raw nested `insight`
- `field`
- `subfield`
- `topic`
- `first_author_hindex`
- `last_author_hindex`
- `institution_score`
- `hf_rank`
- `author_h_score`
- `github_score`
- `community_score`
- `llm_review_score`
- `total_score`
- `snapshot_source`

## insights

- `arxiv_id`
- `title`
- `abstract`
- `paper_type`
- `keywords_extracted`
- `project_page`
- `github_repo`
- `demo_url`
- `problem_statement`: plain string
- `proposed_solution_overview`: plain string
- `key_contributions`: list of strings
- `limitations`: list of strings
- `future_work`
- `research_questions_or_hypotheses`: list of strings
- `datasets`
- `dataset_names`
- `evaluation_metrics`
- `evaluation_metric_names`
- `evaluation_metric_values`
- `baseline_methods`
- `baseline_method_names`
- `implementation_details`: plain string
- `citation_analysis`
- `key_references_summary`
- `experimental_results`
- `main_findings`
- `sota_comparison`
- `ablation_findings`
- `failure_cases`
- `reproducibility_info`
- `is_code_available`
- `code_url`
- `is_data_available`
- `gpu_requirement`
- `training_time`
- `user_interaction_layer`
- `personal_summary`
- `strengths`
- `weaknesses`
- `questions_and_ideas`
- `tags`
- `prerequisite_knowledge`
- `figures_count`
- `tables_count`
- `formulas_count`

Removed from public release:

- `source_chunk_contents`
- `source_chunk_indexs`
- keys containing `chunk_index`
- keys ending in `_chunk_indexs`
- figure or table discussion/context chunk provenance
