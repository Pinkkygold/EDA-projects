# EuroMart Sales Analysis

## 📊 Project Overview
This project analyzes EuroMart's sales data from 2011-2014 to uncover business insights, identify performance patterns, and provide data-driven recommendations for improving profitability and operational efficiency.

## 📁 Dataset Information
- **File**: `EuroMart_Stores.csv`
- **Records**: 8,047 transactions
- **Time Period**: 2011-2014
- **Features**: 18 original columns including customer information, product details, sales metrics, and geographical data

## 🛠️ Data Processing & Feature Engineering

### Data Cleaning
- No missing values or duplicates found
- Removed unnecessary `Unnamed: 0` column
- Converted discount percentages from decimal to integer format

### Feature Engineering
- **Temporal Features**: Extracted Year, Month, Quarters, and Seasons from Order Date
- **Financial Metrics**:
  - Total Sales = Sales × Quantity
  - Total Profit = Profit × Quantity
  - Discount Amount = Total Sales × Discount Percentage
  - Net Sales = Total Sales - Discount Amount
  - Net Profit = Total Profit - Discount Amount

## 📈 Key Business Insights

### 🚩 Critical Red Flags
1. **Profit Inconsistency**: High standard deviation across all financial metrics indicates unstable profitability
2. **Discount Strategy Issues**: 50% of orders have no discount vs. some orders with 85% discount
3. **Loss-making Orders**: Significant negative profits affecting overall performance

### 📊 Performance Metrics
- **Average Order Value**: $292
- **Average Profit per Order**: $35
- **Typical Quantity**: 3 units per order
- **Average Discount**: 11% (highly volatile: 0-85%)

### 🌍 Geographical Concentration
- **Primary Market**: France (1,916 orders)
- **Key Region**: Central region dominates (55% of total orders)
- **Major City**: London (219 orders)

### 🏢 Business Patterns
- **Top Segment**: Consumer (52% of orders)
- **Preferred Shipping**: Economy (60% of orders)
- **Leading Category**: Office Supplies (66% of orders)

### 📅 Seasonal Trends
- **Peak Month**: August (1,132 orders)
- **Strongest Quarter**: Q4 (51% of annual sales)
- **Best Season**: Summer (2,457 orders)

## 🎯 Recommendations

### Immediate Actions
1. **Standardize Discount Strategy**: Reduce discount volatility and establish clear discount policies
2. **Analyze Loss-making Orders**: Identify characteristics of unprofitable transactions
3. **Optimize Inventory**: Focus on high-performing products like "Eldon File Cart, Single Width"

### Strategic Initiatives
1. **Customer Segmentation**: Develop VIP programs for high-frequency customers like Joel Peters
2. **Seasonal Planning**: Allocate resources for Q4 and Summer peaks
3. **Regional Focus**: Strengthen presence in Central Europe markets
4. **Product Diversification**: Expand beyond Office Supplies dominance

## 📊 Technical Implementation

### Libraries Used
- pandas
- numpy
- matplotlib
- seaborn

### Analysis Performed
- Descriptive statistics
- Univariate analysis
- Temporal trend analysis
- Profitability assessment
- Customer behavior patterns

## 🔮 Future Work
- Implement predictive modeling for sales forecasting
- Develop customer lifetime value analysis
- Create dashboard for real-time business monitoring
- Conduct A/B testing for discount strategies

---

*This analysis provides actionable insights to improve EuroMart's profitability and operational efficiency through data-driven decision making.*
