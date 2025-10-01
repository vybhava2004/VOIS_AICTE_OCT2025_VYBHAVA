# 🏡 Airbnb Data Visualization Project  

This project explores an Airbnb dataset using **Python data visualization frameworks** such as **Pandas, Matplotlib, and Seaborn**.  
The goal is to clean the dataset and answer key analytical questions through **interactive visualizations**.  

---

## 📌 Project Objectives  

The project aims to:  
1. **Clean and preprocess** raw Airbnb data.  
2. **Handle missing values, duplicates, outliers, and inconsistent formats.**  
3. **Analyze and visualize** the dataset using plots such as bar, line, scatter, and box plots.  
4. **Answer 9 critical business questions** about property types, neighborhoods, hosts, and reviews.  

---

## 🗂️ Dataset Description  

The dataset (`Airbnb_Open_Data.xlsx`) contains Airbnb listings with features such as:  
- `id` → Listing ID  
- `name` → Property name  
- `host id`, `host name`, `host_identity_verified`  
- `neighbourhood group`, `neighbourhood`  
- `room type`, `price`, `service fee`  
- `availability 365` → Availability in days  
- `number of reviews`, `review rate number`  
- `calculated host listings count`  
- `house_rules`, `license` (dropped due to insufficient data)  

---

## 🧹 Data Cleaning Steps  

The following steps were applied before visualization:  

1. Drop duplicate records  
2. Drop `house_rules` and `license` columns  
3. Remove commas and dollar signs from `price` and `service fee`  
4. Rename `price` → `price_$`, `service fee` → `service_fee_$`  
5. Drop rows with missing values  
6. Convert mismatched data types (e.g., `availability 365`)  
7. Correct spelling of **brookln → Brooklyn**  
8. Remove outliers in `availability 365` (> 365 days)  

---

## 📊 Analysis Questions  

We answer the following **9 questions** with plots:  

1. **What are the different property types in the dataset?**  
   → Count of `room type` categories.  

2. **Which neighborhood group has the highest number of listings?**  
   → Bar chart of `neighbourhood group` frequency.  

3. **Which neighborhood group has the highest average prices?**  
   → Average `price_$` by `neighbourhood group`.  

4. **Is there a relationship between construction year and price?**  
   → Scatterplot (`construction year` vs `price_$`).  

5. **Who are the top 10 hosts by listing count?**  
   → Bar chart of top `host name` by `calculated host listings count`.  

6. **Are verified hosts more likely to receive positive reviews?**  
   → Boxplot comparing `review rate number` across `host_identity_verified`.  

7. **Is there a correlation between price and service fees?**  
   → Scatterplot + correlation coefficient.  

8. **What is the average review rating, and does it vary by neighborhood group and room type?**  
   → Grouped bar chart by `neighbourhood group` and `room type`.  

9. **Are hosts with higher listing counts more likely to maintain higher availability?**  
   → Scatterplot (`calculated host listings count` vs `availability 365`).  

---

## 🖼️ Visualization Methods  

We used:  
- **Bar Plots** → for counts and averages  
- **Scatter Plots** → for correlations and relationships  
- **Box Plots** → for distribution comparisons  
- **Count Plots** → for categorical frequency analysis  

---

## 🛠️ Tech Stack  

- **Python 3.10+**  
- **Pandas** → Data handling & cleaning  
- **Matplotlib** → Basic visualizations  
- **Seaborn** → Advanced statistical plots  
- **Jupyter Notebook** → Interactive analysis  

---

## 🚀 How to Run the Project  

1. Clone this repository:  
   ```bash
   git clone https://github.com/vybhava2004/VOIS_AICTE_OCT2025_VYBHAVA.git
   cd VOIS_AICTE_OCT2025_VYBHAVA

2. Install dependencies:

   pip install pandas matplotlib seaborn jupyter


3. Open Jupyter Notebook:

   jupyter notebook


4. Run the notebook Airbnb_Data_Visualization.ipynb step by step.

📌 Project Structure
├── Airbnb_Open_Data.xlsx         # Dataset
├── Airbnb_Data_Visualization.ipynb  # Main analysis notebook
├── README.md                     # Project documentation

# 📈 Sample Insights

Entire home/apt is the most common room type.

Manhattan has the highest number of listings and highest average prices.

Verified hosts tend to have slightly higher review ratings.

There is a positive correlation between price and service fees.

Top hosts manage multiple properties and maintain higher availability.

# 🔮 Future Improvements

Build an interactive dashboard using Plotly/Dash.

Perform predictive modeling (e.g., price prediction).

Explore geospatial visualization with Folium/Geopandas.

# 👨‍💻 Author

CHAVALA VYBHAVA RAGHAVA SAI