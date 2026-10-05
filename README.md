🇮🇳 COVID-19 India — EDA

Exploring how COVID-19 spread across India through data, trends and visualizations.

This project is a Python-based Exploratory Data Analysis (EDA) of India's COVID-19 data. It examines state-wise case patterns, recovery and mortality rates, monthly trends, and India's vaccination progress.

🔎 What This Project Explores
How COVID-19 cases changed over time
Which states recorded the highest number of cases
Differences in recovery and death rates across states
Monthly patterns in new cases
India's vaccination rollout
Relationships between different COVID-19 indicators
🧰 Tech Stack
Python
│
├── NumPy       → Numerical operations
├── Pandas      → Data manipulation & analysis
├── Matplotlib  → Visualization
├── Seaborn     → Statistical visualization
└── Jupyter     → Notebook environment
📊 Data at a Glance
COVID-19 Cases

Period: January 2020 – August 2020

The case dataset contains daily information for Indian states and Union Territories, including confirmed cases, deaths, recoveries and newly reported cases.

Before cleaning:

4,692 records
10 columns
40 distinct state/UT labels

The data was standardized to remove naming inconsistencies and duplicate entries.

💉 Vaccination

A separate dataset from Our World in Data is used to study India's vaccination progress beginning in January 2021.

🧹 Data Preparation

Real-world datasets are rarely analysis-ready.

The project handles:

Incorrect data types
Inconsistent state names
Duplicate records
Missing-value checks
Column standardization
Derived metrics

One important transformation was calculating:

Active Cases = Confirmed Cases - Deaths - Recovered
After cleaning, the analysis works with 35 standardized states/UTs and no remaining missing values.
📈 Analysis Approach
01 — Data Inspection

Understanding the structure, data types and quality of the raw datasets.

02 — Cleaning

Standardizing names, fixing data types and removing duplicate records.

03 — Aggregation

Using Pandas operations such as:

groupby()
pivot_table()

to generate national and state-level summaries.

04 — Metrics

Calculating:

Recovery Rate
Death Rate
Active Cases
New Confirmed Cases
05 — Visualization

Creating 12 visualizations to communicate the major patterns in the data.

💡 A Few Findings

For the final date available in the case dataset — 6 August 2020:

Indicator	Value
Confirmed	1,964,536
Recovered	1,328,336
Deaths	40,699
Recovery Rate	67.62%
Death Rate	2.07%




Among the states in the final snapshot, Maharashtra recorded the highest confirmed-case count, while the state-level comparison also highlights substantial differences in recovery and death rates.

🗺️ State & Monthly Analysis

The project uses a monthly pivot table to compare new cases across major affected states.

For example, Maharashtra's monthly new-case totals increased substantially through June and July, while different states experienced their strongest growth at different points in the dataset.

This makes the analysis more than just a collection of charts — it helps identify when and where the outbreak accelerated.

📁 Project Structure
📦 India-COVID19-EDA
│
├── 📓 India_COVID19_Analysis.ipynb
├── 📄 README.md
└── 📄 requirements.txt
▶️ Run Locally

Clone the repository:

git clone https://github.com/your-username/India-COVID19-EDA.git
cd India-COVID19-EDA

Install the required libraries:

pip install -r requirements.txt

Launch Jupyter:

jupyter notebook

The notebook loads the datasets directly from their public sources, so the raw CSV files do not need to be manually stored in the repository.

📚 What I Learned

Through this project, I practiced the complete EDA workflow on a real-world dataset:

Raw Data → Cleaning → Transformation → Analysis → Visualization → Insights

More importantly, the project helped me understand how data quality decisions can directly affect the conclusions drawn from an analysis.

👩🏻‍💻 About

Navya Vij

B.Tech CSE — Data Science

Interested in Data Analytics | Business Analytics | Strategy | Data-Driven Decision Making

⭐ Feedback

If you found this analysis interesting, feel free to explore the notebook and share your feedback.
