# House Price Prediction in Pakistan

## Project Overview

This project uses Machine Learning techniques to predict house prices in Pakistan based on various property characteristics.

The dataset contains information about residential properties including area, bedrooms, bathrooms, city location, and additional amenities. Several regression algorithms are trained and compared to identify the model that provides the most accurate predictions.

---

## Features

- Data Cleaning and Preprocessing
- Area Conversion to Square Feet
- Price Conversion to PKR
- Missing Value Handling
- Outlier Removal
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Multiple Machine Learning Models
- Model Evaluation and Comparison
- House Price Prediction Function

---

## Dataset Features

The following features are used for prediction:

| Feature | Description |
|----------|-------------|
| area_sqft | Property area in square feet |
| baths | Number of bathrooms |
| beds | Number of bedrooms |
| city_code | Encoded city value |
| Kitchens | Number of kitchens |
| Dining Room | Availability of dining room |
| Drawing Room | Availability of drawing room |
| Laundry Room | Availability of laundry room |
| Store Rooms | Availability of store rooms |

Target Variable:

```text
price
```

---

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---

## Data Preprocessing

The following preprocessing steps were performed:

### Area Conversion

Different area units were converted into square feet:

- Marla → Square Feet
- Kanal → Square Feet
- Square Yard → Square Feet

### Price Conversion

Prices were converted into Pakistani Rupees (PKR):

- Lakh → PKR
- Crore → PKR

### Missing Values

Missing values were handled using:

- Median imputation for bathrooms
- Median imputation for bedrooms

### Outlier Removal

Extreme price values were removed using the:

- 1st percentile
- 99th percentile

---

## Exploratory Data Analysis

The following visualizations were created:

### Price Distribution

Shows the distribution of house prices.

### Average Price per City

Compares median property prices across cities.

### Area vs Price

Scatter plot showing relationship between property size and price.

### Bedroom Impact

Shows how the number of bedrooms affects property prices.

### Feature Importance

Identifies the most influential features affecting house prices.

---

## Machine Learning Models

The following models were trained and evaluated:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. Gradient Boosting Regressor

---

## Evaluation Metrics

Models were evaluated using:

### R² Score

Measures how well the model explains price variation.

### Mean Absolute Error (MAE)

Measures average prediction error in PKR.

---

## Best Model Selection

All models are compared automatically and the model with the highest R² score is selected as the best-performing model.

Example:

```python
Best Model: Random Forest
R² Score: 0.89
Avg Error: 2.10 Million PKR
```

(Note: Actual results may vary depending on the dataset.)

---

## Prediction Function

The project includes a custom prediction function:

```python
predict_house_price()
```

Example:

```python
predict_house_price(
    area_sqft=5445,
    baths=5,
    beds=5,
    city_name='Islamabad',
    kitchens=2,
    dining=1,
    drawing=1
)
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/House-Price-Prediction-Pakistan.git
```

Move into the project directory:

```bash
cd House-Price-Prediction-Pakistan
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

---

## Project Workflow

1. Load Dataset
2. Clean Data
3. Convert Area Units
4. Convert Prices
5. Handle Missing Values
6. Remove Outliers
7. Perform EDA
8. Encode Categorical Variables
9. Train Models
10. Evaluate Models
11. Select Best Model
12. Predict House Prices

---

## Future Improvements

- Hyperparameter Tuning
- Cross Validation
- Web Application Deployment
- Streamlit Interface
- More Property Features
- Real-Time Property Data Integration

---

## Author

Saifullah Khan

Machine Learning Enthusiast | Computer Science Student
