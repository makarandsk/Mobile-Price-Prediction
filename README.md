# Mobile Price Prediction

## Description
This project involves predicting the price range of mobile phones based on various features such as battery power, presence of Bluetooth, clock speed, dual SIM support, front camera megapixels, 4G support, internal memory, mobile depth, weight, number of processor cores, primary camera megapixels, pixel resolution height and width, RAM, screen height and width, talk time, 3G support, touch screen availability, and WiFi support. The target variable is the price range, categorized as 0 (low cost), 1 (medium cost), 2 (high cost), and 3 (very high cost).

## Context
Bob has started his own mobile company and aims to compete with big companies like Apple and Samsung. To estimate the price of mobiles, he has collected sales data from various companies. However, he needs help in understanding the relationship between mobile features and their selling prices. Machine learning techniques will be employed to assist Bob in this endeavor.

## Data Cleaning
In the context of the Mobile Price Prediction project, the following data cleaning steps were performed:

**1. Handling Missing Values**

- Checked for missing values in the dataset using df.info() to get an overview of the data.
- If any missing values were found, appropriate strategies such as imputation or removal of rows/columns with missing values were applied.

**2. Handling Outliers**

- Identified potential outliers in certain features that might negatively impact the model's performance.
- For instance, features like `fc` (front camera megapixels), `px_height` (pixel resolution height), and `px_width` (pixel resolution width) might have extreme values.
- Outliers were handled using techniques such as truncation or transformation to bring them within a reasonable range.

**3. Handling Duplicate Records**
- Checked for and removed any duplicate records in the dataset to avoid redundancy and ensure the uniqueness of each data point.

**4. DataType Conersion**
- Ensured that the data types of features were appropriate. For example, converting categorical variables to the correct data type (e.g., converting 'object' type to 'category').

**5. Addressing Inconsistencies**
- Checked for any inconsistencies in the data, such as typos or variations in categorical values, and corrected them for uniformity.

## Exploratory Data Analysis (EDA)
Explored correlations between different features using pairplots and heatmaps. Noted important correlations, such as a perfect positive correlation between `ram` and `price_range` and highly positive correlations between `pc` and `fc`, as well as `three_g` and `four_g`.

## Conclusion
This project involves predicting the price range of mobile phones based on various features. Through exploratory data analysis and data cleaning, we addressed outliers and identified key correlations. The dataset is then prepared for machine learning models to assist Bob in estimating the prices of his company's mobile phones.
