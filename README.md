# Weather and Energy Production Analysis in Sweden

## Overview
This repository contains a comprehensive analysis of the relationship between weather conditions and energy production in Sweden. By leveraging data from Swedish meteorological and statistical agencies, the project examines how variables such as temperature, wind speed, and irradiance influence energy output across various sources (e.g., wind and solar).

### Objectives
- Understand the impact of weather conditions on energy production.
- Identify seasonal dependencies and patterns to help optimize energy production.
- Utilize clustering and regression techniques for detailed analysis.

## Data Sources
1. **Sveriges meteorologiska och hydrologiska institut (SMHI)**: Weather data.
2. **Statistikmyndigheten (SCB)**: Energy production statistics.

### Data Characteristics
- Spans 12 to 90 months, capturing seasonal and annual variations.
- Aggregated monthly data.
- Key variables: Air temperature, rainfall, sunshine time, wind speed, cloud percentage, humidity, irradiance, and energy production (wind, solar, and total).

---

## Methodology

### Tools Used
- **KNIME**: For data integration, clustering, and regression analysis.

### Techniques
1. **Data Aggregation**:
   - Daily/hourly data aggregated into monthly averages.
2. **Clustering**:
   - Hierarchical clustering to identify patterns without pre-defining the number of clusters.
3. **Regression Analysis**:
   - Linear regression to explore relationships between weather variables and energy production.
   - Coefficient of determination (R²) used for performance evaluation.

---

## Results and Key Insights

### 1. Air Temperature vs. Total Energy Production
- Data from 5 stations over 90 months.
- **Insight**: Strong correlation between lower temperatures and higher energy production due to heating demands during winter.

### 2. Wind Power vs. Wind Speed
- Data from 4 stations over 90 months.
- **Insight**: Positive but weak correlation between wind speed and energy production. Energy production is higher during winter, likely due to increased wind turbine deployment and stronger winds.

### 3. Solar Power vs. Weather Variables
- Variables: Temperature, sunshine time, irradiance.
- **Insight**: Sunshine time showed a clear clustering effect on solar power usage. Other variables lacked significant structure.

### 4. Irradiance and Solar Time vs. Total Energy Production
- Data from 5 stations over 90 months.
- **Insight**: Distinct clusters for warmer and colder months. Average temperature and irradiance showed a cyclic relationship, with temperature lagging irradiance.

---

## Visualizations
- **Scatter Plots**: Highlight relationships between variables (e.g., temperature vs. irradiance).
- **Parallel Coordinates Plot**: Show clustering based on sunshine time.
- **Cluster Analysis**: Segmented data into meaningful groups for better understanding of seasonal variations.

---

## How to Use

### Requirements
- Python 3.8+
- Libraries: KNIME (for workflow execution), Pandas, Matplotlib, Scikit-learn.

### Steps to Reproduce
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/weather-energy-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd weather-energy-analysis
   ```
3. Follow the KNIME workflow (provided in the `workflow.knwf` file) to recreate the analysis.

---

## Acknowledgments
This project was developed by Group #6 (Mahmut Osmanovic, Isac Paulsson, Sebastian Tuura, Mohamed Al Khaled) as part of the TDSR22 Data Science course, 2024.

## License
This repository is licensed under the MIT License. See `LICENSE` for details.
