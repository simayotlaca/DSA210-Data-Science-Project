# DSA210-Data-Science-Project
## Combining QS and THE University Rankings with CSRankings and Patent Data for a Comprehensive Academic Performance Analysis - DSA210 Project

### 1.Project Overview

This study investigates potential regional biases in global university rankings. It integrates QS and THE rankings with objective institutional features such as research productivity (CSRankings), innovation output (WIPO/Google Patents), and institutional metadata (ownership, age, location). The central hypothesis is that university rankings, rather than being purely performance-based, are influenced by geopolitical prestige, leading to systematic underrepresentation of universities from regions such as Asia.

Machine learning techniques are used to assess the influence of region on ranking scores and to determine whether objective performance indicators can accurately predict ranking positions and institutional classification.

This project is planned to integrate ranking methodologies from QS World University Rankings and Times Higher Education (THE) Rankings, and then enrich this dataset with:
	1.Faculty research output metrics from CSRankings.org (academic publications and impact)
	2.Patent and industry collaboration data from WIPO/Google Patents (innovation and tech transfer metrics)
 
Given the size and complexity of these datasets, a structured data enrichment process will be applied to ensure an unbiased ranking model. This will help identify how universities perform beyond perception-based rankings by emphasizing measurable research and industry impact.

##  Motivation

University rankings play a pivotal role in shaping **institutional reputation**, influencing **funding decisions**, and guiding **student preferences** across the globe. However, the methodologies behind widely recognized ranking systems—such as **QS** and **Times Higher Education (THE)**—raise critical concerns about **objectivity** and **regional fairness**.

### Methodological Limitations

- **QS Rankings** emphasize academic reputation and employer feedback, but they lack depth in assessing **research performance** through measurable metrics.
- **THE Rankings** include research influence, teaching environment, and industry income; however, they apply **unclear criteria** for evaluating **industry collaboration**, which reduces transparency.
- **CSRankings** provide an **objective assessment** of faculty research output based on top-tier conference and journal publications.
- **Patent & Industry Collaboration Data** reflect a university's **real-world innovation** and **technological contributions**, aspects that are largely **missing** from conventional ranking models.

###  The Issue of Regional Prestige Bias

Methodologies relying on **subjective surveys** are vulnerable to **regional prestige bias**—favoring institutions located in politically or economically dominant regions such as **Europe and North America**, while undervaluing high-performing universities in **Asia** and other emerging regions.

Despite their significant contributions to research and innovation, many top-tier institutions in Asia receive **lower-than-expected rankings**, suggesting that geographic location may unjustly influence global perception and evaluation.

## Project Aim

This project investigates the extent to which **geographic location alone** can predict a university’s position in QS and THE rankings. It further explores whether the inclusion of **objective academic indicators**—such as research productivity, patent output, and institutional metadata—can lead to a more **equitable and data-driven evaluation** of global academic performance..



### 3. Project Goals and Objectives

#### Main Goal

To evaluate the **influence of geographic region** on global university rankings and to determine whether **objective academic performance indicators**—such as research productivity and innovation capacity—can provide a **more equitable alternative** to perception-based rankings like QS and THE.

This project aims to highlight **regional biases** in current methodologies and to develop predictive models that rely on **measurable, data-driven metrics** rather than subjective global prestige.

####  Research Questions

- To what extent does a university’s **continent or region** affect its QS and THE rankings?
- Are current global rankings disproportionately influenced by **subjective and geopolitical factors**?
- Can **objective metrics** (e.g., publications, patents, institutional age) **outperform geographic location** in predicting academic excellence?

#### Hypothesis:

> **"The most critical determinant of a university’s global academic standing should be its actual performance in research and innovation—not its geographic location or perceived prestige."**


### 4. Data Collection & Enrichment

#### Data Sources

The dataset used in this study was built by combining multiple sources of institutional data, including:

- **QS World University Rankings**
- **Times Higher Education (THE) Rankings**
- **CSRankings** (computer science research outputs)
- **WIPO / Google Patents** (patent and innovation metrics)

Additional metadata such as **region**, **location**, **ownership type**, and **establishment year** were also integrated to enhance the dataset.

####  Data Processing Workflow

To prepare the dataset for analysis, the following steps were followed:

##### Step 1: Ranking Alignment and Enrichment

- **Manual Matching**:  
  Due to inconsistencies in university naming conventions (e.g., prefixes like *"The"*, abbreviations, and language differences), QS and THE datasets could not be automatically merged. A **manual matching process** was conducted to align entries one by one.
  
- **Unified Ranking Construction**:  
  A combined ranking metric was created using **normalized scores** from both QS and THE:
Example: New Score=(0.5*QS Rank)+(0.5*THE Rank)
  Normalization techniques such as **min-max scaling** and **z-score normalization** were tested to ensure comparability across scales.

- **Research and Innovation Enrichment**:
  - Added publication data and research area information from **CSRankings**.
  - Added patent counts and tech transfer metrics from **WIPO/Google Patents**.
  - Created derived features such as **institutional age**, **ownership**, and **continent**.


##### Step 2: Exploratory Visualization and Pre-Modeling Analysis

- **Rank Consistency Analysis**:  
  Investigated how universities vary between QS and THE rankings to uncover stability or volatility patterns.
  
- **Correlation Analysis**:  
  Explored relationships between rankings and objective indicators such as **publications**, **patents**, and **ownership type**.

- **Bias Evaluation**:  
  Analyzed how strongly **geographic region** correlates with ranking position—regardless of academic output—providing early insight into possible **regional prestige bias**.

These steps laid the foundation for further **predictive modeling** and **bias detection**, enabling the evaluation of how fairly QS and THE rankings reflect actual research and innovation performance across global regions.


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

### 6. Conclusion & Future Work

#### Conclusion

This study examined the structural limitations and implicit biases embedded in global university ranking systems—specifically those of QS and Times Higher Education (THE). By enriching traditional ranking data with **objective academic performance indicators**, such as publication output (CSRankings), patent activity (WIPO/Google Patents), and institutional metadata (region, age, ownership), a more holistic and transparent analysis of university performance was achieved.

A key finding of the project was that **geographic location alone**—independent of measurable research or innovation—serves as a **strong predictor** of a university’s rank. In predictive models, regional variables consistently outperformed or rivaled core performance indicators, such as research output. This pattern indicates the presence of **regional prestige bias**, where institutions from **Europe and North America** tend to receive **higher rankings**, even when their objective performance is on par with or below that of **Asian universities**, which are often **undervalued**.

The analysis demonstrated that traditional ranking systems may inadvertently reinforce **global hierarchies** rather than reward academic merit. Institutions in regions like **Asia**, which have made significant advances in scientific research, technological innovation, and academic output, do not always see these successes reflected in their global standing.

Thus, the project supports the conclusion that global university rankings are not fully reflective of institutional quality and that relying on **subjective perception metrics**—such as academic reputation surveys—can distort public understanding of academic excellence. These results call for a shift toward **data-driven, equitable, and transparent evaluation methodologies** that emphasize **research productivity, innovation, and measurable impact** over prestige and historical dominance.

Future Directions:
	•	Expanding the dataset to analyze historical trends in university rankings.
	•	Developing an interactive dashboard for real-time ranking comparisons.
	•	Exploring machine learning techniques to predict university ranking trends based on research and industry performance.

## References:
https://www.topuniversities.com/world-university-rankings
https://www.timeshighereducation.com/world-university-rankings/2024/world-ranking
