# ⛽ Pakistani Vehicle Price Prediction

## 📄 Introduction
The used car market in Pakistan plays a significant role in the country’s economy, valued at **PKR 1.5 trillion (USD 5 Billion)** with over **2000 cars changing hands daily** (Source: PAMA 2023). However, determining fair prices remains challenging due to **data scarcity, subjectivity, and lack of transparency**.

This project leverages **machine learning** to bring **accuracy, fairness, and transparency** to used car pricing in Pakistan, providing an **AI-powered vehicle price prediction system**.

---

## 🌟 Objective
The goal of this project is to **revolutionize car pricing** in Pakistan through machine learning by:
- ✔ Providing **accurate price estimates** based on vehicle attributes and market trends.
- ✔ **Empowering buyers** with informed decision-making.
- ✔ **Boosting seller confidence** with data-driven pricing.
- ✔ Enhancing **transparency and fairness** in the market.

---

## ❓ Problem Description
The current car pricing system faces multiple issues:
- **📊 Data Scarcity**: Limited reliable data makes valuation difficult.
- **🤖 Subjectivity**: Prices vary due to individual assessments and biases.
- **🎨 Information Asymmetry**: Sellers often have more information than buyers.
- **🔒 Lack of Transparency**: Buyers struggle to understand price determinants.

---

## 🔬 Methodology
### 📚 Data Collection
- Data sourced from **PakWheels.com** (Pakistan’s largest automobile marketplace).
- Custom **Python-based web scraper** (built with Scrapy) extracted **59,817 car listings**.

### 🛠 Data Pre-Processing
- **Feature Engineering**: Extracted **Make, Model, Variant** from car names.
- **Brand Harmonization**: Unified similar brands (e.g., "Range Rover" & "Land Rover").
- **Outlier Removal**:
  - **Mileage & Engine Capacity**: Used IQR filtering & domain knowledge.
  - **Price Cleaning**: Removed unrealistic values and "Call for Price" entries.
- **Final Dataset**: **54,984 records** with 9 features, stored as `CleanedPakWheels.csv`.

### 🎯 Model Training
We trained four machine learning regression models:

| Model | MAE | MSE | R² Score |
|--------|--------------|-----------------|------------|
| **Linear Regression** | 742,825.63 | 10,558,350,352,630 | 0.6946 |
| **Decision Tree** | 448,053.27 | 2,758,935,622,566 | 0.9202 |
| **XGBoost** | 424,358.50 | 1,360,031,035,991 | **0.9606** |
| **LightGBM** | 456,811.62 | 2,451,209,441,574 | 0.9291 |

- **XGBoost and LightGBM performed the best**, demonstrating **high accuracy and efficiency**.

---

## 📲 User Interface Development
- Allows users to **input car details** and receive an **AI-generated price estimate**.

---

## 🌍 Solution Application Areas
This system can benefit various stakeholders:
- 🚗 **Used car buyers & sellers**: Informed decision-making and fair pricing.
- 🏢 **Car dealerships**: Improved pricing accuracy and customer satisfaction.
- 🏦 **Financial institutions**: Loan collateral valuation.
- 💼 **Insurance companies**: Accurate insurance policy pricing.

---

## 🛠️ Tools & Technologies Used
- **Programming Languages**: Python, Java
- **Machine Learning Libraries**: scikit-learn, XGBoost, LightGBM
- **Data Processing**: NumPy, Pandas
- **Web Scraping**: Scrapy
- **Mobile App Development**: Java (Android Studio)

---

## 📊 Analysis & Findings
- Evaluated **56 test vehicles** sourced from PakWheels.com.
- **XGBoost & LightGBM models showed the highest accuracy** in predicting used car prices.
- Model predictions closely aligned with **actual car prices**, improving market transparency.
![Screenshot 1](https://github.com/SyedMuhammadHamzaAli/Pakistani-Vehicle-Price-Prediction-/blob/main/Pakistani%20Vehicle%20price%20predict.png)
---

## ✅ Conclusion
This project successfully addresses **key issues** in Pakistan's used car market by introducing an **AI-powered valuation system**. The combination of **data-driven insights, advanced ML models, and an intuitive mobile interface** enhances transparency, fairness, and accuracy in car pricing.

---

## ✨ Future Improvements
- Expand dataset for better generalization.
- Implement **real-time API integration** for live price updates.
- Enhance mobile app **user experience** and introduce new features.

---

## 🔗 Repository Details
Feel free to **contribute** or report issues! 
- **Author:** Syed Muhammad Hamza Ali  
- **License:** MIT  

---
