# Wind Turbine Data Analysis and Prediction

This repository contains a Jupyter Notebook for analyzing and predicting wind turbine power output using machine learning techniques. The analysis utilizes a dataset of wind turbine data collected from 2013 to 2016.

## Dataset

The dataset used in this project is sourced from the [ENGIE Open Data](https://opendata-renewables.engie.com/explore/dataset/d543716b-368d-4c53-8fb1-55addbe8d3ad/information). It includes various parameters such as wind speed, temperature, and power output recorded over several years at a wind farm.

## Dependencies

To run the notebook, the following Python packages are required:

- pandas
- numpy
- matplotlib
- seaborn
- sklearn
- pandas-profiling (Note: You might need to install this separately as it may not be included in the standard Anaconda distribution)

You can install the missing dependencies using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn pandas-profiling
```

## Notebook Overview

1. **Data Loading and Preprocessing**: 
   - The CSV file is read and relevant columns are extracted.
   - Date-time parsing and sorting are performed for time-series analysis.

2. **Exploratory Data Analysis (EDA)**:
   - Missing values are identified and filtered.
   - Data is visualized using correlation matrices and pair plots.
   - A `pandas_profiling` report is generated for a comprehensive overview.

3. **Machine Learning Models**:
   - A Random Forest Regressor is implemented to predict the average power output (`P_avg`).
   - Model performance is evaluated using metrics such as Mean Absolute Error (MAE) and R-squared score.
   - Feature importance is visualized to understand the influence of different variables.

4. **Advanced Techniques**:
   - A Gradient Boosting Regressor is employed to provide prediction intervals.
   - The model's performance is compared with the Random Forest model.

## Results

- The Random Forest model achieved a high R-squared score of 0.997, indicating excellent predictive performance.
- The Gradient Boosting model showed a slightly lower R-squared score but provided valuable insights into prediction intervals.

## Usage

To use this notebook, clone the repository and open the notebook in Jupyter Notebook or Jupyter Lab. Ensure that all dependencies are installed. Run the notebook cells sequentially to reproduce the analysis and results.

## Contribution

Feel free to open issues or contribute to the repository by forking and submitting pull requests. Contributions that improve the analysis or add new features are welcome.

## License

This project is licensed under the MIT License.

--- 
