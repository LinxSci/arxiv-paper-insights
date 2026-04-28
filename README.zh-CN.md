# arXiv Paper Insights

arXiv Paper Insights 是一个面向 arXiv 论文发现、推荐与结构化洞察的公开数据集。

数据来源平台为 LinxSci：`https://linxsci.com`

对于任意一个 `arxiv_id`，都可以直接访问 LinxSci 上的论文阅读与 insights 页面：

`https://linxsci.com/pdf/{arxiv_id}`

## 相关链接

- LinxSci：`https://linxsci.com`
- GitHub 仓库：`https://github.com/LinxSci/arxiv-paper-insights`
- Hugging Face 数据集页面：`https://huggingface.co/datasets/LinxSci/arxiv-paper-insights`
- Kaggle 数据集页面：`https://www.kaggle.com/datasets/linxsci/arxiv-paper-insights`

## 这个 GitHub 导出包包含什么

- 项目说明
- 数据集 schema
- 轻量 sample 文件
- release 元数据

## 更新节奏

- 数据集会在每周一更新
- 每次更新覆盖上一周推荐出来的论文
- 如 release 流程中已有对应 insights，也会一并纳入更新

## 文件说明

- `DATASET_CARD.md`
- `LICENSE`
- `schemas/SCHEMA.md`
- `sample/recommendations.sample.jsonl`
- `sample/insights.sample.jsonl`
- `manifest.json`
- `release_notes.md`

## 字段详解

### recommendations

- `date`：推荐日期
- `arxiv_id`：arXiv 论文编号
- `rank`：在推荐列表中的排序
- `title`：论文标题
- `abstract`：论文摘要
- `tldr`：简短总结
- `arxiv_categories`：arXiv 分类
- `github_links`：提取出的 GitHub 链接
- `hf_links`：提取出的 Hugging Face 链接
- `github_stars`：GitHub stars 快照
- `figures_count`：检测到的图片数量
- `tables_count`：检测到的表格数量
- `has_insight`：是否存在对应的 insight 记录

### insights

- `arxiv_id`：arXiv 论文编号
- `title`：论文标题
- `abstract`：论文摘要
- `paper_type`：论文类型标签
- `keywords_extracted`：提取出的关键词
- `project_page`：项目主页链接
- `github_repo`：GitHub 仓库链接
- `demo_url`：演示链接
- `problem_statement`：问题定义
- `proposed_solution_overview`：解决方案概述
- `key_contributions`：核心贡献列表
- `limitations`：局限性列表
- `future_work`：未来工作总结
- `research_questions_or_hypotheses`：研究问题列表
- `dataset_names`：文中涉及的数据集名称
- `evaluation_metric_names`：评测指标名称
- `baseline_method_names`：对比基线方法名称
- `implementation_details`：实现细节概述
- `key_references_summary`：关键引用摘要
- `main_findings`：主要发现列表
- `sota_comparison`：与已有方法对比总结
- `ablation_findings`：消融实验总结
- `failure_cases`：失败案例总结
- `is_code_available`：是否提供代码
- `code_url`：代码链接
- `is_data_available`：是否提供数据
- `gpu_requirement`：GPU 需求说明
- `training_time`：训练时间说明
- `personal_summary`：面向读者的总结
- `strengths`：优点列表
- `weaknesses`：缺点列表
- `questions_and_ideas`：问题与想法
- `tags`：标签列表
- `prerequisite_knowledge`：前置知识列表
- `figures_count`：图片数量
- `tables_count`：表格数量
- `formulas_count`：公式数量

## 说明

- 不包含论文全文
- 已去除原始 chunk provenance
- 这个 GitHub 导出包更适合作为项目展示页和轻量样例
- 许可协议：`CC BY 4.0`，但仅适用于本项目生成和整理的派生数据
- 原始论文内容及第三方来源材料仍受其各自版权和许可约束

## 引用方式

如果你使用这个数据集，请引用 LinxSci 并回链：

`https://linxsci.com`

## 版本记录

- `2026-04-27`：更新
- `2026-04-20`：首次公开发布
- 周期说明：每周一发布上一周推荐论文的更新
