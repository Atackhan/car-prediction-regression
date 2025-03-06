---

## **README.md**

```markdown
# 🚗 Car Price Prediction Using Machine Learning

This project aims to predict the selling price of used cars based on various factors such as age, kilometers driven, fuel type, seller type, and transmission. The dataset includes information about multiple car models and their corresponding selling prices.

## 📌 Project Overview

- **Data Cleaning & Preprocessing**
  - Removed irrelevant columns (e.g., `Car_Name`).
  - Converted categorical variables (`Fuel_Type`, `Seller_Type`, `Transmission`) into numerical values.
  - Created a new feature `No_Year` to represent the car's age.
  - Checked for missing values and handled them accordingly.

- **Exploratory Data Analysis (EDA)**
  - Visualized trends of selling prices over the years.
  - Analyzed correlations between different features.
  - Identified the most important features using `ExtraTreesRegressor`.

- **Model Building**
  - Split the dataset into training (80%) and testing (20%) sets.
  - Trained two different machine learning models:
    1. **Random Forest Regressor** (with hyperparameter tuning using `RandomizedSearchCV`).
    2. **XGBoost Regressor** (with optimized hyperparameters).
  - Compared model performance using **Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).**

## 📊 Results & Model Comparison

| Model                  | MAE  | MSE  | RMSE  |
|------------------------|------|------|-------|
| **Random Forest**      | 0.8884 | 2.8509 | 0.9425 |
| **XGBoost (Best Model)** | 0.5686 | 0.8044 | 0.8969 |

✅ The **XGBoost model performed better** with lower error rates and was chosen as the final model for car price prediction.

---

## 🔧 Technologies Used

- **Python** (pandas, numpy, matplotlib, seaborn)
- **Scikit-Learn** (Random Forest, ExtraTreesRegressor)
- **XGBoost**
- **Matplotlib & Seaborn** (for visualization)

---

## 📂 Dataset Information

The dataset contains the following features:

| Feature         | Description |
|---------------|-------------|
| `Year`         | Manufacturing year of the car |
| `Selling_Price` | Selling price of the car (target variable) |
| `Present_Price` | Current market price of the car |
| `Kms_Driven`   | Total kilometers driven by the car |
| `Fuel_Type`    | Type of fuel used (Petrol/Diesel/CNG) |
| `Seller_Type`  | Individual or Dealer |
| `Transmission` | Manual or Automatic |
| `Owner`       | Number of previous owners |

---

## 📌 How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/car-price-prediction.git
   cd car-price-prediction
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
   Open `Car_Price_Prediction.ipynb` and execute all cells.

---

## 📢 Future Improvements

🔹 Improve feature engineering by adding more external car-related data.  
🔹 Test with deep learning models such as Neural Networks.  
🔹 Deploy the model using Flask or FastAPI for real-world application.  

---

## 🛠 Author

👤 **Atakan AKIN**  

### ✅ **How to Use It on GitHub**
1. Copy the above markdown content.
2. Create a new file in your GitHub repository called **README.md**.
3. Paste the content and commit the changes.

Bu **README.md** dosyası projenin yapısını, kullanılan teknolojileri ve nasıl çalıştırılacağını güzelce özetliyor. Eğer özel bir ekleme yapmak istersen bana söyleyebilirsin! 🚀
