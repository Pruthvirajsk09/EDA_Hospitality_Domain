# EDA_Hospitality_Domain
# 🏨 AtliQ Hotels Data Analysis Project

## 📖 Overview

This project presents a comprehensive analysis of booking data from **AtliQ Hotels** to identify patterns, uncover insights, and improve operational decisions. The analysis is performed in a Jupyter Notebook using Python and pandas.

---

## 📁 Datasets Used

The project makes use of the following CSV files:

- `dim_date.csv` - Contains date-related metadata
- `dim_hotels.csv` - Information on each hotel property
- `dim_rooms.csv` - Room types and capacities
- `fact_aggregated_bookings.csv` - Aggregated booking facts
- `fact_bookings.csv` - Raw transactional booking data

---

## 🧭 Project Workflow

### 1️⃣ Data Import & Exploration
- Load all datasets
- Preview data using `.head()`, `.info()`, and summary statistics
- Understand relationships between datasets

### 2️⃣ Data Cleaning
- Remove invalid entries (e.g., guests < 0)
- Analyze and assess revenue outliers
- Handle missing values in customer ratings appropriately
- Detect and handle data inconsistencies such as bookings exceeding capacity

### 3️⃣ Data Transformation
- Calculate **occupancy percentage**:
  ```python
  df["occupancy_%"] = (df["successful_bookings"] / df["capacity"]) * 100

### 🧪 Exercises & Business Questions Answered
1)Identify unique property IDs from the aggregated bookings

2)Calculate total bookings per property

3)Identify overbooked days (bookings > capacity)

4)Find properties with the highest capacities

5)Evaluate rating distribution and null value handling

### 💻 Tools & Technologies
- Python 3
- Jupyter Notebook
- Pandas for data wrangling

