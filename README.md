# 🏠 Real Estate Sales Dashboard – Power BI

## 📌 Project Overview

The **Real Estate Sales Dashboard** is a Business Analytics mini-project developed using **Microsoft Power BI** to analyze and visualize real estate sales data. The dashboard provides meaningful insights into property sales, revenue trends, city-wise performance, property types, and agent performance.

The project transforms raw sales data into interactive visualizations that help users understand business performance and make data-driven decisions.

## 🎯 Objectives

- Analyze total real estate sales revenue.
- Track the number of deals closed and total area sold.
- Identify the highest-performing property types and cities.
- Analyze monthly sales trends.
- Calculate the average price per square foot.
- Provide interactive filtering for detailed analysis.

## 🛠️ Technologies Used

- **Microsoft Power BI** – Dashboard development and visualization
- **Power Query** – Data cleaning and transformation
- **DAX (Data Analysis Expressions)** – Measures and calculations
- **Excel / CSV** – Data source

## 📊 Dataset Information

The dataset contains the following columns:

| Column | Description |
|---|---|
| `Deal_ID` | Unique deal identifier |
| `Date` | Date of the property sale |
| `Property_Type` | Type of property sold |
| `City` | City where the property was sold |
| `Area_sqft` | Property area in square feet |
| `Agent` | Sales agent responsible for the deal |
| `Sale_Price_INR` | Property sale price in Indian rupees |

## 📈 Dashboard Features

- **KPI Cards:** Total Sales Value, Deals Closed, and Average Price per Square Foot.
- **Monthly Sales Trend:** A line chart showing sales revenue over time.
- **Property Type Analysis:** A clustered bar chart comparing revenue across property types.
- **City-wise Sales Analysis:** A donut chart showing each city's contribution to total sales.
- **Detailed Sales Table:** Displays deal ID, date, property type, city, agent, and sale price.
- **Interactive Slicers:** Filter the dashboard by date, property type, city, and agent.

## 🧮 DAX Measures

The following DAX measures are used in the project:

### 1. Total Sales Value
```dax
Total Sales Value =
SUM(RealEstate[Sale_Price_INR])
```

### 2. Total Area Sold
```dax
Total Area Sold (sqft) =
SUM(RealEstate[Area_sqft])
```

### 3. Deals Closed
```dax
Deals Closed =
COUNTROWS(RealEstate)
```

### 4. Average Price per Square Foot
```dax
Avg Price per sqft =
DIVIDE(
    [Total Sales Value],
    [Total Area Sold (sqft)]
)
```

### 5. Premium Deals
```dax
Premium Deals =
CALCULATE(
    [Deals Closed],
    RealEstate[Sale_Price_INR] > 20000000
)
```

## 🔍 Key Insights

Based on the expected results documented in the project report:

- **Total Sales Value:** ₹174.56 crore.
- **Total Deals Closed:** 100.
- **Average Sales Value per Deal:** Approximately ₹1.75 crore.
- **Premium Deals:** 33 properties sold for more than ₹2 crore.
- **Top Property Type:** Villa, generating ₹53.52 crore in sales.
- **Lowest Property Type:** Studio, generating ₹6.65 crore.
- **Top-Performing City:** Mumbai, contributing ₹37.76 crore.
- **Best Sales Month:** December, with ₹23.52 crore.
- **Weakest Sales Month:** January, with ₹6.75 crore.

*Note: These are the expected figures from the project report. Actual dashboard values should be verified against the dataset and report filters.*

## ⚙️ How to Run the Project

1. Download or clone this repository.
2. Ensure the real estate dataset is available in CSV or Excel format.
3. Open Microsoft Power BI Desktop.
4. Import the dataset using **Home → Get Data**.
5. Check data types and clean the data using Power Query.
6. Create the required DAX measures.
7. Build the KPI cards, line chart, bar chart, donut chart, and detail table.
8. Add interactive slicers for date, property type, city, and agent.
9. Save the dashboard as a `.pbix` file.

## 📌 Conclusion

The Real Estate Sales Dashboard demonstrates how Microsoft Power BI can be used to transform raw real estate sales data into meaningful business insights. Through data cleaning, DAX calculations, KPI cards, and interactive visualizations, the dashboard helps analyze revenue trends, compare property types, evaluate city-wise sales, and assess sales performance.

This project strengthened practical skills in **data analysis, data visualization, Power Query, DAX, and business intelligence**.

## 👨‍💻 Author

**SAI DARSHAN PM**

- **GitHub:** [SAIDARSHAN1402](https://github.com/SAIDARSHAN1402)
- **Portfolio:** [saidarshanpm.netlify.app](https://saidarshanpm.netlify.app)
- **LinkedIn:** [Sai Darshan PM](https://www
