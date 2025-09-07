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
- **trip_distance**
- All **time components** (Hour, Min, Sec for both pickup and dropoff)
