# World Population Exploratory Data Analysis (EDA) 🌍📊

This repository contains an Exploratory Data Analysis (EDA) of the World Population dataset using Python, Pandas, Matplotlib, and Seaborn. The analysis covers historical population trends from 1970 to 2022, country-wise rankings, growth rates, population density, and feature correlations.

---

## 📂 Dataset Source & Raw Data

The dataset used for this analysis is available in this repository:
- **CSV File**: [world_population.csv](https://github.com/AlexTheAnalyst/PandasYouTubeSeries/blob/main/world_population.csv) *(Click to view or download the raw data)*
- **Data Source**: The dataset can also be accessed and downloaded publicly from popular data repositories like Kaggle.

---

## 📌 Dataset Overview

The dataset (`world_population.csv`) contains historical population data and demographic metrics for 234 countries/territories.

### Key Features (Columns):
- **Rank**: Country rank based on 2022 population.
- **CCA3**: 3-letter Country Code.
- **Country**: Name of the country/territory.
- **Capital**: Capital city name.
- **Continent**: Continent where the country is located.
- **Population Columns**: Historical population records (`2022`, `2020`, `2015`, `2010`, `2000`, `1990`, `1980`, `1970`).
- **Area (km²)**: Total land area in square kilometers.
- **Density (per km²)**: Population density per square kilometer.
- **Growth Rate**: Population growth rate factor.
- **World Population Percentage**: Percentage share of total world population.

---

## 🛠️ Tech Stack & Dependencies

- **Language**: Python 3.x
- **Libraries Used**:
  - `pandas`: Data manipulation and inspection
  - `matplotlib`: Data visualization
  - `seaborn`: Advanced statistical data visualization

### Installation

Install the required Python packages:
```bash
pip install pandas matplotlib seaborn
```

---

## 🚀 Analysis & Key Steps Covered
1. ### Environment Setup & Data Import:
```text
- Libraries (pandas, matplotlib, seaborn) imported.
- Loaded dataset into Pandas DataFrame.
- Configured float formatting to 2 decimal places (pd.set_option('display.float_format', ...)).
```

2. ### Data Inspection:
- **df.info()**: Inspected column data types and identified missing/null values.
- **df.describe()**: Summary statistics (mean, std, min, max, percentiles) for numerical attributes.
- **df.isnull().sum()**: Evaluated missing value counts per feature.
- **df.nunique()**: Counted unique values across categorical and numerical fields.

3. ### Demographic Insights & Sorting:
```text
-Identified top most populous countries in 2022 using df.sort_values(by="2022 Population", ascending=False).
-Analyzed top countries by World Population Percentage.
```

4. ### Correlation Analysis:
```text
-Computed correlation matrix across all numerical attributes using df.select_dtypes(include="number").corr().
-Identified strong linear relationships between historical population counts across all milestone years.
```

---

## 📊 Key Insights & Findings
- **Top Populous Nations (2022)**: China and India lead globally, together accounting for over 35% of the total world population.
- **Historical Correlation**: High positive correlation (~0.97 - 1.00) exists across population metrics from 1970 to 2022, indicating consistent long-term population scaling across most nations.
- **Density & Area Variation**: High variance in population density and land area across countries (min density ~0.03/km² up to over 23,000/km²).

---

## 💻 How to Run
Clone the repository:
```Bash
git clone [https://github.com/your-username/world-population-eda.git](https://github.com/your-username/world-population-eda.git)
cd world-population-eda
```
Ensure world_population.csv is placed in the project root folder.
-Open and run the Jupyter Notebook (EDA.ipynb):
```Bash
jupyter notebook
```

---
