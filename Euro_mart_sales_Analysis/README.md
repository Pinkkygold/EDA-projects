
# EuroMart Sales Analysis  

![Python](https://img.shields.io/badge/python-3.9-blue)  
![License](https://img.shields.io/badge/license-MIT-green)  

## 📑 Table of Contents  
1. [Project Overview](#-project-overview)  
2. [Dataset Information](#-dataset-information)  
3. [Data Processing & Feature Engineering](#-data-processing--feature-engineering)  
4. [Key Business Insights](#-key-business-insights)  
5. [Recommendations](#-recommendations)  
6. [Technical Implementation](#-technical-implementation)  
7. [Future Work](#-future-work)  
8. [How to Run](#-how-to-run)  

---

## 📊 Project Overview  
This project analyzes **EuroMart’s sales data (2011–2014)** to uncover business insights, identify performance patterns, and provide **data-driven recommendations** to improve profitability and operational efficiency.  

---

## 📁 Dataset Information  
- **File**: `EuroMart_Stores.csv`  
- **Records**: 8,047 transactions  
- **Time Period**: 2011–2014  
- **Features**: 18 columns covering customer details, product attributes, financial metrics, and geography  

---

## 🛠️ Data Processing & Feature Engineering  

### 🔹 Data Cleaning  
- Removed unnecessary `Unnamed: 0` column  
- Verified no missing values or duplicates  
- Converted discount percentages from decimal → integer format  

### 🔹 Feature Engineering  
- **Temporal Features**: Year, Month, Quarter, Season extracted from Order Date  
- **Financial Metrics**:  
  - `Total Sales = Sales × Quantity`  
  - `Total Profit = Profit × Quantity`  
  - `Discount Amount = Total Sales × Discount %`  
  - `Net Sales = Total Sales − Discount Amount`  
  - `Net Profit = Total Profit − Discount Amount`  

---

## 📈 Key Business Insights  

### 🚩 Red Flags  
1. **Unstable Profitability** – Wide fluctuations across all financial metrics  
2. **Discount Volatility** – 50% of orders without discounts vs. some at 85%  
3. **Unprofitable Orders** – Negative profits lowering overall margins  

### 📊 Performance Metrics  
- Avg. Order Value: **$292**  
- Avg. Profit per Order: **$35**  
- Typical Quantity: **3 units**  
- Avg. Discount: **11%** (range: 0–85%)  

### 🌍 Geography  
- Primary Market: **France** (1,916 orders)  
- Key Region: **Central Europe** (55% of orders)  
- Top City: **London** (219 orders)  

### 🏢 Business Patterns  
- Segment: **Consumer** (52% of orders)  
- Shipping: **Economy** (60%)  
- Category: **Office Supplies** (66%)  

### 📅 Seasonality  
- Peak Month: **August** (1,132 orders)  
- Strongest Quarter: **Q4** (51% of annual sales)  
- Best Season: **Summer** (2,457 orders)  

> 📸 *Sample visualizations (add screenshots here)*  
> - ***Sales by Month***
> - <img width="1189" height="390" alt="image" src="https://github.com/user-attachments/assets/bda6b20a-5f69-4c8f-af2e-d7a47adef63c" />


> - ***Profitability Heatmap***
>   
> - <img width="1389" height="990" alt="image" src="https://github.com/user-attachments/assets/07a2dcf4-8477-4924-8ccf-03e3536cc18f" />


> - ***Discounts Distribution***
>   
> - <img width="871" height="547" alt="image" src="https://github.com/user-attachments/assets/75ecf731-0227-448f-ad84-da20e6504fa7" />


---

## 🎯 Recommendations  

### Immediate Actions  
- Standardize discount strategy to reduce volatility  
- Investigate loss-making transactions to minimize profit leaks  
- Optimize inventory for high-performing products (e.g., *Eldon File Cart, Single Width*)  

### Strategic Initiatives  
- Build **VIP programs** for repeat customers (e.g., Joel Peters)  
- Prioritize **Q4 & Summer** for campaigns and resource allocation  
- Strengthen **Central Europe** market penetration  
- Diversify beyond **Office Supplies** to reduce dependency  

---

## 📊 Technical Implementation  

### Libraries  
- `pandas`, `numpy`, `matplotlib`, `seaborn`  

### Analysis Performed  
- Descriptive statistics  
- Univariate analysis  
- Temporal trend analysis  
- Profitability assessment  
- Customer segmentation patterns  

---

## 🔮 Future Work  
- Predictive sales forecasting (ARIMA, Prophet, LSTMs)  
- Customer Lifetime Value (CLV) modeling  
- Real-time BI dashboard integration  
- A/B testing for discount effectiveness  
- Classification models to flag **high-risk (loss-making) orders**  

---
