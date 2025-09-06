# 🎮 Video Game Sales Forecasting  
*Market analysis and forecasting of video game sales to support Ice’s 2017 marketing campaign strategy.*  

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)  
![pandas](https://img.shields.io/badge/pandas-EDA-green?logo=pandas)
![numpy](https://img.shields.io/badge/numpy-Numerical-blue?logo=numpy) 
![matplotlib](https://img.shields.io/badge/matplotlib-Visualization-orange)  
![scipy](https://img.shields.io/badge/scipy-Stats-lightblue?logo=scipy)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter) 
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)  

---

## 📌 Overview  
Ice, an online video game retailer, seeks to identify **potential best-sellers for 2017** and allocate advertising resources accordingly. This project analyzes historical video game sales data, critic/user reviews, platforms, genres, and regional preferences to provide actionable recommendations.  

---

## 📊 Dataset  
- **Source:** Aggregated open datasets (games, reviews, platforms, regional sales).  
- **Key Features:**  
  - `name`, `platform`, `year_of_release`  
  - `genre`, `critic_score`, `user_score`, `rating`  
  - `na_sales`, `eu_sales`, `jp_sales`, `other_sales`  
- **Preprocessing:**  
  - Missing value handling (median fill for scores, “No Rating” label for rating)  
  - Type conversions (e.g., user score to float)  
  - Creation of `total_sales` feature  

---

## ⚙️ Methods & Tools  
- **Libraries:** pandas, matplotlib, scipy  
- **Techniques:**  
  - Data cleaning and feature engineering  
  - Descriptive and comparative sales analysis  
  - Regional profiling (NA, EU, JP)  
  - Hypothesis testing with `scipy.stats.ttest_ind`  

---

## 📈 Results  
- **Platforms:**  
  - NA/EU: **PS4** and **Xbox One** lead sales, early in lifecycle → strong future growth  
  - JP: **3DS** dominates, highlighting a cultural preference for handhelds  
  - Legacy platforms (PS3, Xbox 360, Wii) are in decline and should not be prioritized  

- **Genres:**  
  - NA/EU: Action, Sports, and Shooter titles dominate  
  - JP: Role-Playing leads, followed by Action  
  - Cultural differences drive genre appeal across markets  

- **ESRB Ratings:**  
  - NA/EU: Mature (M) titles have highest sales → indicates aging gamer demographic  
  - JP: Sales largely unaffected by ESRB ratings (local systems dominate)  

- **Hypothesis Testing:**  
  - No significant difference in **Xbox One vs PC user ratings** → cross-platform parity likely driven by shared releases  
  - Significant difference in **Action vs Sports ratings** → cultural and market differences shape user perception  

---

## 💡 Key Insights  
- Prioritize **PS4 and Xbox One campaigns** in western markets (early lifecycle, strong sales trajectory).  
- In Japan, emphasize **mobile/handheld platforms** (3DS, PS Vita, next-gen handhelds).  
- Focus advertising on **Action, Shooter, and Sports** titles in NA/EU; **RPGs** in JP.  
- Highlight **M-rated titles** in western campaigns for maximum ROI.  
- Critic scores have minimal direct impact but can supplement pre-launch hype.  

---

## 🗂 Repo Structure  
```
video-game-sales-forecasting/
├── notebooks/ <- Final cleaned Jupyter notebook
├── data/ <- Video game sales dataset
├── requirements.txt <- Dependencies
├── LICENSE <- MIT License
└── README.md <- This file
```

---

## 🚀 How to Run  
1. Clone the repo:  
   ```bash
   git clone https://github.com/Flamingo-Rocker/video-game-sales-forecasting.git
   cd video-game-sales-forecasting
2. Install dependencies:
    ```bash
    pip install -r requirements.txt
3. Open the notebooks in `/notebooks` to follow the full workflow.

---

## 📦 Requirements  
```
pandas==2.3.2
numpy==2.2.5
numpy-base==2.2.5            
numpydoc==1.9.0            
matplotlib==3.10.5           
matplotlib-base==3.10.5           
matplotlib-inline==0.1.6
seaborn==0.13.2         
plotly==6.3.0           
mpmath==1.3.0            
sphinxcontrib-jsmath==1.0.1            
scipy==1.16.0           
mkl_random==1.2.8        
```

---

## 🙏 Acknowledgment
Developed as part of the TripleTen Data Science Bootcamp, applying statistical data analysis and hypothesis testing to forecast video game sales and guide marketing strategies.
