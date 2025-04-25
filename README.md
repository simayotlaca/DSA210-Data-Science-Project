# DSA210-Data-Science-Project
## Combining QS and THE University Rankings with CSRankings and Patent Data for a Comprehensive Academic Performance Analysis - DSA210 Project

### 1.Project Overview

This project aims to analyze global university rankings by combining QS and THE rankings while incorporating CSRankings data and industry collaboration metrics (patents, research partnerships) from WIPO/Google Patents to enrich the analysis with academic productivity and industry impact metrics. The goal is to create a more balanced and research-driven ranking system that better reflects university performance in both education, research, and industrial collaboration.

This project is planned to integrate ranking methodologies from QS World University Rankings and Times Higher Education (THE) Rankings, and then enrich this dataset with:
	1.Faculty research output metrics from CSRankings.org (academic publications and impact)
	2.Patent and industry collaboration data from WIPO/Google Patents (innovation and tech transfer metrics)
 
Given the size and complexity of these datasets, a structured data enrichment process will be applied to ensure an unbiased ranking model. This will help identify how universities perform beyond perception-based rankings by emphasizing measurable research and industry impact.

### 2.Motivation

University rankings significantly influence institutional reputation, funding, and student choices. However, the methodologies of QS and THE rankings have limitations that may lead to inconsistencies in university evaluations.
	•QS Rankings emphasize academic reputation and employer feedback but lack depth in research performance evaluation.
	•	THE Rankings consider research influence, teaching environment, and industry income but have unclear criteria for measuring industry collaboration.
	•	CSRankings provide an objective measure of faculty research output and impact through top-tier publications.
	•	Patent & Industry Collaboration Data reflect real-world economic and technological contributions, aspects largely missing from traditional rankings.

By integrating these diverse data sources, the project aims to develop a ranking methodology that prioritizes measurable research output, innovation impact, and industrial collaborations over subjective perception-based rankings.


### 3.Project Goals and Objectives

Main Goal:

To develop a comprehensive university ranking model that integrates QS, THE, CSRankings, and patent/industry collaboration data to provide a more research-driven and innovation-focused assessment of academic institutions.

Hypothesis:

The most important criterion for a university’s ranking is its success and quality in research and development.

### 4.Data Collection & Enrichment

Data Processing Steps:

To demonstrate the methodology, the following steps will be applied:

Step 1: Combining QS and THE Rankings
	•	Normalize QS and THE rankings to create a unified ranking system.
	•	Define a weighting methodology:
	•	Example: New Score=(0.5*QS Rank)+(0.5*THE Rank)
	•	Implement normalization using min-max scaling or z-score normalization.
	•	Integrating academic productivity data from CSRankings, including publication count and research areas.
	•	Examining correlations between university ranking position and research outputs.
Due to inconsistencies in university naming conventions between the QS and THE ranking websites—such as the presence of prefixes like “The”, differing abbreviations, and variations in institutional naming—it was not feasible to merge the datasets automatically using Python code. Therefore, I manually matched universities from the THE rankings to their corresponding positions in the QS ranking by carefully reviewing each entry. Although this process was time-consuming and required significant effort, I created a fully aligned dataset by hand, ensuring consistency across all entries. In this sense, the final dataset used in the project was manually constructed and curated from multiple sources.

Step 2: Visualization and Analysis
	•	Comparing consistency across QS & THE rankings—which universities show stability, and which exhibit large variations?
	•	Comparing the newly created ranking with QS & THE rankings to assess accuracy.
	•	Determining key influencing factors in university rankings, potentially using machine learning models.

These analyses will help determine whether QS & THE rankings fairly represent academic productivity and industry impact.


### 5.Analysis & Visualizations

Analysis Methods:

Correlation Analysis:
	•	Compare QS and THE rankings, identifying inconsistencies.
	•	Investigate how CSRankings data influences university positions.
	•	Analyze the impact of patent and industry data on ranking shifts.

Machine Learning:
	•	Develop a model to predict QS & THE scores.
	•	Test how factors such as faculty publication count and h-index influence rankings.

Data Visualization (Matplotlib, Seaborn, Plotly):
	•	Heatmaps to illustrate QS & THE ranking discrepancies.
	•	Scatter plots to analyze university performance by country.
	•	Relationship mapping between patents, publications, and university rankings.


### 6.Conclusion & Future Work

This project will merge QS and THE rankings with CSRankings and patent data to establish a new university ranking model that balances reputation, research productivity, and industry impact. The findings may lead to more transparent and data-driven evaluations of academic institutions.

Future Directions:
	•	Expanding the dataset to analyze historical trends in university rankings.
	•	Developing an interactive dashboard for real-time ranking comparisons.
	•	Exploring machine learning techniques to predict university ranking trends based on research and industry performance.
