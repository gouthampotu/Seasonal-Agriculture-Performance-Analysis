# Seasonal-Agriculture-Performance-Analysis
Seasonal Agriculture Performance Analysis

VOIS × AICTE

A focused data analytics project investigating how agricultural
performance varies across Kharif, Rabi, and Zaid seasons using
farm-level environmental, resource, production, and economic data.

Project Overview

Agricultural performance is influenced by seasonal environmental
conditions, farming practices, resource availability, crop
characteristics, and market conditions. This project analyzes the
supplied agricultural dataset to identify meaningful seasonal patterns
in yield, production, resource usage, profitability, water efficiency,
and disease/pest risk.

The central question is:

How does agricultural performance vary across seasons, and what
meaningful patterns can be identified from the available data?

The project combines data cleaning, exploratory data analysis,
visualization, descriptive statistics, and statistical testing to
produce evidence-based insights.

Problem Statement

Raw agricultural data does not directly explain how agricultural
performance changes between seasons.

This project therefore investigates:

Seasonal differences in yield and production

Changes in revenue, cost, and profitability

Differences in resource usage

Seasonal environmental conditions

Water-use efficiency

Disease/pest risk

Crop-specific seasonal performance

Irrigation-related differences

Statistical significance of seasonal yield differences

Important patterns requiring further investigation

Objectives

Explore and understand the agricultural dataset.

Clean and prepare the data for analysis.

Compare agricultural performance across Kharif, Rabi, and Zaid.

Identify important seasonal patterns and trends.

Examine relationships between environmental conditions and outcomes.

Compare resource usage across seasons.

Analyze economic performance and profitability.

Compare crop performance across seasons.

Identify significant and unusual observations.

Apply appropriate statistical and visualization techniques.

Interpret findings using evidence from the dataset.

Develop practical, evidence-based recommendations.

Document the analysis in a reproducible Jupyter/Google Colab
notebook.

Dataset

The project uses the agricultural dataset supplied for the VOIS AICTE
Batch 1 2026--2027 Major Project.

Attribute                          Value

Records                            4,000
Variables                             28
Seasons                                3
Seasons               Kharif, Rabi, Zaid
Crop categories                        8
Observation level             Farm-level

The dataset contains information related to:

Farm and geographical characteristics

Crop and season

Environmental conditions

Soil characteristics

Farming inputs

Irrigation

Water usage

Yield and production

Market price

Revenue and costs

Profitability

Disease/pest risk

Water-use efficiency

Analytical Questions

The project addresses questions including:

How does agricultural yield vary across seasons?

Which season has the highest average yield?

How does profitability change between seasons?

Which season has the highest average profit?

How does water consumption vary across seasons?

Which season has better water-use efficiency?

How does disease/pest risk vary by season?

Are there meaningful crop × season differences?

How does irrigation method relate to yield, water use, and profit?

Are observed seasonal yield differences statistically significant?

How much yield variation can be explained by season alone?

What findings can support better seasonal agricultural planning?

Methodology

1. Data Loading

The CSV dataset is loaded using Pandas and its dimensions, structure,
data types, and variables are inspected.

2. Data Quality Assessment

The analysis checks for missing values, duplicates, inconsistent data
types, unusual values, and numerical distributions.

3. Data Cleaning

Missing values in Rainfall_mm, Soil_Moisture_pct, and
Yield_Tonnes_Ha are handled using season-wise median imputation so
that seasonal context is retained. Duplicate records are also checked.

4. Exploratory Data Analysis

Descriptive statistics and visualizations are used to examine seasonal
distributions, relationships, crop patterns, resource usage, and
economic outcomes.

5. Seasonal Comparison

Kharif, Rabi, and Zaid are compared using yield, production, revenue,
cost, profit, water usage, water efficiency, disease/pest risk, and
environmental measures.

6. Statistical Analysis

The project applies: - One-way ANOVA - Kruskal--Wallis test - Pairwise
Mann--Whitney U tests - Bonferroni correction - Eta-squared effect size

7. Interpretation

Statistical results are interpreted together with descriptive statistics
and visual evidence.

8. Recommendations

Recommendations are derived from observed dataset patterns and are
presented as planning insights rather than causal claims.

Key Results

Season           Avg. Yield  Avg. Profit (₹)          Water   Disease/Pest
(t/ha)                      Efficiency           Risk
(t/1,000 m³)

Kharif         5.63   178,914.65       5.89     54.47%

Rabi               5.04        87,689.47           5.19         40.48%

Zaid               4.64       -24,804.82           4.41         38.22%

Major Findings

Kharif recorded the highest average yield at approximately 5.63
tonnes/hectare, the highest average profit at approximately ₹1.79
lakh per farm, and the highest water-use efficiency at approximately
5.89 tonnes per 1,000 m³.

However, Kharif also recorded the highest average disease/pest risk at
approximately 54.47%, highlighting a performance-versus-risk
trade-off.

Rabi recorded an average yield of approximately 5.04
tonnes/hectare and average profit of approximately ₹87,689 per
farm, placing it between Kharif and Zaid for the main performance
measures.

Zaid recorded the lowest average yield at approximately 4.64
tonnes/hectare, the lowest water-use efficiency at approximately
4.41 tonnes per 1,000 m³, and an average loss of approximately
₹24,805 per farm.

Statistical Evidence

The analysis indicates statistically significant differences in yield
distributions across the three seasons using the non-parametric
Kruskal--Wallis test. Pairwise Mann--Whitney U comparisons also remain
significant after Bonferroni correction.

