# STATA Project: What Really Drives Firm Profitability?

## About This Project
I built this project to answer a simple but important question:

**What actually makes a company profitable?**

Using STATA, I analyzed firm-level financial and operational data to uncover the key drivers behind profit margins. This project walks through the full data analysis process from cleaning the data to running econometric models.

---

## Objective
The goal of this analysis is to:

Identify which factors influence firm profitability
Apply econometric techniques using STATA
Generate real-world, actionable business insights

---

## Dataset
The dataset contains **500 observations** with the following variables:

`revenue` – Total firm revenue  
`expenses` – Total firm costs  
`employees` – Number of employees  
`rd_spend` – Research & Development spending  
`debt` – Total debt  
`profit_margin` – Profitability (target variable)  

---

## Step 1: Understanding the Data (EDA)

I started by exploring the dataset to understand general patterns.

### What stood out:
Firms vary a lot in terms of revenue and expenses
Profitability is not consistent across firms
Some firms are clearly more efficient than others

### Correlation insights:
Revenue and expenses move together (as expected)
Higher debt tends to reduce profitability
R&D spending shows a positive relationship with profit

**Early takeaway:**  
Innovation seems to help, while too much debt hurts.

---

## Step 2: Regression Analysis

### Basic Model
I first ran a regression using the raw variables.

**What I found:**
Revenue → increases profit margin  
Expenses → reduce profit margin  
Debt → negatively impacts profitability  
R&D → positively impacts profitability  

This confirms that both **cost control and investment decisions matter**.

---

### Improved Model
I then created better variables like:
Revenue per employee (efficiency)
Debt ratio

**New insights:**
**Revenue per employee became the strongest predictor**
Debt ratio had a clear negative effect
R&D remained consistently positive
Number of employees became less important

**Big insight:**  
It’s not about how big a company is, it’s about how efficient it is.

---

## Step 3: Model Diagnostics

### Multicollinearity (VIF Test)
No serious issues detected

The model is stable and reliable.

---

### Heteroskedasticity Test
Heteroskedasticity was present

I fixed this using **robust standard errors**

This ensures the results are statistically valid.

---

## Step 4: Panel Data Analysis

Since the dataset includes firms over time, I used panel data techniques.

### Fixed vs Random Effects:
The **Hausman test recommended Fixed Effects**

This means:
Each firm has unique characteristics (like management or strategy) that affect profitability.

---

## Key Insights (The Real Value)

### 1. Efficiency > Size
Revenue per employee is the strongest driver of profit  
Companies should focus on productivity, not just growth

---

### 2. Debt Can Hurt Performance
Higher debt ratios reduce profitability  
Firms should be careful with borrowing

---

### 3. Innovation Pays Off
R&D spending consistently improves profit margins  
Investing in innovation is worth it

---

### 4. Costs Still Matter
Expenses have a direct negative impact  
Cost control is critical

---

### 5. Internal Factors Matter More Than You Think
Firm-specific effects are significant  
Strategy and management play a big role

---



## Final Thoughts

This project really showed me how powerful STATA is when it comes to econometric analysis.

**Profitability is driven by efficiency, smart investment, and financial discipline.**



