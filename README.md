# Global Shark Attack Analysis 🦈

This repository contains an Exploratory Data Analysis (EDA) and statistical reasoning project based on the Global Shark Attack File (GSAF). 

The goal of this project is to take a messy, web-scraped dataset of historical human-shark interactions and apply rigorous data preprocessing, visualization, and basic statistical inference to uncover underlying demographic trends and reporting biases.

## 📂 Repository Contents

* **`shark_attack_analysis.ipynb`**: The main Jupyter Notebook containing all Python code, data cleaning steps, visualizations, and written interpretations.
* **`attacks.csv`**: The raw dataset containing over 6,000 reported incidents, including features like Date, Year, Victim Age, Activity, Species, and Fatality status.
* **`README.md`**: Project documentation and setup instructions.

---

## 🚀 How to Open and Run the Project

This project is designed to be fully reproducible and runs seamlessly in the cloud using **Google Colab**. You do not need to install Python, download any files, or configure a local environment.

**Step 1: Open the Notebook**
Click the badge below to open the notebook directly in your browser:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SirojWongpitakroj/shark-attack-analysis/blob/main/Shark_Attacks_Analysis.ipynb)

**Step 2: Run the Code**
1. Once inside Google Colab, go to the top menu and click **Runtime > Run all**.
2. **Zero Setup Required:** The notebook is programmed to automatically fetch the `attacks.csv` dataset directly from this GitHub repository using its Raw URL. **You do not need to manually upload the dataset to Colab.**

---

## 📊 What the Notebook Does

The `.ipynb` file is structured as an end-to-end data science report, walking through the following phases:

### 1. Data Preprocessing & Cleaning
Real-world data is inherently messy. The notebook demonstrates data wrangling by:
* Extracting strictly numeric values from inconsistent text strings (e.g., cleaning the `Age` column).
* Standardizing categorical variables (e.g., grouping thousands of unique victim activities into primary categories like "Surfing" and "Swimming").
* Handling missing values logically without introducing artificial bias into the demographic statistics.

### 2. Descriptive Statistics
Calculates and interprets key measures of center and spread. The notebook specifically contrasts sensitive metrics (Mean and Standard Deviation) against robust metrics (Median and IQR) to prove the right-skewed nature of victim age demographics.

### 3. Exploratory Data Analysis (EDA)
Generates professional-grade visualizations using `matplotlib` and `seaborn` to satisfy core statistical comparisons:
* **Distribution:** Histograms and line graphs analyzing demographic spread and temporal reporting trends.
* **Group Comparisons:** Side-by-side boxplots and bar charts evaluating fatality rates across different activities and shark species.
* **Relationship Exploration:** Scatterplots demonstrating the correlation between reporting volume and fatality rates over time.

### 4. Basic Statistical Inference
Focuses on statistical reasoning, conditional probability, and base-rate interpretation. Key findings include:
* **Survivorship Bias:** Using conditional probability to show how fatal outcomes mask the identification of apex predators, causing the "Unknown" species category to artificially reflect the highest fatality rate.
* **Reporting Bias (The Safety Paradox):** Interpreting the massive post-1990 spike in attacks not as a biological shift, but as a shift in the *base rate of reporting* due to the internet and modern media capturing non-fatal incidents that were historically ignored.
