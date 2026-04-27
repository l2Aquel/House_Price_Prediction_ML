# House_Price_Prediction_ML

## 1. Project Title / Headline  
An end-to-end Machine Learning pipeline that predicts house prices based on key property features, deployed as an interactive Streamlit web application.

## 2. Short Description / Purpose  
This project transforms raw Indian housing data into a deployable price prediction tool. By analyzing features like living area, bedrooms, bathrooms, house condition, and nearby schools, the model estimates market price — served through a simple web app that requires no coding to use.

## 3. Tech Stack  
- **Python** - Data analysis, modeling, and app development
- **Pandas/Numpy** - Data loading, exploration, and preprocessing
- **Matplotlib & Seaborn** – Exploratory visualizations 
- **Scikit-learn** – Model training, GridSearchCV tuning and evaluation
- **Joblib** – Model serialization (model.pkl)
- **Streamlit** – Interactive web application
- **File Format** – `.ipynb` ,`.py`,`.pkl` and `.csv`


## 4. Data Source  

- Source: Kaggle–House Prices India
- Volume: 14,619 rows × 23 columns, No missing values, No duplicates
- Target Variable: price (Range: ₹78,000 – ₹77,00,000 | Mean: ₹5,38,806)
- Feature Variables: number_of_bedrooms, number_of_bathrooms, living_area, condition_of_the_house, number_of_schools_nearby


## 5. Features / Highlights

### Model Comparison (GridSearchCV, 80/20 Split)

To offer a 360° view of sales performance across:
- Product-level trends and return rates
- Customer-level revenue insights
- Country-wise and category-wise demand
- Periodic profit/revenue tracking vs. targets

### • Walkthrough of Key Visuals

#### KPI Cards (Top Row)
- **Revenue**: $24.9M  
- **Profit**: $10.5M  
- **Orders**: 25.2K  
- **Return Rate**: 2.2%

#### Trend Analysis
- **Monthly Revenue**: Upward trend with 3.31% MoM growth  
- **Monthly Orders/Returns**: Interactive YoY and MoM comparisons  
- **Profit vs. Target**: Visual gauge and actuals line

#### Product Insights
- **Most Ordered Category**: Accessories (17K orders)  
- **Most Returned Product Type**: Shorts  
- **Top Products by Orders & Return %**:  
  - Water Bottle – 30 oz. (3,983 orders, 1.95% return)
  - Patch Kit, Tire Tubes, Helmets, etc.

#### Geo Breakdown
- 🇺🇸 United States
- 🇨🇦 Canada
- 🇫🇷 France
- 🇬🇧 UK
- 🇦🇺 Australia
- 🇩🇪 Germany

#### Customer Segmentation
- 17.4K Unique Customers  
- Avg Revenue per Customer: $1,431  
- Top Customer: Mr. Maurice Shan ($12.4K from 6 orders)  
- Segments by:
  - **Income Level** (Low, Avg, High)
  - **Occupation** (Professional, Skilled Manual, Management)


## 6. Business Impact & Insights

- Living area, condition, and nearby schools are the strongest price drivers
- Random Forest outperformed both Linear Regression and Decision Tree, reflecting non-linear relationships in the data
- The Streamlit app makes price estimation accessible to buyers, sellers, and agents — no data science background needed

## 6. SQL Logic and Insights

1. Total Revenue Check: Calculate the total revenue generated in millions for the entire dataset with the currency.
> SELECT CONCAT('$',ROUND(SUM(order_quantity * product_price)/1000000,1),'M') as overall_sales
FROM sales_data s
JOIN product_lookup p
ON s.product_key = p.product_key;


## 7. Screenshots / Demos  
![https://github.com/l2Aquel/AdventureWorks_Dashboard/blob/main/AdventureWorks_preview.png](AdventureWorks_preview.png)
![https://github.com/l2Aquel/Adventure_Works/blob/main/PostgreSQL.png](PostgreSQL.png)
