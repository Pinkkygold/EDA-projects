# Car Price Analysis - Exploratory Data Analysis (EDA)

## 📁 Project Overview
This project performs an in-depth Exploratory Data Analysis (EDA) on a used cars dataset to understand the factors influencing car prices in the Indian market. The analysis covers data cleaning, feature engineering, and comprehensive visualization to extract meaningful insights about used car pricing patterns.

## 📊 Dataset Information
- **Source**: `used_cars_data.csv`
- **Records**: 7,253 used car listings
- **Features**: 14 original columns covering various car attributes

### Original Features:
- `S.No.`: Serial number
- `Name`: Car name and model details
- `Location`: City where the car is located
- `Year`: Manufacturing year
- `Kilometers_Driven`: Total distance traveled
- `Fuel_Type`: Type of fuel (CNG, Diesel, Petrol, etc.)
- `Transmission`: Manual or Automatic
- `Owner_Type`: First, Second, Third, or Fourth owner
- `Mileage`: Fuel efficiency with units
- `Engine`: Engine capacity with units
- `Power`: Engine power with units
- `Seats`: Number of seats
- `New_Price`: Original price (mostly missing)
- `Price`: Current selling price (target variable)

## 🛠️ Data Processing Steps

### 1. Data Cleaning & Handling
- **Missing Values Treatment**:
  - Price: Filled with mean values
  - Mileage: Split into numeric values and units, converted to uniform kmpl
  - Engine: Extracted CC values, filled missing with 0
  - Power: Extracted bhp values, filled missing with 0
  - Seats: Filled with mode value

### 2. Feature Engineering
- **Car_Age**: Calculated from manufacturing year to current date
- **Brand**: Extracted from car name (first word)
- **Model**: Extracted from car name (second and third words)
- **Mileage(kmpl)**: Standardized fuel efficiency metric
- **Engine(CC)**: Numeric engine capacity
- **Power(bhp)**: Numeric power rating

### 3. Data Reduction
Removed redundant columns:
- `S.No.`, `New_Price`, `Mileage`, `Engine`, `Power`, `Unit`

## 🔍 Key Analysis Areas

### Descriptive Analysis
- **Year Distribution**: Cars from 1996-2019
- **Kilometers Driven**: Average ~58k KM (with outliers)
- **Fuel Type Distribution**: Mostly Diesel (3,852 vehicles)
- **Transmission**: Predominantly Manual (5,203 vehicles)
- **Owner Type**: Mostly First owners (5,951 vehicles)
- **Seating Capacity**: Average 5.27 seats

### Statistical Insights
- **Price Range**: ₹0.44L - ₹160L (average ₹9.48L)
- **Mileage**: 0-46.96 kmpl (average 18.24 kmpl)
- **Engine Capacity**: 0-5998 CC (average 1606 CC)
- **Power**: 0-616 bhp (average 110 bhp)
- **Car Age**: 6-29 years (average 11.63 years)

## 📈 Key Findings

### Market Trends
- **Most Popular Brand**: Maruti (1,444 listings)
- **Most Popular Model**: Swift Dzire (189 listings)
- **Top Location**: Mumbai (948 listings)
- **Fuel Preference**: Diesel dominates the used car market
- **Transmission**: Manual transmission preferred (90% of listings)

### Price Influencers
- **Age Impact**: Older cars generally priced lower
- **Mileage**: Higher mileage correlates with lower prices
- **Engine & Power**: Direct relationship with price
- **Brand Value**: Premium brands (Audi, BMW) command higher prices

## 🎯 Analysis Goals Achieved

✅ **Descriptive Analysis**: Comprehensive summary of all key features  
✅ **Data Quality**: Handled missing values and duplicates effectively  
✅ **Feature Engineering**: Created meaningful derived features  
✅ **Outlier Detection**: Identified data quality issues and extreme values  
✅ **Market Understanding**: Gained insights into used car pricing patterns  

## 🛠️ Technical Stack
- **Python Libraries**: Pandas, NumPy, Matplotlib, Seaborn
- **Data Visualization**: Comprehensive plots and statistical summaries
- **Data Processing**: Advanced feature engineering and cleaning techniques

## 📋 Files Structure
- `Car_Price_Analysis.ipynb`: Main analysis notebook
- `used_cars_data.csv`: Original dataset ( included in repository)

## 🚀 Potential Applications
- Used car price prediction models
- Market trend analysis for automotive industry
- Investment decisions for used car dealerships
- Consumer guidance for car purchases

This analysis provides a solid foundation for building predictive models and offers valuable insights for stakeholders in the used car market ecosystem.
