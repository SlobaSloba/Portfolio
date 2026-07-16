# Portfolio

Hello, and welcome to my portfolio! 

Below, you will find a variety of projects that I have either done for clients in the past, or have created using mock/online data to showcase my skills in fields where real data that I have worked with is proprietary or sensitive. For each of the projects, you will find a link to the HTML rendering of the .Rmd or .ipynb file, which will include the full code and output that was used for the analysis, along with comments outlining the steps I took and the interpretation of the output. 

If you have any questions or would like to collaborate, reach out at: slobodan.pantelicc@gmail.com

## Projects Overview

### Cardiovascular Risk: Lipoprotein(a) & ASCVD Discrimination Analysis

[Open Report](./Cardiovascular-health.html)

- Evaluated whether Lipoprotein(a) improves on standard ASCVD risk categories as a predictor of subclinical atherosclerosis, using logistic regression on a de-identified clinical dataset (~2,000 patients)
- Benchmarked discrimination via ROC/AUC analysis (AUC package): the ASCVD 10-year risk score achieved an AUC of 0.713, while Lp(a) alone performed near chance (AUC ≈ 0.48)
- Modeled 7-year time-to-revascularization (CABG/PCI) via Kaplan-Meier survival analysis (survival, survminer), then simulated hazard-based survival curves from ASCVD scores to validate calibration against observed outcomes
- Extended the analysis to family history/statin scenario modeling and Aortic Stenosis prediction, finding Lp(a) added no incremental value in either case — concluding ASCVD risk scores alone fully capture the available predictive signal in this cohort

---

### Real-World Evidence: Patient-Reported Outcomes After Stem Cell Injection Therapy

[Open Report](./Hospital-data-project.html)

- Analyzed real-world, non-randomized clinical data from patients receiving stem cell injection therapy (autologous fat- or bone-marrow-derived) for pain management, tracking nine patient-reported outcomes (PROs) — anxiety, depression, four pain domains, physical/mental health, and social role functioning — across an irregular, up-to-one-year follow-up schedule (baseline through day 365)
- Modeled each PRO trajectory with linear mixed-effects models (`lme4`/`lmerTest`, one random intercept per patient) and derived estimated marginal means and contrasts against baseline via `emmeans`, with Benjamini–Hochberg FDR correction across all simultaneous tests
- Constructed a time-varying stem-cell-source exposure variable that avoids immortal time bias to compare fat-derived vs. bone-marrow-derived cells, addressing confounding by indication inherent to non-randomized therapy selection
- Found statistically significant, clinically consistent reductions in pain intensity, behavior, and interference (most pronounced around day 90), no detectable change in psychological/general-health outcomes, and transparently reported that no exposure comparison survived multiple-testing correction

---

### Epidemiology: Allergy & Wheeze Risk Factor Analysis
[Open Report](./allergy_analysis.html)

- Analyzed observational clinical data to evaluate environmental, biological, and demographic risk factors associated with allergy and wheezing prevalence
- Built multivariable logistic regression models in R to estimate adjusted odds ratios (aORs), establishing key predictors while controlling for confounding variables
- Conducted regression diagnostics and multicollinearity checks to validate model assumptions and ensure epidemiological rigor
- Generated reproducible, deliver-ready tables and visualizations (TFLs) translating complex statistical associations into clear risk profiles for clinical stakeholders

---

### Developer Survey Analysis: Android vs. iOS
[Open Notebook](./Mobile development survey analysis.html)

- Cleaned and recoded a 5,000-respondent mobile developer survey using a codebook-driven recode map, handling three distinct response formats (single-choice ordinal, multi-select binary flags, and ranked platform preference)
- Analysed platform reach across six mobile platforms, finding Android dominant at 81.5% total reach; examined cross-platform targeting patterns, showing iOS-primary developers are more likely to also target Android (56%) than the reverse (42%)
- Profiled Android vs. iOS primary developers across geography, experience, organisation size, roles, app categories, and programming languages, identifying the most strategically relevant differences for a business audience
- Found iOS developers are concentrated in high-income western markets and skew more senior (50.5% with 3+ years mobile experience vs. 33.6% for Android), while Android developers are more prevalent in emerging markets and more likely to work independently

---

