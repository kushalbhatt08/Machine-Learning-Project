# 🏠 California House Value Prediction using Machine Learning

This project builds and evaluates multiple machine learning regression models to predict median house values across California districts. It uses the well-known **California Housing Dataset** sourced directly from `scikit-learn`, derived from the 1990 U.S. Census, which contains 20,640 records across 8 numerical features per census block group.

---

## 📊 Dataset Overview

The dataset is loaded using `sklearn.datasets.fetch_california_housing` and includes the following features:

| Feature | Description |
|---|---|
| **MedInc** | Median income in the block group |
| **HouseAge** | Median age of houses in the block |
| **AveRooms** | Average number of rooms per household |
| **AveBedrms** | Average number of bedrooms per household |
| **Population** | Block group population |
| **AveOccup** | Average number of household members |
| **Latitude** | Geographic latitude of the block |
| **Longitude** | Geographic longitude of the block |

The target variable is **MedHouseVal** — the median house value for California districts (in units of $100,000).

---

## 🔍 Project Workflow

### 1. Data Loading & Exploration
The dataset is loaded using scikit-learn and converted into a Pandas DataFrame for exploration. Basic inspection is performed using `.head()`, `.describe()`, and `.info()` to understand the structure and distributions of the data.

### 2. Exploratory Data Analysis (EDA)
Visualizations are created using Matplotlib and Seaborn to understand feature distributions, correlations, and relationships with the target variable. This step helps identify key predictors of house value.

### 3. Data Preprocessing
The target column (`MedHouseVal`) is added to the DataFrame. Features (X) and the target (y) are separated, and the data is split into training and testing sets using an 80/20 split via `train_test_split`. Feature scaling is applied using `StandardScaler` to normalize the data for better model performance.

### 4. Model Training & Evaluation
Three regression algorithms are trained and evaluated:

- **Linear Regression** — A baseline model that assumes a linear relationship between features and the target.
- **Decision Tree Regressor** — A non-linear model that splits data based on feature thresholds.
- **Random Forest Regressor** — An ensemble of decision trees that averages predictions to improve accuracy and reduce overfitting.

Each model is evaluated using three key metrics:
- **MAE** (Mean Absolute Error)
- **MSE** (Mean Squared Error)
- **R² Score** (Coefficient of Determination)

### 5. Model Comparison & Selection
Based on the evaluation metrics, the **Random Forest Regressor** outperforms the other models with an R² score of approximately **0.806**, a MAE of **~0.332**, and an MSE of **~0.255**, making it the best model for this task.

### 6. Prediction on New Data
The final Random Forest model is used to predict the median house value for a new, custom data point. For example, given a block with median income of 7.325, house age of 30 years, average rooms of 5.984, and located at latitude 37.88 / longitude -122.23, the model predicts a median house value of approximately **$365,998**.

---

## 🛠️ Technologies Used

- **Python 3.8**
- **Pandas & NumPy** — Data manipulation and numerical computation
- **Matplotlib & Seaborn** — Data visualization
- **Scikit-learn** — Machine learning models, preprocessing, and evaluation metrics
- **Jupyter Notebook** — Interactive development environment

---

## 📈 Results Summary

| Model | MAE | MSE | R² Score |
|---|---|---|---|
| Linear Regression | Higher | Higher | ~0.60 |
| Decision Tree | Medium | Medium | ~0.63 |
| **Random Forest** | **~0.332** | **~0.255** | **~0.806** |

The Random Forest Regressor achieved the best performance, explaining over **80% of the variance** in house values on the test set.

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/house-value-prediction.git
   cd house-value-prediction
   ```

2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook House_value_prediction.ipynb
   ```

4. Run all cells sequentially to reproduce the results.

---

## 👤 Author

**Kushal Bhatt**
