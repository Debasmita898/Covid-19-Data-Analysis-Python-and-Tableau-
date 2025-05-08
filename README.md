"""
# 🦠 COVID-19 India Analysis and Visualization

This project presents a comprehensive exploratory data analysis (EDA), data cleaning, transformation, and visualization of two key datasets:

- **COVID-19 India Dataset** — containing case-wise data such as confirmed cases, cured, and deaths.
- **COVID-19 Vaccine Statewise Dataset** — providing detailed vaccination information by gender, age, and dose status.

---

## 📁 Datasets Used

1. **`covid-19_india.csv`**
   - Columns: `Sno`, `Date`, `Time`, `State/UnionTerritory`, `ConfirmedIndianNational`, `ConfirmedForeignNational`, `Cured`, `Deaths`, `Confirmed`

2. **`covid_vaccine_statewise.csv`**
   - Columns: `Updated On`, `State`, `Total Doses Administered`, `Sessions`, `Sites`, `First Dose Administered`, `Second Dose Administered`, `Male (Doses Administered)`, `Female (Doses Administered)`, `Transgender (Doses Administered)`, `...`, `Total Individuals Vaccinated`, etc.

---

## 🔧 Key Transformations

- Added **Active Cases**, **Recovery Rate** and **Mortality Rate** per state.
- Updated Column names.
- Cleaned inconsistencies in state names.
- Handled null values and merged overlapping data where necessary.
- Removed unncessary columns.
- Changed datatype of 'Date' column from object to datetime format.
- Created a Pivot table with aggregate function 'Max'.
- Create a gradient colormap.

---

## 📊 Key Findings

### 🏥 COVID Cases Analysis:
- **Top 10 States with Most Active Cases**:
  - Maharashtra, Karnataka, Kerala, Uttar Pradesh, Tamil Nadu, Rajasthan, Andhra Pradesh, Gujarat, West Bengal, Chhattisgarh.
  
- **Top 10 States with Highest Deaths**:
  - Maharashtra (highest by a large margin), Karnataka, Delhi, Uttar Pradesh, West Bengal, Punjab, Chhattisgarh, Andhra Pradesh, Gujarat.

- **Most Affected State**:
  - Maharashtra was the most affected during both the first and second waves, with the second wave being significantly worse.

- **Top States by Recovery & Mortality Rate**:
  - Punjab and Sikkim ranked highest for both **Recovery Rate** and **Mortality Rate**.

---

### 💉 Vaccination Insights:
- **Gender-wise Vaccination**:
  - Males: **53%**
  - Females: **47%**
  - Transgenders: **~0.015%**

- **Top 5 Vaccinated States**:
  - Maharashtra, Uttar Pradesh, Rajasthan, Gujarat, West Bengal

- **Age Group Distribution**:
  - Most vaccinations occurred in the **45–60 years** and **60+ years** groups.

- **Dose Coverage**:
  - **76.1%** of people received **only the first dose**
  - **23.9%** received **both doses**

---

## 📈 Visualizations

- Bar charts: Top states by cases, deaths, vaccinations
- Line graphs: Case trends over time
- Pie charts: Gender and dose-wise vaccination distribution
- Donut chart: Partial vs. complete vaccination comparison
- Sub-plots: Recovery vs. Mortality Rate

---

## 📌 Conclusion

This project provides valuable insights into the spread and control of COVID-19 in India. It highlights the disparities in impact across states and vaccination distribution among different groups.

---
## 💻 Technologies Used

- Python (Pandas, NumPy, Seaborn, Matplotlib, Plotly)
- Jupyter Notebook

---
## Visulaization Using Tableau
## 📊 COVID-19 Visualization – `country_wise_latest` Dataset

I used the `country_wise_latest` dataset to create an interactive COVID-19 dashboard in Tableau. This dataset includes up-to-date country-level statistics such as:

- Confirmed Cases
- Deaths
- Recoveries
- Active Cases
- Mortality and Recovery Rates

---
### 📁 Dataset Overview
The `country_wise_latest.csv` file provides a snapshot of the latest COVID-19 data by country. It served as the primary source for the visualizations in this project.

Columns: 'Country/Region','Confirmed','Deaths',	'Recovered','Active',	'New cases',	'New deaths',	'New recovered',	'Deaths / 100 Cases',	'Recovered / 100 Cases',	'Deaths / 100', 'Recovered',	'Confirmed last week',	'1 week change',	'1 week % increase',	'WHO Region'.

---
### 📷 Dashboard Preview
![COVID-19 Tableau Dashboard]

