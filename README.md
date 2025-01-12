# Forecasting-Sticker-Sales
Sales Predictions for Sticker Sales Using Gradient Boosting

## Project Overview
This project focuses on developing a machine learning model to predict product sales across different regions and stores. Using Gradient Boosting Regressor, the model achieves high accuracy and minimizes error, making it suitable for forecasting and decision-making.

## Key Features
- **Model Used:** Gradient Boosting Regressor
- **Hyperparameter Tuning:** Optimized model parameters using GridSearchCV.
- **Error Analysis:** Residual analysis to identify patterns in prediction errors.
- **Feature Importance:** Insights into the most impactful features on predictions.

## Dataset
The dataset includes historical sales data with features like:
- `date`: Date of the sales record
- `store`: Store identifier
- `country`: Country where the store is located
- `product`: Product category identifier
- `num_sold`: Number of units sold (target variable)

## Model Performance
### Train Set Metrics:
- **MAPE:** 0.2374
- **MAE:** 37.5486
- **R²:** 0.9922

### Validation Set Metrics:
- **MAPE:** 0.2419
- **MAE:** 38.6949
- **R²:** 0.9918

## Steps to Reproduce
1. Clone this repository:
   ```bash
   git clone <repository_url>
   cd <repository_folder>
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook sales_prediction.ipynb
   ```

## Files in the Repository
- `sales_prediction.ipynb`: Jupyter Notebook containing the entire workflow.
- `train.csv`: Training dataset.
- `test.csv`: Test dataset.
- `submission_predictions.csv`: Predicted results for the test dataset.
- `requirements.txt`: List of Python dependencies.

## How to Use
1. Train the model using the provided training dataset.
2. Use the trained model to generate predictions for the test dataset.
3. Save predictions in the required format (`id`, `num_sold`) for submission or further analysis.

## Results and Insights
### Feature Importance:
The top features contributing to the predictions include:
- `month`
- `weekday`
- `day`
- `store`

### Error Analysis:
Residual analysis showed that the model performs well across most data points, with minor underestimations in specific cases.

## Submission Format
The output predictions are saved in a CSV file with the following structure:
| id  | num_sold |
|-----|----------|
| 1   | 500      |
| 2   | 600      |
| ... | ...      |

## Future Improvements
- Experimenting with additional models like XGBoost or LightGBM.
- Incorporating external data sources (e.g., holidays, weather).
- Enhancing hyperparameter optimization using Bayesian search.

## Contact
If you have questions or feedback, feel free to reach out:
- **LinkedIn:** [Your LinkedIn Profile]([https://linkedin.com/in/your-profile](https://www.linkedin.com/in/edo-aditya-0b2867103/))
- **GitHub:** [Your GitHub Profile]([https://github.com/your-profile](https://github.com/eaditya99))

---
Thank you for exploring this project!
