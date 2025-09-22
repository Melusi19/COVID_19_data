# COVID-19 Exploratory Data Analysis (OWID Dataset)

This project performs an exploratory data analysis (EDA) of the **Our World in Data (OWID) COVID-19 dataset**.  
It explores case trends, deaths, and vaccination progress across countries, with visualizations including line charts, bar plots, correlation heatmaps, and choropleth maps.

---

## 📊 Dataset
Source: [Our World in Data – COVID-19](https://ourworldindata.org/coronavirus)  
File used: `owid-covid-data.csv`

**Key Columns**
- `date` – Observation date  
- `location` – Country/region name  
- `iso_code` – Country ISO code (used for maps)  
- `total_cases`, `new_cases`  
- `total_deaths`, `new_deaths`  
- `total_vaccinations`, `people_fully_vaccinated`  
- `population`  

---

## 🔧 Tools & Libraries
- [Python 3](https://www.python.org/)  
- [pandas](https://pandas.pydata.org/) – data cleaning and manipulation  
- [matplotlib](https://matplotlib.org/) – plotting  
- [seaborn](https://seaborn.pydata.org/) – statistical plots  
- [plotly express](https://plotly.com/python/plotly-express/) – choropleth maps  

Install dependencies:
```bash
pip install pandas matplotlib seaborn plotly

🚀 How to Run

Clone this repository or download the files.

Place the owid-covid-data.csv file in the project directory.

Open the Jupyter Notebook:

jupyter notebook covid19_eda.ipynb


Run all cells in order.

📈 Analysis Workflow

Data Loading & Exploration – Load the CSV, inspect structure, check missing values.

Data Cleaning – Handle missing values, select countries of interest (Kenya, USA, India).

Exploratory Data Analysis – Cases, deaths, daily new cases, and death rate trends.

Vaccination Analysis – Cumulative vaccinations and % fully vaccinated over time.

Global Overview – Top 10 countries by total cases, correlation heatmap.

Choropleth Maps – Cases per million and vaccination rates on a world map.

Insights & Reporting – Document key findings.

🌍 Example Insights

India had the highest spike in daily new cases among Kenya, USA, and India.

The USA recorded the highest cumulative deaths.

Kenya’s vaccination rollout lagged compared to the USA and India.

Death rates stabilized after major vaccination campaigns.

Choropleth maps highlight uneven vaccine distribution globally.

📂 Project Structure
├── covid19_eda.ipynb   # Main Jupyter Notebook
├── owid-covid-data.csv # Dataset (not included, download from OWID)
└── README.md           # Project documentation

📝 Notes

The dataset is updated regularly by OWID. Make sure you use the latest CSV.

Choropleth maps require ISO country codes (iso_code) available in the dataset.

The notebook can be extended with interactive dashboards (e.g., Streamlit or Dash).
