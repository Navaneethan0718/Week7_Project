COVID-19 Data Analysis and Interactive Dashboard

The COVID-19 pandemic generated massive amounts of global health data. Analyzing this data helps researchers, governments, and organizations understand infection trends, mortality rates, recovery patterns, and the overall impact of the virus.

This project performs Exploratory Data Analysis (EDA) on a global COVID-19 dataset and develops an interactive dashboard using Dash and Plotly. The dashboard allows users to explore COVID-19 statistics for different countries through dynamic visualizations.

Objectives

* Collect and analyze global COVID-19 data.
* Clean and preprocess the dataset.
* Study trends in confirmed, recovered, and death cases.
* Compare COVID-19 cases across countries.
* Create interactive visualizations using Plotly.
* Develop a web-based dashboard using Dash.
* Enable users to explore country-specific COVID-19 statistics.

Dataset Information

Data Source

The dataset is loaded directly from GitHub:

https://raw.githubusercontent.com/datasets/covid-19/main/data/time-series-19-covid-combined.csv



| Column         | Description           |
| -------------- | --------------------- |
| Date           | Date of record        |
| Country/Region | Country name          |
| Province/State | State or province     |
| Confirmed      | Total confirmed cases |
| Recovered      | Total recovered cases |
| Deaths         | Total death cases     |



* Python
* Pandas
* Plotly Express
* Dash
* HTML Components (Dash)
* Jupyter Notebook



The following preprocessing steps were performed:



The Date column was converted into datetime format for time-series analysis.



Duplicate records were removed to improve data quality.


Missing values were replaced with zero values where appropriate.

The project calculates:

* Total Confirmed Cases
* Total Death Cases
* Total Recovered Cases


* Total Confirmed Cases: 118,939,403,514
* Total Deaths: 2,261,860,890
* Total Recovered Cases: 23,227,207,579

 COVID-19 Trend Analysis

A line chart was created to visualize:

* Confirmed Cases
* Death Cases
* Recovered Cases

over time.

Country-wise Analysis

A bar chart compares confirmed COVID-19 cases across countries.

Case Distribution

A pie chart illustrates the proportion of:

* Confirmed Cases
* Recovered Cases
* Death Cases

Correlation Visualization

A scatter plot analyzes the relationship between:

* Confirmed Cases
* Death Cases
* Recovered Cases

for different countries.

Interactive Dashboard

The project includes a Dash-based dashboard that allows users to:

* Select a country from a dropdown menu.
* View country-specific COVID-19 trends.
* Analyze confirmed cases over time.
* Interact with visualizations in real time.

Dashboard Features

* Country Selection Dropdown
* Dynamic Line Graph
* Interactive User Interface
* Real-Time Data Visualization

Project Structure

```text
COVID-19-Dashboard/
│
├── covid_dashboard.py
├── README.md
├── requirements.txt
│
├── images/
│   ├── trend_chart.png
│   ├── country_cases.png
│   ├── pie_chart.png
│   └── scatter_plot.png
│
└── dashboard_screenshot.png
```

---
Installation

Clone the Repository

```bash
git clone https://github.com/yourusername/covid19-dashboard.git
```

Install Required Libraries

```bash
pip install pandas plotly dash
```
Run the Dashboard

```bash
python covid_dashboard.py
```

Open your browser and visit:

```text
http://127.0.0.1:8050/
```

---

Key Insights

* COVID-19 cases increased rapidly during major outbreak periods.
* Some countries experienced significantly higher case counts than others.
* Recovery rates improved over time in many regions.
* Death rates varied across countries and time periods.
* Interactive dashboards make pandemic data easier to understand and explore.

---

Future Enhancements

* Add vaccination statistics.
* Include active case tracking.
* Integrate real-time API updates.
* Add geographical maps.
* Deploy the dashboard on Render or Heroku.
* Implement advanced analytics and forecasting models.

---

Conclusion

This project demonstrates how data analysis and interactive visualization tools can be used to explore large-scale health datasets. By combining Pandas, Plotly, and Dash, the application provides an intuitive way to analyze COVID-19 trends and gain meaningful insights from global pandemic data.

---

