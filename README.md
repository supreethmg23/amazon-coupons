# Will the Customer Accept the Coupon?
### Exploratory Data Analysis – Module 5 Assignment

---

## Overview
This project analyzes the factors that influence whether a driver accepts a mobile coupon while driving.  

This data is from the UCI Machine Learning Repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios, including the destination, current time, weather, and passenger, and then asks people whether they will accept the coupon if they are the driver. There are three possible answers people can choose from:

“Right away”
“Later, before the coupon expires”
“No, I do not want the coupon”

Using Python (`pandas`, `matplotlib`, `seaborn`, `numpy`), the analysis explores patterns that distinguish drivers who accept coupons from those who do not, focusing first on **bar coupons** and later extending to **independent variables** such as passenger type, weather, occupation, and income.

---

## Objectives
- Investigate how coupon acceptance varies with contextual and demographic factors.  
- Identify customer segments most likely to accept coupons.  
- Provide data-driven recommendations for targeted marketing.

---

## Tools and Libraries
- Python 3.x  
- pandas  
- numpy  
- matplotlib  
- seaborn  

---

## Notebook Link
👉 [View the Jupyter Notebook](coupon_analysis.ipynb)

---

## 🔹 Key Findings

### 1. Initial Bar Coupon Analysis
- Around **41%** of all bar coupons were accepted.  
- Among drivers who visit bars **more than once a month**, acceptance rose to **~73%**.  
- **Younger drivers (<30)** and those **without kids** had the highest acceptance.  
- Drivers who were **not widowed** and frequently went to bars showed significantly higher likelihood of accepting.  
- **Conclusion:** Drivers who are **younger, socially active, and regularly visit bars** are most responsive to bar coupon offers.

---

### 2. Independent Investigations

#### Passenger Analysis
- **With Friends:** Highest acceptance → social context increases likelihood.  
- **With Partner:** Moderate.  
- **Alone:** Lower.  
- **With Kids:** Lowest → family constraints reduce flexibility.  
**Insight:** Social passengers (friends/partners) encourage spontaneous decisions to redeem coupons.

#### Weather and Time Analysis
- **Sunny days:** Highest acceptance.  
- **Rainy days:** Lowest.  
- **Snowy:** Moderate.  
- Across all weather types, acceptance peaked around **2 PM** → drivers are more open during midday travel.  
**Insight:** Drivers are more likely to accept coupons during **pleasant weather** and **daytime hours**.

#### Occupation and Income Analysis
- **Construction & Extraction**, **Healthcare**, **Personal Care & Service**, and **Students** show the **highest coupon acceptance** (often above 0.7).  
- **Farming**, **Protective Service**, and **High-income professions** show the **lowest acceptance** (<0.4).  
- Across all occupations, **lower-income groups (<$50K)** are much more likely to accept coupons.  
**Insight:** Coupon acceptance is highest among **service-based or student occupations** and **lower-income earners**, highlighting the influence of economic motivation.

---

## Visualizations
- Bar plots for:
  - Coupon type (Bar Coupons)  
  - Passenger type  
  - Weather & Time  
  - Occupation & Income  
- Histogram of temperature distribution  

All plots include clear labels, readable scales, and descriptive titles.

---

## Summary & Recommendations
- Focus marketing on **younger, social, and lower-income** drivers.  
- Send offers during **afternoon hours** and **good weather**.  
- Emphasize **service-sector and student audiences**, who demonstrate the highest acceptance levels.  
- Reduce spending on campaigns targeting **high-income professionals**, who show low responsiveness to small discounts.

---

## Project Structure
├── data/
│   └── coupons.csv
├── coupon_analysis.ipynb
└── README.md