### Market Research: E-Commerce Sustainability Certifications
[Open Notebook](./Sustainability_Market_Research_Portfolio.html)
- Developed an asynchronous Python web scraper utilizing the Scrapfly API and `asyncio` to extract pricing, ratings, and certification badges from ~15,800 Amazon UK beauty products
- Conducted statistical hypothesis testing (Welch’s t-tests, Levene's test) and calculated Cohen's *d* effect sizes to evaluate market outcome differences between certified and non-certified items
- Trained and evaluated OLS and Random Forest regression models (`scikit-learn`, `statsmodels`) to predict price and engagement metrics based on specific sustainability badges
- Analyzed consumer survey data (N=102) using Linear Mixed-Effects Models to estimate Green Perceived Value (GPV), measuring interactions between certification types, demographics, and environmental identity

---

### Data Visualization: UK Gender Disparity Dashboard
[Open Dashboard](./Gender%20disparity%20UK%20dashboard.html)
- Developed an interactive Tableau dashboard to visualize gender pay gap metrics and workforce representation across various UK industries and organizations
- Engineered calculated fields, parameters, and interactive filters to allow users to dynamically explore wage differences by company size, sector, and geographic region
- Designed accessible data visualizations to highlight systemic earnings disparities and easily identify sectors with the most significant wage gaps
- Translated complex national demographic and salary data into an intuitive interface, facilitating data-driven storytelling and exploratory analysis

---

### NLP: Morgan Stanley Employee Sentiment Analysis
[Open Notebook](./MS_Sentiment_Analysis_Portfolio.html)
- Scraped 10,000+ employee reviews from Glassdoor and Indeed via the Scrapfly API, handling JavaScript rendering and anti-scraping protections
- Built a parallelised, fault-tolerant multi-page scraper with automatic checkpointing in R
- Conducted sentiment analysis using three NLP lexicons (NRC, Bing, AFINN) to capture emotion categories, polarity, and numeric sentiment scores
- Performed temporal analysis across four periods (Pre-COVID to time of analysis), uncovering a sustained post-2018 decline in employee sentiment

---

### Labour Economics: Remote Work & Mental Health
[Open Report](./wfh_policy_report.html)
- Estimated the causal effect of gaining a work-from-home option on mental health using LISS panel data (Netherlands, 2019–2024)
- Applied a Difference-in-Differences design exploiting COVID-19 as an exogenous shock, with two-way fixed effects and wild-cluster bootstrap inference
- Validated the parallel trends assumption visually and via placebo testing; excluded COVID-affected waves to isolate the WFH effect
- Found a significant negative effect on MHI-5 scores, concentrated among parents and full-time employees, with policy recommendations

---

### Churn Dataset Simulation  
[Open Notebook](./Churn%20dataset%20simulation.html)
- Built a synthetic dataset (100K users) to simulate churn behavior  
- Engineered behavioral and subscription-based features to reflect real-world drivers  
- Embedded probabilistic churn logic to enable controlled experimentation  
- Designed dataset for downstream analytics and predictive modeling workflows  

---

### SQL Analysis (DuckDB)  
[Open Notebook](./SQL%20analysis.html)
- Analyzed relational data (users, subscriptions, activity logs) using DuckDB  
- Wrote SQL queries for joins, aggregations, and time-series analysis  
- Evaluated engagement, retention, and revenue-related metrics  
- Translated query outputs into actionable business insights  

---

### Econometrics: Homeownership Analysis  
[Open Notebook](./Econometrics.html)
- Modeled time-to-homeownership using survival analysis techniques  
- Applied log-rank tests to compare demographic groups  
- Built logistic regression models to estimate ownership probability  
- Analyzed income mobility and its impact on housing outcomes  

---

### NLP: Instagram Influencer Messaging
[Open Report](./Instagram-analysis.html)
- Conducted Natural Language Processing (NLP) on social media corpora to extract messaging patterns
- Performed sentiment analysis leveraging the NRC emotion lexicon
- Applied Latent Dirichlet Allocation (LDA) for topic modeling, utilizing quantitative criteria for rigorous model selection
- Mapped comparative corpus structures using tf-idf weighting and `igraph` network visualizations

---

### Financial Inclusion, Digital Trust, and Economic Growth
[Open Report](./Trust-in-banks---portfolio-project.html)
- Investigated the relationship between digital trust, financial inclusion, and macroeconomic indicators
- Conducted statistical analysis to identify key drivers of user trust in digital banking environments
- Evaluated demographic and behavioral factors influencing financial participation and adoption
- Synthesized findings to provide actionable insights on digital financial engagement

---

Change history: \
18/03/2026: Created repo, added Churn dataset simulation (Python) and exploration (Python + SQL) \
25/03/2026: Added Econometrics notebook (Python) \
26/03/2026: Added Instagram NLP analysis (R) and Financial Inclusion project (R) \
27/03/2026: Added Morgan Stanley Employee sentiment analysis (R) \
02/04/2026: Added Labour Economics: Remote Work & Mental Health (R + Stata) \
08/04/2026: Added Market Research: E-Commerce Sustainability Certifications (Python) \
10/06/2026: Added Market Research: Developer Survey Analysis: Android vs. iOS (Python) \
13/06/2026: Added Data Visualization: UK Gender Disparity Dashboard (Tableau) \
08/07/2026: Added Cardiovascular Risk: Lipoprotein(a) & ASCVD Discrimination Analysis (R) \
16/07/2026: Added Epidemiology: Allergy & Wheeze Risk Factor Analysis and Real-World Evidence: Patient-Reported Outcomes After Stem Cell Injection Therapy (R)
