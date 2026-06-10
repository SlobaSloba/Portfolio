# Portfolio

Hello, and welcome to my portfolio! 

Below, you will find a variety of projects that I have either done for clients in the past, or have created using mock/online data to showcase my skills in fields where real data that I have worked with is proprietary or sensitive. For each of the projects, you will find a link to the HTML rendering of the .Rmd or .ipynb file, which will include the full code and output that was used for the analysis, along with comments outlining the steps I took and the interpretation of the output. 

If you have any questions or would like to collaborate, reach out at: slobodan.pantelicc@gmail.com

## Projects Overview

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
10/06/2026: Added Market Research: Developer Survey Analysis: Android vs. iOS (Python
