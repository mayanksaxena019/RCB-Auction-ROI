# RCB Auction ROI Dashboard (2016–2025)

## 📌 Project Overview

This project analyzes the Royal Challengers Bengaluru (RCB) auction strategy from **2016 to 2025** using **Power BI**. The dashboard evaluates player investments, auction spending patterns, squad composition, and player value to understand how effectively RCB utilized its auction budget across multiple IPL seasons.

The project combines **Python (Pandas)** for data cleaning, preprocessing, and feature engineering with **Power BI** for building an interactive business intelligence dashboard.

---

## 🌟 Highlights

- Analyzed **113 RCB player signings** across 10 IPL auction seasons.
- Evaluated **₹317+ Crore** of auction investments.
- Built a **custom Value Score** to estimate player ROI.
- Created an interactive **Power BI dashboard** with dynamic filtering.
- Standardized and merged multiple datasets from different sources.

---

## 🎯 Objectives

- Analyze RCB's auction spending across seasons.
- Compare investments made on different player roles.
- Evaluate Indian vs Overseas player acquisitions.
- Identify the most expensive player signings.
- Measure player value using a custom Value Score metric.
- Build an interactive dashboard for exploring auction trends.

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Power BI Desktop
- Jupyter Notebook
- CSV & JSON Datasets

---

## 📂 Project Workflow

### 1. Data Collection

The analysis combines multiple datasets collected from different publicly available sources. Since these datasets followed different naming conventions and structures, additional preprocessing and standardization were required before analysis.

The datasets include:

- RCB auction records
- Player performance statistics
- Squad information
- Player nationality information

---

### 2. Data Cleaning

The raw datasets were cleaned by:

- Removing duplicate records
- Handling missing values
- Standardizing player names
- Standardizing historical team names
- Cleaning text columns
- Mapping player nationalities
- Mapping missing player roles
- Merging auction and performance datasets

---

### 3. Feature Engineering

Several analytical metrics were engineered to evaluate player investments and auction efficiency, including:

- Total Investment
- Average Cost per Player
- Cost per Run
- Cost per Wicket
- Player Value Score (custom ROI metric)
- Indian vs Overseas player counts

> **Note:**  
> The **Value Score** is a custom analytical metric created solely for this project and is **not an official IPL statistic**.

---

### 4. Dashboard Development

An interactive Power BI dashboard was built featuring:

- KPI Cards
- Auction Spending by Year
- Investment by Player Role
- Top 10 Most Expensive Signings
- Top 10 Best Value Signings
- Interactive slicers and cross-filtering

> **Additional Documentation:**  
> Details regarding dataset limitations, assumptions, player name mappings, team standardization, duplicate player purchases, and the custom Value Score methodology are documented in **DATA_CHALLENGES.md**.

---

## 📊 Dashboard Preview
<img width="1367" height="938" alt="image" src="https://github.com/user-attachments/assets/4b7c6ae0-57ae-4c57-ab54-17a61becc9d4" />

---

## 📈 Dashboard Features

### KPI Cards

- Players Signed
- Total Investment
- Average Cost per Player
- Overseas Players
- Indian Players

### Visual Analytics

- 📊 Auction Spending by Year
- 🍩 Investment by Player Role
- 💰 Top 10 Most Expensive Signings
- ⭐ Top 10 Best Value Signings

### Interactive Filters

- Auction Year
- Player Role
- Nationality

All visuals are interconnected through Power BI cross-filtering, enabling dynamic exploration of auction trends.

---

## 📌 Key Insights

- RCB signed **113 players** between **2016–2025**.
- Total auction investment exceeded **₹317 Crore**.
- All-Rounders accounted for the highest share of auction spending.
- Overseas players represented approximately **40%** of total signings.
- Several lower-cost signings delivered better value than high-profile expensive acquisitions based on the custom Value Score.


---

## 🚀 How to Use

### Clone the repository

```bash
git clone https://github.com/yourusername/RCB-Auction-ROI-Dashboard.git
```

### Install the required libraries

```bash
pip install -r requirements.txt
```

### Run the notebook

Execute the Jupyter Notebook to reproduce the cleaned dataset and engineered features.

### Open the dashboard

Open the `.pbix` file using **Power BI Desktop** to explore the interactive dashboard.

---

## 💡 Skills Demonstrated

- Python (Pandas)
- Data Cleaning
- Data Transformation
- Data Integration
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Power BI
- Dashboard Design
- Business Intelligence
- Data Visualization
- KPI Development

---

## 🚀 Future Improvements

- Incorporate fielding statistics into the Value Score.
- Compare RCB's auction strategy with other IPL franchises.
- Add player retention analysis.
- Include season-wise team performance alongside auction spending.
- Enhance the Value Score using advanced statistical weighting.

---

## 📬 Feedback

Contributions, suggestions, and feedback are welcome.

If you found this project useful or interesting, consider giving the repository a ⭐.
