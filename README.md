\# E-commerce Product Analytics



\## User Behavior, Conversion, Retention \& Experimentation



\### Overview



This project analyzes e-commerce user interaction data to understand how users move through the purchasing funnel, how they engage with the platform, and how their behavior changes over time.



The project follows an end-to-end product analytics workflow using event-level user data.



\### Business Objectives



\- Analyze the user purchasing funnel

\- Measure user engagement and activity

\- Analyze conversion behavior

\- Segment users into activity cohorts and measure retention

\- Demonstrate statistical experimentation methodology

\- Identify areas for further product investigation



\### Dataset



The dataset contains approximately 10 days of e-commerce event data.



Key characteristics:



\- 115,403 unique visitors

\- 214,787 events

\- 65,173 unique products

\- 133,336 inferred sessions



The primary event types include product views, add-to-cart events, and transactions.



\### Analysis Performed



\#### 1. User Funnel Analysis



The purchasing journey was analyzed across:



View → Add to Cart → Purchase



Key results:



\- View → Cart conversion: 2.55%

\- Cart → Purchase conversion: 31.36%

\- View → Purchase conversion: 0.80%



\#### 2. Session Analysis



User events were grouped into sessions using a 30-minute inactivity threshold, resulting in 133,336 inferred sessions.



\#### 3. User Engagement



Daily and weekly activity patterns were analyzed using active-user metrics.



\- Average DAU: approximately 11,352

\- Peak DAU: 13,789



\#### 4. Cohort \& Retention Analysis



Users were grouped based on their first recorded activity week.



The first cohort showed 3.39% retention into the following week.



Because the dataset covers only approximately 10 days, the retention analysis has limited long-term follow-up.



\#### 5. Statistical Experimentation



Because the source dataset does not contain actual experimental treatment assignments, an A/A simulation was used to demonstrate an experimentation workflow.



Results:



\- Control conversion: 0.8095%

\- Treatment conversion: 0.7884%

\- Absolute difference: -0.0211 percentage points

\- Relative lift: -2.61%

\- p-value: 0.6871

\- 95% confidence interval: -0.1238 to +0.0816 percentage points



The simulated experiment did not provide sufficient evidence of a statistically significant difference between the two groups.



\### Key Findings



\- A large drop-off occurs between product viewing and cart addition.

\- Users who added items to their cart converted at a substantially higher rate than the overall visitor population.

\- User engagement varied throughout the observed period.

\- The short observation window limits long-term retention analysis.

\- The simulated A/A test demonstrated how conversion differences can be evaluated using statistical significance and confidence intervals.



\### Tools \& Technologies



\- Python

\- Pandas

\- NumPy

\- Matplotlib

\- Jupyter Notebook

\- Statistical hypothesis testing



\### Project Structure



```text

Product\_Analysis\_Project/

│

├── notebooks/

│   └── Product\_Analytics.ipynb

│

├── reports/

│   └── Product\_Analytics\_Report.pdf

│

├── data/

│   └── raw/

│

├── README.md

├── requirements.txt

└── .gitignore

