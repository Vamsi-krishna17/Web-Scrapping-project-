# Used Car Resale Price Analysis
Web Scraping & Exploratory Data Analysis (EDA)

**Project Overview**

This project focuses on analyzing used car resale prices by scraping real-world listing data from the Cars24 platform. The objective is to understand how various vehicle attributes and market factors influence resale value across different Indian cities. The project covers the complete data analytics pipeline — data extraction, cleaning, exploratory analysis, and insight generation.

 Web Scraping Methodology

Data was collected from Cars24, an online used-car marketplace

Since listings are location-based, city-wise URLs were used

Data was scraped for major cities such as Delhi, Mumbai, Pune, Hyderabad, Bangalore, Chennai, and others

Python libraries used:

Requests for sending HTTP requests

BeautifulSoup for parsing HTML content

Pandas for storing and processing data

Pagination was implemented to extract multiple pages per city

Each car listing card was identified and required attributes were extracted

Final dataset contains approximately 1,800 used-car records

📊 Dataset Description

Each row in the dataset represents one used-car listing with the following features:

Target Variables: price, final_price

Numerical Features: year, km_driven, emi

Categorical Features: city, brand, fuel_type, transmission

Identifier columns (model, variant) were retained for reference

🧹 Data Cleaning & Preprocessing

To make the dataset analysis-ready, the following steps were performed:

Removed currency symbols (₹), commas, and textual units such as lakh, k, and km

Converted price, final_price, emi, km_driven, and year from text to numeric format

Handled missing values in numerical columns using median imputation to reduce outlier impact

Rows with missing critical categorical values (city, brand, fuel_type, transmission) were dropped (less than 5%)

Ensured consistent data types and standardized text formatting across columns

📈 Exploratory Data Analysis (EDA)

🔹 Univariate Analysis

Distribution of car prices and final prices

Year-wise and kilometer-driven distributions

Frequency analysis of brands, fuel types, transmissions, and cities

🔹 Bivariate Analysis

Price vs vehicle age (year)

Price vs kilometers driven

Price comparison across fuel types and transmission types

City-wise and brand-wise price variations

🔹 Multivariate Analysis

Correlation analysis between numerical variables

Relationship between EMI, price, and final price

Combined analysis of city, fuel type, and transmission to study pricing patterns

🔍 Key Insights

Used-car prices are primarily influenced by vehicle age, EMI, fuel type, transmission, and city

Strong correlation observed between final price and EMI (0.70)

Newer vehicles generally command higher resale value

Mileage affects pricing in a non-linear manner

Automatic and premium-brand cars have higher average resale prices

✅ Conclusion

This project demonstrates how real-world used-car data can be effectively collected, cleaned, and analyzed to derive meaningful insights. The results show that resale pricing depends more on vehicle condition, usage, and affordability indicators than on brand alone. City-wise demand and transmission type also significantly influence prices. Overall, the project strengthened my practical skills in web scraping, data preprocessing, and exploratory data analysis, and provided valuable exposure to solving real-world business problems using data
