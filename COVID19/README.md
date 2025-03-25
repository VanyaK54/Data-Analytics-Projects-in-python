# Diabetes Prediction Using Machine Learning

## Project Overview
This project aims to predict the likelihood of diabetes in individuals using machine learning techniques. The model is trained on healthcare data and considers various health metrics such as glucose levels, BMI, age, and other relevant features. The goal is to provide a reliable predictive tool that can assist in early detection and intervention.

## Key Features
- **Data Collection:** Utilizes COVID-19 and World Bank datasets for socio-economic and health-related indicators.
- **Data Processing:** Converts raw data into structured datasets, handling missing values and data inconsistencies.
- **Feature Engineering:** Creates features such as daily case changes, cases since first 100 cases, and mortality rates.
- **Machine Learning:** Implements predictive models for outcome estimation.
- **Automated Testing:** Includes comprehensive test cases to ensure data integrity and consistency.

## Project Structure
```
├── data
│   ├── raw
│   ├── processed
├── scripts
│   ├── download_data.py
│   ├── make_all.py
│   ├── make_cases.py
│   ├── make_cases_daily_change.py
│   ├── make_cases_since_t0.py
│   ├── make_continents.py
│   ├── make_coordinates.py
│   ├── make_country_stats.py
│   └── utils.py
├── tests
│   └── test.py
├── README.md
```

## Usage
1. **Download Data:**
   ```bash
   python scripts/download_data.py
   ```

2. **Process Data:**
   ```bash
   python scripts/make_all.py
   ```

3. **Run Tests:**
   ```bash
   python -m unittest tests/test.py
   ```

## Test Cases
- **Boat Data Removal:** Ensures data from cruise ships like MS Zaandam is excluded.
- **Data Consistency:** Verifies confirmed cases match the sum of active, recovered, and dead cases.
- **Edge Cases:** Checks for data completeness and correct date formats.

## Future Improvements
- Implement predictive modeling for case forecasting.
- Add visualizations for better data interpretation.
- Integrate a web interface for end-user interaction.

## Contributions to this repo
- Added a new test case to ensure data consistency across case types.

## License
This project is licensed under the MIT License.

