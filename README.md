# 🏠 House Price Prediction in Ho Chi Minh City

This repository contains a complete end-to-end data science workflow for predicting house prices in Ho Chi Minh City, Vietnam. The project covers **web scraping**, **data preprocessing**, **exploratory data analysis**, **feature engineering**, **machine learning modeling**, and **deep learning experiments**.

---

## 📌 Table of Contents
- [Project Overview](#project-overview)
- [Work Flow](#work-flow)
- [Challenges Encountered](#challenges-encountered)
- [Conclusion](#conclusion)
- [Contributors](#contributors)

---

## 📖 Project Overview

The goal of this project is to build a predictive system that estimates house prices based on real-world data scraped from: https://batdongsan.vn/ban-nha/

The workflow includes:
1. Collecting raw real estate listings via **web scraping**
2. Cleaning and engineering features
3. Visualizing the geographic and statistical properties of the dataset
4. Training multiple machine learning models
5. Experimenting with a basic deep learning model

---

## 📂 Work Flow

### **1. `Data Collection`**
- Extracts URL tails used for crawling.
- Defines the structure and features of the crawling DataFrame
- Integrates:
  - **Generative Language API**
  - **Geocoding API**
- Scrapes housing listings and stores them in  `Initial Data.xlsx`.

---

### **2. `Data Preprocessing and Feature Engineering`**
- Cleaning scraped data
- Handling missing values
- Removing or adjusting outliers
- Creating new meaningful features
- Ensuring data consistency
- Stores cleaned data in `Handled Data.xlsx`

---

### **3. `Visualizes and observes`**
- Visualizes administrative boundaries of Ho Chi Minh City by using file `District zoning.geojson`.
- Observes spatial distribution of houses for sale  
- Heatmaps and scatter plots are used to show density
  
<img width="1748" height="989" alt="image" src="https://github.com/user-attachments/assets/9f9a168e-285d-4452-9510-bcfed61a8008" />

---

### **4. `Measures Model Performance and Compares`**

| Model                | MSE        | MAE       | R²        |
|---------------------|------------|-----------|-----------|
| Linear Regression   | 5.450013   | 1.707550  | 0.614092  |
| Ridge Regression    | 5.449884   | 1.707505  | 0.614101  |
| Lasso Regression    | 5.563383   | 1.726661  | 0.606064  |
| Decision Tree       | 6.396784   | 1.840652  | 0.547052  |
| Random Forest       | 4.855765   | 1.571356  | 0.656170  |
| Gradient Boosting   | 5.078654   | 1.621607  | 0.640387  |

A **basic deep learning model** was also trained to compare performance.

<img width="855" height="472" alt="image" src="https://github.com/user-attachments/assets/d8bda4de-33cc-4aa6-b968-4298777d184c" />

---

## Challenges Encountered

### **Web Scraping Difficulties**
- Designing and implementing a scraping algorithm from scratch.
- Difficulties in analyzing inconsistent HTML structures.
- Large-scale scraping required long runtime and stable internet.
- Price differences between:
  - HTML title price  
  - Description price within the same listing  

### **Data Processing Challenges**
- Handling missing values with varying rates across features.
- Many features exhibited strong multicollinearity.
- High outlier ratio made cleaning decisions more difficult.

### **Modeling Challenges**
- Choosing models robust to outliers.
- Understanding trade-offs between simple regressors and more complex models.
- Learning deep learning fundamentals and training rules from scratch.

---

## 🧾 Conclusion

The House Price Prediction project is a comprehensive data science exercise that applies the knowledge we gained from the Introduction to Data Science course. 
Throughout this project, we completed an end-to-end real-world data pipeline and accumulated valuable experience in solving predictive modeling problems. 
From scraping raw data to cleaning, preprocessing, performing exploratory data analysis, and implementing machine learning models, each step strengthened our technical understanding and workflow discipline.

Moreover, the project deepened our insights into the real estate domain and enhanced our ability to collaborate effectively as a dynamic team while tackling challenging issues. 
We believe that the lessons learned from this project will serve as a strong foundation and enable us to go much further in the field of predictive analytics in the future.

---

## 👥 Contributors

- **Pham Le Hong Duc**  
- **Truong Binh Ba**  
- **Bach Ngoc Le Duy**  
- **Hoang Minh Hien**
  
