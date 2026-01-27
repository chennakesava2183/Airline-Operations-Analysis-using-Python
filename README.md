# ✈️ Airline Operations Analysis using Python

## 📌 Project Overview
This project performs an end-to-end exploratory and analytical study of airline operations, focusing on flight delays, cancellations, airline performance, airport congestion, and traffic patterns. 

Using Python and data analysis libraries, the project extracts actionable insights that help understand:

- Which airlines are most reliable
- Which airports experience the highest delays
- How delays vary by time, route, and season
- Major reasons behind flight cancellations

The insights generated in Python can be exported and visualized interactively in Power BI.

## 🎯 Objectives
- Analyze arrival and departure delays
- Identify on-time vs delayed airline performance
- Study flight cancellations and their reasons
- Understand hourly, daily, and monthly traffic trends
- Identify high-traffic and high-delay routes
- Prepare aggregated datasets for dashboarding

## 📊 Dataset Description
The dataset contains commercial flight records with the following key attributes:

| Attribute | Description |
|-----------|-------------|
| Flight Date | Year, Month, Day, Hour |
| Airline Codes | IATA, Airline |
| Origin & Destination Airports | Origin Airport, Destination Airport |
| Scheduled and Actual Times | Scheduled Time, Departure Delay, Departure Time, Taxi Out, Wheels Off etc|
| Arrival & Departure Delays | Scheduled Arrival, Elapsed Time, Departure Time, Arrival Delay, Taxi In, Wheels In etc|
| Cancellation Status and Reasons | Cancelled, Cancelled Reason |
| Distance Travelled | Distance, Airtime |

The dataset is pre-cleaned for analysis by handling missing values, invalid time formats, and inconsistent categorical data.

## 🛠️ Tools & Technologies Used

### Programming & Libraries
- **Python**
- **pandas** – data manipulation
- **numpy** – numerical operations
- **matplotlib** – static visualizations

# Dataset File 
Dataset on which I worked (https://mavenanalytics.io/data-playground/airline-flight-delays)

## 🔄 Data Cleaning & Preparation
Key preprocessing steps include:

- Extracting Month Names from Month Number Data
- Extracting hour of day from scheduled times
- Handling: NaN / None / NaT values
- Empty and whitespace strings
- Selective row removal (`dropna(subset=...)`)
- Standardizing month order using categorical data
- Creating derived metrics (on-time %, cancellation rate)

## 📈 Key Analyses Performed

### 1️⃣ Delay Analysis
- Median Arrival Delay by Airline
- Median Departure Delay by Hour of Day
- Distance vs Delay Scatter Analysis

### 2️⃣ Cancellation Analysis
- Cancellation Rate by Airline
- Cancellation Reasons Distribution
- Cancellations by Hour of Day

### 3️⃣ Airline Performance
- On-time performance percentage
- Worst and best performing airlines

### 4️⃣ Airport & Route Insights
- Busiest airports by flight volume
- Most congested destination airports
- Routes with highest air traffic

## 📊 Visualizations Created
- Line charts (hourly and monthly trends)
- Bar and horizontal bar charts
- Histograms (delay distributions)
- Scatter plots (distance vs delay)
- Pie charts (cancellation reasons)
- Area charts (monthly traffic trends)

**All charts are:**
- Properly labeled
- Scaled for readability


## ✅ Key Business Insights (Example)
- Certain airlines consistently maintain lower median delays
- Peak delays occur during late evening hours
- Summer months show higher flight volume and congestion
- Weather-related cancellations dominate over technical issues
- High-traffic routes do not always have the highest delays

## 🚀 Future Enhancements
- Predictive delay modeling using ML
- Weather data integration
- Route-level optimization analysis
- Real-time dashboarding
- Automated data quality checks

## 👤 Author
**Chenna Kesava Kumar Bonu**  
*Data Analyst | Python | Power BI | SQL*

## 📜 License
This project is for educational and portfolio purposes.

