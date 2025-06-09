# Hyderabad-Rental-Houses-Web-Scraping-Data-Analysis


This project involves **web scraping rental listings of independent houses in Hyderabad** from [Housing.com](https://housing.com), followed by data cleaning, feature extraction, and in-depth Exploratory Data Analysis (EDA) to uncover meaningful rental trends and patterns.

---

## Problem Statement

House seekers in Hyderabad often face challenges accessing well-organized and insightful rental data. While websites like Housing.com have rich property listings, they do not provide options to download or analyze the data directly. This project aims to **scrape**, **structure**, and **analyze** that data to support informed rental decisions.

---

##  Project Objectives

- Scrape rental listings for independent houses/villas from Housing.com.
- Extract features like BHK, area (sqft), rent, furnishing, and more.
- Clean and preprocess raw data for analysis.
- Conduct univariate, bivariate, and multivariate analysis.
- Derive insights on rent pricing, area-wise trends, and feature influences.

---

##  Tools & Libraries Used

- `Python`
- `BeautifulSoup`, `requests`
- `pandas`, `numpy`, `re`
- `matplotlib`, `seaborn`

---

##  Dataset Summary

- **Source**: [Housing.com](https://housing.com)
- **Total Listings**: ~800 houses (from 32 pages)
- **Key Features**:
  - Address, BHK, Area (sqft), Rent, Furnishing, Parking
  - Bathrooms, Balconies, Posting Date
  - Derived: City, Primary Location, Day of Week, Posted Month

---

##  EDA Highlights

###  Univariate Analysis:
- Most houses are **2 BHK** with **2 bathrooms**, area typically **500–1300 sqft**.
- Majority rents fall between **₹8,000 – ₹18,000**.
- Semi-furnished homes dominate (~45%).

###  Bivariate/Multivariate Analysis:
- **Rent** increases with **balconies, furnishing quality, and area**.
- **Area (sqft)** has stronger correlation with rent (0.53) than BHK or bathrooms.
- **Manikonda** shows the highest average rent (~₹21.3K), while **Prem Nagar** is among the cheapest.

---

##  Visuals & Insights

- Histograms, boxplots, scatter plots, heatmaps, violin plots
- Correlation matrix to analyze feature relationships
- Posting pattern analysis by weekday and time

---

##  How to Run

```bash
# Clone the repository
git clone https://github.com/yourusername/hyderabad-rentals-analysis.git
cd hyderabad-rentals-analysis

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook Housing_data_webscrapping.ipynb
