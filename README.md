# 🚕 NYC Yellow Taxi Data Transformation Project

## 📋 Project Overview
This project focuses on **cleaning** and **transforming** the New York City Yellow Taxi Trip Data from **March 2020**. The dataset contains detailed information about taxi trips including **pickup/dropoff times**, **locations**, **fare amounts**, and **passenger counts**.

## 📊 Dataset Information
- **Source**: [Kaggle - NYC Yellow Taxi Trip Data 2020-2019](https://www.kaggle.com/datasets/microize/newyork-yellow-taxi-trip-data-2020-2019)
- **File**: `yellow_tripdata_2020-03.csv`
- **Time Period**: **March 2020**
- **Original Size**: Varies based on the month

## 🛠️ Data Transformation Process

### 1. **Data Loading & Initial Setup**

### 2. **Data Quality Assessment & Cleaning**

#### ✅ **Null Value Treatment**
#### ✅ **Duplicate Detection & Removal**

### 3. **Feature Engineering**

#### 📅 **Pickup DateTime Transformation**
#### 📅 **Dropoff DateTime Transformation**  

#### 🔢 **Data Type Optimization**
Converted **decimal values** to **integers** for the following columns:
- **VendorID**, **passenger_count**, **RatecodeID**
- **PULocationID**, **DOLocationID**, **payment_type**

#### 4. **Data Modeling & Export**
#### 🏗️ **Dimensional Modeling**
Created **three separate tables** following data warehousing best practices:
📊 **Fact Table** (fact_table.csv)

fare_amount, extra, mta_tax, total_amount
tip_amount, tolls_amount, improvement_surcharge, congestion_surcharge

📅 **Date Dimension** (dim_date.csv)

Pickup: Date, Year, Month, Day, Hour, Min
Dropoff: Dropoff_Date, Dropoff_Year, Dropoff_Month, Dropoff_Day, Dropoff_Hour, Dropoff_Min, Dropoff_Sec

🚖 **Trip Dimension** (dim_trip.csv)

passenger_count, trip_distance, RatecodeID, VendorID
store_and_fwd_flag, PULocationID, DOLocationID, payment_type

#### 💾 **File Export**

Saved all tables as CSV files for easy analysis
Files ready for import into databases or BI tools
Downloaded files from Google Colab environment

#### 📁 **Output Files**

**fact_table.csv** - Financial and fare data
**dim_date.csv** - Time-based dimensions
**dim_trip.csv** - Trip characteristics and metadata
- **trip_distance**
- All **time components** (Hour, Min, Sec for both pickup and dropoff)
