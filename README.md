# 🏡 Real Estate Price Analysis and Prediction

## 📌 Project Overview
This project explores a dataset containing global property listings and applies **Data Science** and **Machine Learning** techniques to analyze the factors influencing real estate prices. The primary goal is to understand how different property attributes affect price variations and to develop predictive models for property valuation.

## 📂 Dataset
- **Source:** `properties_data.csv`
- **Size:** 1,905 entries, 38 columns
- **Key Features:**
  - **Location-based:** `neighborhood`, `latitude`, `longitude`
  - **Property size:** `size_in_sqft`, `price_per_sqft`
  - **Amenities:** `private_pool`, `shared_gym`, `walk_in_closet`, etc.
  - **Price Information:** `price`

## 📊 Exploratory Data Analysis (EDA)
### 🔍 Key Insights:
- **Correlation analysis**: Identified the most relevant factors impacting price.
- **Data distribution**: Visualized using histograms, boxplots, and scatter plots.
- **Geographical analysis**: Mapped property prices based on location.
- **Outlier detection**: Removed extreme price values using the **Interquartile Range (IQR)** method.

## 🛠 Data Preprocessing
- **Missing Values & Duplicates:** Verified and handled appropriately.
- **Feature Engineering:**
  - Created **new features** such as `price_per_sqft`.
  - Encoded categorical variables (`quality`, `neighborhood`).
  - Normalized numerical variables (`size_in_sqft`, `price_per_sqft`).

## 🧠 Machine Learning Models
### 1️⃣ **Linear Regression**
- **Objective:** Predict property prices based on key attributes.
- **Performance Metrics:**
  - **Mean Absolute Error (MAE):** 178,092
  - **Root Mean Squared Error (RMSE):** 250,988

### 2️⃣ **Decision Tree Regressor**
- **Objective:** Capture non-linear relationships in property pricing.
- **Performance:**
  - **MAE:** 68,293
  - **RMSE:** 120,912
  - **Cross-validation accuracy:** 98%

### 3️⃣ **Multi-Layer Perceptron (MLP)**
- **Objective:** Neural network-based regression model for price prediction.
- **Architecture:**
  - Input: 8 features
  - 4 hidden layers (16-8-4-2 neurons)
  - Output: 1 neuron (Price)
- **Optimization:** Hyperparameter tuning with GridSearchCV.
- **Final Performance:** MAE: **17.8k**, RMSE: **26.3k**

## 🎯 Key Takeaways
✅ Location, size, and quality significantly impact property prices.
✅ Decision Trees performed better than Linear Regression.
✅ MLP model showed potential with fine-tuning but required further optimization.

## 🚀 Future Improvements
- Implement **ensemble methods** (Random Forest, Gradient Boosting) to improve predictions.
- Integrate **geospatial analysis** to refine location-based pricing trends.
- Fine-tune **deep learning models** with advanced hyperparameter tuning.