At the same time, the calculated eta-squared effect size is
approximately 0.004, indicating that season alone explains only a very
small proportion of total yield variation.

This is an important interpretation:

Season matters, but season alone does not explain agricultural
performance.

Crop, farm characteristics, environmental conditions, inputs,
irrigation, and geographical differences should therefore be considered
together with season.

Visualizations

The notebook includes visual analysis covering:

Average yield by season

Average profit by season

Water efficiency and disease/pest risk

Irrigation method and profitability

Crop × season yield comparison

Seasonal distributions

Correlation analysis

Outlier investigation

Key Agricultural Insights

1. Kharif shows the strongest average performance

Kharif leads the dataset in average yield, profit, and water-use
efficiency.

2. Zaid requires closer investigation

Zaid shows the lowest average yield and water efficiency and has
negative average profit.

3. Higher performance can coexist with higher risk

Kharif combines strong production outcomes with the highest disease/pest
risk.

4. Season should not be analyzed in isolation

The small effect size indicates that other variables contribute
substantially to yield variation.

5. Irrigation deserves deeper analysis

Differences in profitability and water usage across irrigation methods
provide useful areas for further investigation. These are associations
and should not be interpreted as proof of causation.

Recommendations

Seasonal planning

Give additional attention to the lower-performing Zaid season.

Investigate the factors contributing to Zaid's negative average
profitability.

Use seasonal performance benchmarks for crop and resource planning.

Resource management

Investigate practices associated with higher water-use efficiency.

Compare irrigation strategies alongside crop, soil, region, and
environmental conditions.

Evaluate water use using productivity per unit of water rather than
consumption alone.

Risk management

Incorporate Kharif's higher disease/pest risk into seasonal
planning.

Identify crops, regions, and environmental conditions associated
with higher risk.

Consider crop-specific risk management strategies.

Future analytics

Build predictive models for yield and profit.

Add multi-year agricultural records.

Integrate weather and market-price information.

Develop crop- and region-specific recommendation systems.

Use causal or experimental designs to evaluate interventions.

Limitations

Findings are limited to the supplied dataset.

Statistical association does not establish causation.

Season alone explains only a small proportion of yield variation.

Selected missing numerical values were imputed using season-wise
medians.

The analysis does not establish causal effects of irrigation,
inputs, or other farming practices.

Multi-year data would improve seasonal trend analysis.

External weather and market information was not added unless
represented in the supplied dataset.

Recommendations should be validated with agricultural domain experts
before real-world use.

Project Structure

Seasonal-Agriculture-Performance-Analysis/
│
├── README.md
├── Seasonal_Agriculture_Performance_Analysis.ipynb
│
├── data/
│   └── seasonal_agriculture_performance_dataset.csv
│
├── presentation/
│   └── VOIS_AICTE_Seasonal_Agriculture_Performance_Analysis_Presentation.pptx
│
└── outputs/
    ├── charts/
    └── analysis_outputs/

If the dataset is restricted, do not upload the raw CSV to a public
GitHub repository. Instead, provide instructions for obtaining or
placing the dataset locally.

Technologies Used

Python --- Core programming language

Pandas --- Data manipulation and analysis

NumPy --- Numerical computation

Matplotlib --- Data visualization

SciPy --- Statistical testing

Google Colab / Jupyter Notebook --- Reproducible analysis

Microsoft PowerPoint --- Project presentation

How to Run

Google Colab

Open Google Colab.

Upload the project notebook.

Upload the dataset when prompted.

Ensure the dataset path matches the notebook configuration.

Run all cells sequentially.

Review the generated tables, charts, statistical tests, and
conclusions.

Local Jupyter

Install the required packages:

pip install pandas numpy matplotlib scipy jupyter

Start Jupyter:

jupyter notebook

Open the notebook and execute the cells from top to bottom.

Future Scope

The project can be extended into an agricultural decision-support system
through:

Machine-learning-based yield prediction

Profit forecasting

Disease/pest risk prediction

Crop recommendation

Irrigation recommendation

Weather-integrated analytics

Market-price forecasting

Region-specific agricultural intelligence

Power BI/Tableau dashboards

Explainable AI for agricultural recommendations

The next stage is to move from descriptive analytics toward
predictive and prescriptive analytics.

Conclusion

This project demonstrates how agricultural data can be transformed into
meaningful seasonal insights through data cleaning, exploratory
analysis, visualization, statistical testing, and evidence-based
interpretation.

The supplied dataset shows clear differences among Kharif, Rabi, and
Zaid in yield, profitability, water-use efficiency, and disease/pest
risk. Kharif demonstrates the strongest overall average performance,
while Zaid shows comparatively weaker economic and resource-efficiency
outcomes.

However, the small eta-squared effect size shows that season alone
explains only a small share of yield variation. This reinforces the
importance of considering crop, environment, inputs, irrigation, farm
characteristics, and geography together.

Overall, the project provides a structured analytical foundation for
better seasonal agricultural planning and a pathway toward future
predictive and decision-support solutions.

Author

Student: Goutham Potu
Program: VOIS × AICTE
Project: Seasonal Agriculture Performance Analysis

AICTE STU ID: Add from offer letter
College: Add college name
GitHub: Add repository link

Acknowledgement

This project was completed as part of the VOIS × AICTE 
Major Project for the problem statement Seasonal
Agriculture Performance Analysis.
