COVID-19 Global Data Tracker

objectives
Buildig a data analysis and reporting notebook (or app) that tracks global COVID-19 trends. The project analyzes cases, deaths, recoveries, and vaccinations across countries and time. it involed cleaning and processing real-world data, performing exploratory data analysis (EDA), generating insights, and visualizing trends using Python data tools.

 Project Objectives:
✅ Import and clean COVID-19 global data
✅ Analyze time trends (cases, deaths, vaccinations)
✅ Compare metrics across countries/regions
✅ Visualize trends with charts and maps
✅ Communicate findings in a Jupyter Notebook or PDF report 

 Tools and libraries used
pandas
matplotlib
seaborn
Jupyter Notebook (or VS Code with Jupyter extension) 


How to run/view the project
Project Segments (Step-by-Step Guide)
1️⃣ Data Collection

Goal: Obtain a reliable COVID-19 dataset.

✅ Data Sources:

Our World in Data COVID-19 Dataset (CSV & API)

Johns Hopkins University GitHub Repository

👉 Recommended for beginners: Use the cleaned CSV from Our World in Data (easy to load with pandas).

✅ Action:

Download owid-covid-data.csv from the above link.

Save in your working folder.


2️⃣ Data Loading & Exploration

Goal: Load the dataset and explore its structure.

✅ Tasks:

Load data using pandas.read_csv().

Check columns: df.columns.

Preview rows: df.head().

Identify missing values: df.isnull().sum().

✅ Tools:

pandas

📌 Key columns:

date, location, total_cases, total_deaths, new_cases, new_deaths, total_vaccinations, etc.


3️⃣ Data Cleaning

Goal: Prepare data for analysis.

✅ Tasks:

Filter countries of interest (e.g., Kenya, USA, India).

Drop rows with missing dates/critical values.

Convert date column to datetime: pd.to_datetime().

Handle missing numeric values with fillna() or interpolate().

✅ Tools:

pandas

4️⃣ Exploratory Data Analysis (EDA)

Goal: Generate descriptive statistics & explore trends.

✅ Tasks:

Plot total cases over time for selected countries.

Plot total deaths over time.

Compare daily new cases between countries.

Calculate the death rate: total_deaths / total_cases.

✅ Visualizations:

Line charts (cases & deaths over time).

Bar charts (top countries by total cases).

Heatmaps (optional for correlation analysis).

✅ Tools:

matplotlib

seaborn

5️⃣ Visualizing Vaccination Progress

Goal: Analyze vaccination rollouts.

✅ Tasks:

Plot cumulative vaccinations over time for selected countries.

Compare % vaccinated population.

✅ Charts:

Line charts.

Optional: Pie charts for vaccinated vs. unvaccinated.

✅ Tools:

matplotlib

seaborn

6️⃣ Optional: Build a Choropleth Map

Goal: Visualize cases or vaccination rates by country on a world map.

✅ Tools:

Plotly Express

Or geopandas (advanced)

✅ Tasks:

Prepare a dataframe with iso_code, total_cases for the latest date.

Plot a choropleth showing case density or vaccination rates.


Any insights or reflections
India had one of the fastest vaccination rollouts by total volume, administering hundreds of millions of doses within months of vaccine availability. However, its percentage of fully vaccinated individuals remained lower than that of the U.S.

The United States showed early and rapid case growth, but also led in early access to vaccines. Despite that, new case spikes continued due to uneven vaccine uptake and emerging variants.

Kenya experienced slower vaccine distribution, with a much lower percentage of the population vaccinated as compared to India and the U.S., highlighting disparities in global vaccine access.

Death rates were highest during the early waves of the pandemic before vaccine rollouts. After vaccination campaigns scaled up, death rates began to stabilize or decline.

Anomalies:

Some countries show zero daily new cases or deaths for extended periods, likely due to missing data or underreporting.

Sudden jumps in total case numbers for some countries suggest data corrections or backlogged reporting.

